<div align="center">

<h1>Relatório Final: Classificação de Usabilidade</h1>

<img src="https://img.shields.io/badge/Disciplina-IHC_&_Machine_Learning-00663C?style=for-the-badge&logo=googlescholar&logoColor=white">
<img src="https://img.shields.io/badge/Prof.-Andrey_Rodrigues-005875?style=for-the-badge&logo=teacher&logoColor=white">
<img src="https://img.shields.io/badge/Ferramenta-Weka-3b3b3b?style=for-the-badge&logo=weka&logoColor=white">

<br><br>

> **TP2 - Classificação Supervisionada Aplicada a Problemas de Usabilidade**
> Projeto "Agenda Fácil": Previsão automática da qualidade de interação do usuário.

</div>

---

## 1. Contexto e Motivação
O problema de classificação foi formulado no contexto de um aplicativo hipotético chamado **“Agenda Fácil”**, projetado para profissionais autônomos gerenciarem agendamentos. A principal proposta de valor é a simplicidade e eficiência.

**Motivação:** Investigar se é possível treinar um modelo de *machine learning* para classificar automaticamente o nível de usabilidade de uma sessão, baseando-se em dados quantitativos. Isso auxiliaria na identificação automática de pontos de atrito na interface.

---

## 2. Atributos Preditores
Foram selecionados **5 atributos preditores** representando a tarefa "realizar um novo agendamento".

| Atributo | Tipo | Significado |
| :--- | :---: | :--- |
| **`tempo_para_agendar`** | Numérico | Tempo total (segundos). Mede a **eficiência**. |
| **`passos_ate_concluir`** | Numérico | Total de cliques/toques. Mede a **complexidade**. |
| **`usou_lista_clientes`** | Nominal | `{sim, nao}`. Indica uso de funcionalidade de atalho. |
| **`ativou_lembrete`** | Nominal | `{sim, nao}`. Indica engajamento. |
| **`erros_no_fluxo`** | Numérico | Quantidade de erros (ex: cliques inválidos). Mede a **eficácia**. |

---

## 3. Classe-Alvo
A classe representa a qualidade geral da usabilidade da sessão.
* **Nome da Classe:** `nivel_usabilidade`
* **Valores:** `{Alta, Media, Baixa}`

| Nível | Descrição |
| :--- | :--- |
| 🟢 **Alta** | Experiência fluida e eficiente. |
| 🟡 **Média** | Tarefa concluída com alguma dificuldade. |
| 🔴 **Baixa** | Experiência frustrante e ineficiente. |

---

## 4. Regras Geradoras
As regras utilizadas para definir a classe-alvo na base sintética foram:

* **Usabilidade Alta:** `tempo_agendar < 45s` **E** `erros_fluxo = 0`
* **Usabilidade Baixa:** `tempo_agendar > 120s` **OU** `erros_fluxo > 2`
* **Usabilidade Média:** Casos que não se enquadram nas condições anteriores.
---

## 5. Descrição da Base Sintética
A base `base_sintetica.arff` contém **200 instâncias** e **6 atributos** (5 preditores + 1 classe). Ela foi criada artificialmente para simular o comportamento de usuários do aplicativo.

---

## 6. Experimentos no Weka
A ferramenta **Weka Explorer** foi utilizada para análise.

### 6.1 Análise Visual (Plot Matrix)
Os dados foram visualizados por meio de uma Matriz de Gráficos de Dispersão.
* 🟦 **Azul escuro:** Alta usabilidade
* 🟥 **Vermelho:** Média usabilidade
* cyan **Ciano:** Baixa usabilidade

**Padrões observados:**
1.  **Correlação:** `tempo_agendar` e `passos_concluir` são positivamente correlacionados.
2.  **Separação:** Instâncias com baixo tempo e poucos passos pertencem à classe Alta.
3.  **Categóricos:** O uso de `lista_clientes` e `lembrete` ("sim") está associado a melhor usabilidade.

---

## 7. Resultados da Classificação
Foram testados os algoritmos abaixo com **Percentage Split (66% treino)**.

### 7.1 ZeroR (Baseline)
* **Acurácia:** 46,97%
* **Matriz de Confusão:**
    ```text
    a  b  c <-- classificado como
    0 18  0 | a = Alta
    0 31  0 | b = Media
    0 17  0 | c = Baixa
    ```

### 7.2 OneR
* **Acurácia:** 98,48%
* **Matriz de Confusão:**
    ```text
    a  b  c <-- classificado como
    17  1  0 | a = Alta
    0 31  0 | b = Media
    0  0 17 | c = Baixa
    ```

