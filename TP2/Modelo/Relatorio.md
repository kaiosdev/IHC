# RELATÓRIO FINAL

## Classificação Supervisionada Aplicada a Problemas de Usabilidade

**TP2 – IHC e Machine Learning – Prof. Andrey Rodrigues**

**Autores:**  
GEOVANNA BEATHRYZ  
GUSTAVO SOUZA  
IASMIM BRAGA  
JEAN BARAÚNA  
KAIO SOBRAL  
PEDRO JHEIVISON  


## 1. Contexto e Motivação

O problema de classificação foi formulado no contexto de um aplicativo hipotético chamado **“Agenda Fácil”**, projetado para profissionais autônomos (como manicures, barbeiros e personal trainers) gerenciarem seus agendamentos de clientes.  
A principal proposta de valor do aplicativo é ser simples e eficiente, minimizando a chance de erros comuns em agendamentos manuais.

A motivação para este estudo é investigar se é possível treinar um modelo de *machine learning* para classificar automaticamente o nível de usabilidade de uma sessão de uso, com base em dados quantitativos da interação do usuário.  
Tal modelo poderia, no futuro, ajudar desenvolvedores a identificar pontos de atrito na interface e a validar melhorias de design de forma automatizada, prevendo se uma interação foi positiva ou negativa.


## 2. Atributos Preditores

Foram selecionados **5 atributos preditores** que representam diferentes aspectos da tarefa central do aplicativo: “realizar um novo agendamento”.  
Esses atributos foram escolhidos por serem métricas clássicas de usabilidade, como tempo de tarefa e número de erros.

- **tempo_para_agendar (Numérico):** Tempo total, em segundos, que o usuário levou para concluir a tarefa de agendamento. Mede a **eficiência**.  
- **passos_ate_concluir (Numérico):** Número total de cliques ou toques necessários para finalizar o agendamento. Mede a **complexidade do fluxo**.  
- **usou_lista_clientes (Nominal: {sim, não}):** Indica se o usuário utilizou a funcionalidade de selecionar um cliente já cadastrado.  
- **ativou_lembrete (Nominal: {sim, nao}):** Verifica se o usuário ativou a função de lembrete automático, indicando engajamento.  
- **erros_no_fluxo (Numérico):** Quantidade de erros cometidos durante o processo, como clicar em um botão desabilitado ou tentar agendar em um horário já ocupado. Mede a **eficácia**.


## 3. Classe-Alvo

A classe-alvo representa a qualidade geral da usabilidade da sessão.

- **Nome da Classe:** `nivel_usabilidade`  
- **Valores Possíveis:** {Alta, Media, Baixa}  
- **Tipo de Problema:** Multiclasse

Cada valor indica:
- **Alta:** experiência fluida e eficiente  
- **Média:** tarefa concluída com alguma dificuldade  
- **Baixa:** experiência frustrante e ineficiente


## 4. Regras usadas para gerar a classe-alvo

- **Usabilidade Alta:** `tempo_agendar < 45s` **E** `erros_fluxo = 0`  
- **Usabilidade Baixa:** `tempo_agendar > 120s` **OU** `erros_fluxo > 2`  
- **Usabilidade Média:** Casos que não se enquadram nas condições anteriores


## 5. Descrição da Base Sintética

A base `base_sintetica.arff` contém **200 instâncias** e **6 atributos** (5 preditores e 1 classe).  
Ela foi criada artificialmente para simular o comportamento de usuários do aplicativo.

**Atributos:**
- `tempo_agendar` (Numérico)  
- `passos_concluir` (Numérico)  
- `usou_lista_clientes` (Nominal: {sim, nao})  
- `ativou_lembrete` (Nominal: {sim, nao})  
- `erros_fluxo` (Numérico)  
- `nivel_usabilidade` (Nominal: {Alta, Media, Baixa})


## 6. Descrição dos Experimentos no Weka

A ferramenta **Weka Explorer** foi utilizada para análise e experimentação da base `base_sintetica.arff`.

### 6.1 Análise Visual dos Dados

Os dados foram visualizados por meio de uma **Matriz de Gráficos de Dispersão (Plot Matrix)**.

**Legenda das classes:**
- Azul escuro → Alta usabilidade  
- Vermelho → Média usabilidade  
- Ciano → Baixa usabilidade  

**Padrões observados:**
- **Correlação entre atributos:** `tempo_agendar` e `passos_concluir` são positivamente correlacionados.  
- **Separação das classes:** instâncias com baixo tempo e poucos passos pertencem à classe Alta.  
- **Atributos categóricos:** uso de `lista_clientes` e `lembrete` (“sim”) está associado a melhor usabilidade.


## 7. Resultados dos Experimentos de Classificação

Foram testados os algoritmos: **ZeroR, OneR, J48, Naive Bayes e IBk (k-NN)**.  
A divisão da base foi feita com **Percentage Split (66% treino)**.

### 7.1 ZeroR

**Acurácia:** 46,97%

```
a  b  c <-- classified as
0 18  0 | a = Alta
0 31  0 | b = Media
0 17  0 | c = Baixa
```

### 7.2 OneR

**Acurácia:** 98,48%