### 7.3 J48 (Árvore de Decisão)
* **Acurácia:** 100%
* **Matriz de Confusão:**
    ```text
    a  b  c <-- classificado como
    18  0  0 | a = Alta
    0 31  0 | b = Media
    0  0 17 | c = Baixa
    ```

### 7.4 Naive Bayes
* **Acurácia:** 100%
* **Matriz de Confusão:**
    ```text
    a  b  c <-- classificado como
    18  0  0 | a = Alta
    0 31  0 | b = Media
    0  0 17 | c = Baixa
    ```

### 7.5 IBk (k-NN)
* **Configuração:** k=1
* **Acurácia:** 98,48%
* **Matriz de Confusão:**
    ```text
    a  b  c <-- classificado como
    18  0  0 | a = Alta
    0 30  1 | b = Media
    0  0 17 | c = Baixa
    ```

### 7.6 Tabela Comparativa Final

| Algoritmo | Acurácia | Instâncias Corretas |
| :--- | :---: | :---: |
| **J48** | **100%** | **66/66** |
| **Naive Bayes** | **100%** | **66/66** |
| OneR | 98.48% | 65/66 |
| IBk (kNN) | 98.48% | 65/66 |
| ZeroR | 46.97% | 31/66 |

---

## 8. Análise do Modelo (J48)
O modelo J48 é altamente interpretável e revelou regras claras:

1.  **Fator Decisivo (Tempo):** O atributo mais importante é `tempo_agendar`. Se `tempo > 120s`, a usabilidade é **Baixa**. Isso demonstra que a **eficiência** é o pilar principal.
2.  **Diferencial (Erros):** Para tempos aceitáveis (`<= 120s`), o fator determinante é `erros_fluxo`.
    * `erros > 0` → **Média**
    * `erros = 0` → **Alta**

---

## 9. Resultados Visuais

<div align="center">
<table>
  <tr>
    <td align="center"><strong>Fig 1. Aba Visualize</strong></td>
    <td align="center"><strong>Fig 2. Dispersão: Tempo</strong></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/218014b7-c388-46e3-b77f-e0fc8bf271d4" width="400"></td>
    <td><img src="https://github.com/user-attachments/assets/88221e05-42da-4039-8c0c-8a4e5ea9a0fb" width="400"></td>
  </tr>
  <tr>
    <td align="center"><strong>Fig 3. Dispersão: Passos</strong></td>
    <td align="center"><strong>Fig 4. ZeroR (Baseline)</strong></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/a89f9b3c-d610-42b4-bd07-4f4eab14018d" width="400"></td>
    <td><img src="https://github.com/user-attachments/assets/a7c60da5-87d0-4887-9a7a-ec2bb2791773" width="400"></td>
  </tr>
  <tr>
    <td align="center"><strong>Fig 5. OneR</strong></td>
    <td align="center"><strong>Fig 6. Naive Bayes</strong></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/bb55a3f9-da6a-4ed9-95ec-0206dbbc4964" width="400"></td>
    <td><img src="https://github.com/user-attachments/assets/c145559f-e4a8-4a46-bab3-637e373e0354" width="400"></td>
  </tr>
  <tr>
    <td align="center"><strong>Fig 7. IBk (k-NN)</strong></td>
    <td align="center"><strong>Fig 8. J48 (Árvore)</strong></td>
  </tr>
  <tr>
    <td><img src="https://github.com/user-attachments/assets/aadda2c5-e3bf-4905-b852-e297f876b0cf" width="400"></td>
    <td><img src="https://github.com/user-attachments/assets/c5d57ce9-73e5-4695-98ae-33ee6f2c0749" width="400"></td>
  </tr>
</table>
</div>

---

## 10. Análise Crítica dos Resultados
Os modelos J48 e Naive Bayes obtiveram **100% de acurácia**, comprovando que os atributos escolhidos explicam bem a usabilidade.

**Conclusões:**
* **Eficiência:** `tempo_agendar` é o critério decisivo.
* **Eficácia:** A ausência de erros diferencia a usabilidade Alta da Média.
* Atributos secundários tiveram impacto mínimo.

O estudo comprova que modelos de Machine Learning podem servir como ferramentas de diagnóstico para apoiar o design centrado no usuário.

---

## 👥 Equipe de Desenvolvimento

<div align="center">

| ID | Discente |
| :---: | :--- |
| **A1** | Geovanna Beathryz |
| **A2** | Gustavo Souza |
| **A3** | Iasmim Braga |
| **A4** | Jean Barauna |
| **A5** | Kaio Sobral |
| **A6** | Pedro Jheivison |

</div>