```
a  b  c <-- classified as
17  1  0 | a = Alta
0  31  0 | b = Media
0  0  17 | c = Baixa
```

### 7.3 J48 (Árvore de Decisão)

**Acurácia:** 100%

```
a  b  c <-- classified as
18  0  0 | a = Alta
0  31  0 | b = Media
0  0  17 | c = Baixa
```

### 7.4 Naive Bayes

**Acurácia:** 100%

```
a  b  c <-- classified as
18  0  0 | a = Alta
0  31  0 | b = Media
0  0  17 | c = Baixa
```

### 7.5 IBk (k-NN)

**Configuração:** k = 1  
**Acurácia:** 98,48%

```
a  b  c <-- classified as
18  0  0 | a = Alta
0  30  1 | b = Media
0  0  17 | c = Baixa
```

### 7.6 Tabela Comparativa dos Resultados

| Algoritmo | Acurácia | Instâncias Corretamente Classificadas |
|------------|-----------|--------------------------------------|
| ZeroR | 46,97% | 31 / 66 |
| OneR | 98,48% | 65 / 66 |
| IBk (kNN) | 98,48% | 65 / 66 |
| J48 | 100% | 66 / 66 |
| Naive Bayes | 100% | 66 / 66 |


## 8. Análise do Modelo da Árvore de Decisão (J48)

O modelo J48 é altamente interpretável. Ele revelou regras claras entre atributos e níveis de usabilidade.

### Fator Decisivo: Tempo na Tarefa
O atributo mais importante é `tempo_agendar`.  
Se `tempo_agendar > 120`, a usabilidade é **Baixa**.  
Isso demonstra que **eficiência** é o principal pilar da usabilidade.

### Diferencial: Ausência de Erros
Para `tempo_agendar <= 120`, o fator determinante é `erros_fluxo`:  
- `erros_fluxo > 0` → **Média**  
- `erros_fluxo = 0` → **Alta**

Essas regras confirmam que a **eficiência (tempo)** e **eficácia (erros)** definem a experiência de usabilidade.


## 9. Resultados Visuais

<div align="center">
 
   Figura 1 - Aba “Visualize”
 
   <img width="889" height="689" alt="Captura de tela 2025-11-03 150805" src="https://github.com/user-attachments/assets/218014b7-c388-46e3-b77f-e0fc8bf271d4" /> 
 
   Figura 2- Gráfico de Dispersão : tempo_agendar 
   
   <img width="899" height="660" alt="Captura de tela 2025-11-03 150813" src="https://github.com/user-attachments/assets/88221e05-42da-4039-8c0c-8a4e5ea9a0fb" />
   
   Figura 3- Gráfico de Dispersão: passos_concluir 
   
   <img width="903" height="709" alt="Captura de tela 2025-11-03 150823" src="https://github.com/user-attachments/assets/a89f9b3c-d610-42b4-bd07-4f4eab14018d" />
   
   Figura 4- ZeroR (Baseline) 
   
   <img width="895" height="724" alt="Captura de tela 2025-11-03 140331" src="https://github.com/user-attachments/assets/a7c60da5-87d0-4887-9a7a-ec2bb2791773" />
   
   Figura 5- OneR (Baseline) 
   
   <img width="829" height="672" alt="Captura de tela 2025-11-03 140612" src="https://github.com/user-attachments/assets/bb55a3f9-da6a-4ed9-95ec-0206dbbc4964" />
   
   Figura 6- Algoritmo NaiveBayes  
   
   <img width="829" height="651" alt="Captura de tela 2025-11-03 141122" src="https://github.com/user-attachments/assets/c145559f-e4a8-4a46-bab3-637e373e0354" />
  
   Figura 7- Algoritmo IBk (k-NN) 
   
   <img width="799" height="660" alt="Captura de tela 2025-11-03 141228" src="https://github.com/user-attachments/assets/aadda2c5-e3bf-4905-b852-e297f876b0cf" />
   
   Figura 8- J48 (Árvore de Decisão)
   
   <img width="920" height="666" alt="Captura de tela 2025-11-03 140725" src="https://github.com/user-attachments/assets/c5d57ce9-73e5-4695-98ae-33ee6f2c0749" />
</div>

## 10. Análise Crítica dos Resultados

Os modelos J48 e Naive Bayes obtiveram **100% de acurácia**, enquanto OneR e IBk chegaram a **98,48%**.  
Isso mostra que os atributos escolhidos explicam bem a usabilidade do sistema.

**Conclusões principais:**
- **Eficiência:** `tempo_agendar` é o critério decisivo.  
- **Eficácia:** ausência de erros diferencia a usabilidade Alta da Média.  
- **Atributos secundários** (`usou_lista_clientes`, `ativou_lembrete`) tiveram impacto mínimo.  

O estudo comprova que é possível prever objetivamente a usabilidade com métricas de interação.  
Modelos de *machine learning* podem, portanto, servir como ferramentas de diagnóstico para apoiar o design centrado no usuário.


Este trabalho tem como objetivo integrar conceitos de Interação Humano-Computador (IHC) e Aprendizado de Máquina (Machine Learning) para resolver um problema de classificação supervisionada. O foco é utilizar métricas de interação para prever a qualidade da usabilidade de um sistema, conforme proposto nos objetivos do projeto.
