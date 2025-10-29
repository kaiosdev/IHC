# RELATÓRIO FINAL

## Classificação Supervisionada Aplicada a Problemas de Usabilidade

**TP2 - IHC e Machine Learning - Prof. Andrey Rodrigues**

**Autores:**

  * GEOVANNA BEATHRYZ
  * GUSTAVO SOUZA
  * IASMIM BRAGA
  * JEAN BARAÚNA 
  * ΚΑΙΟ SOBRAL
  * PEDRO JHEIVISON
-----

## Sumário

  * [1. Contexto e Motivação](#1-contexto-e-motivação)
  * [2. Atributos Preditores](#2-atributos-preditores)
  * [3. Classe-Alvo](#3-classe-alvo)
  * [4. Regras usadas para gerar a classe-alvo](#4-regras-usadas-para-gerar-a-classe-alvo)
  * [5. Descrição da Base Sintética](#5-descrição-da-base-sintética)
  * [6. Descrição dos Experimentos no Weka](#6-descrição-dos-experimentos-no-weka)
      * [6.1 Análise Visual dos Dados](#61-análise-visual-dos-dados)
  * [7. Resultados dos Experimentos de Classificação](#7-resultados-dos-experimentos-de-classificação)
      * [7.1 ZeroR](#71-zeror)
      * [7.2 OneR](#72-oner)
      * [7.3 J48 (Árvore de Decisão)](#73-j48-árvore-de-decisão)
      * [7.4 Naive Bayes](#74-naive-bayes)
      * [7.5 IBk (k-Nearest Neighbors)](#75-ibk-k-nearest-neighbors)
      * [7.6 Tabela Comparativa dos Resultados](#76-tabela-comparativa-dos-resultados)
  * [8. Análise do Modelo da Árvore de Decisão (J48)](#8-análise-do-modelo-da-árvore-de-decisão-j48)
  * [9. Resultados (tabelas, matrizes de confusão, prints de tela)](#9-resultados-tabelas-matrizes-de-confusão-prints-de-tela)
  * [10. Análise crítica dos resultados em relação ao domínio de IHС](#10-análise-crítica-dos-resultados-em-relação-ao-domínio-de-ihс)

-----

Este trabalho tem como objetivo integrar conceitos de Interação Humano-Computador (IHC) e Aprendizado de Máquina (Machine Learning) para resolver um problema de classificação supervisionada[cite: 37]. [cite\_start]O foco é utilizar métricas de interação para prever a qualidade da usabilidade de um sistema, conforme proposto nos objetivos do projeto.

## 1\. Contexto e Motivação

O problema de classificação foi formulado no contexto de um aplicativo hipotético chamado "Agenda Fácil", projetado para profissionais autônomos (como manicures, barbeiros e personal trainers) gerenciarem seus agendamentos de clientes. A principal proposta de valor do aplicativo é ser simples e eficiente, minimizando a chance de erros comuns em agendamentos manuais.

A motivação para este estudo é investigar se é possível treinar um modelo de machine learning para classificar automaticamente o nível de usabilidade de uma sessão de uso, com base em dados quantitativos da interação do usuário. Tal modelo poderia, no futuro, ajudar desenvolvedores a identificar pontos de atrito na interface e a validar melhorias de design de forma automatizada, prevendo se uma interação foi positiva ou negativa.

## 2\. Atributos Preditores

Para treinar o modelo, foram selecionados 5 atributos preditores que representam diferentes aspectos de uma tarefa central do aplicativo: "realizar um novo agendamento"[cite: 45]. [cite\_start]Esses atributos foram escolhidos por serem métricas clássicas de usabilidade, como tempo de tarefa e número de erros[cite: 46].

  * **tempo\_para\_agendar (Numérico):** Tempo total, em segundos, que o usuário levou para concluir a tarefa de agendamento. [cite\_start]Mede a eficiência[cite: 47].
  * **passos\_ate\_concluir (Numérico):** Número total de cliques ou toques necessários para finalizar o agendamento. [cite\_start]Mede a complexidade do fluxo de interação[cite: 48].
  * **usou\_lista\_clientes (Nominal: {sim, não}):** Indica se o usuário utilizou a funcionalidade de selecionar um cliente já cadastrado, uma ação que representa um caminho mais eficiente[cite: 50].
  * [cite\_start]**ativou\_lembrete (Nominal: {sim, nao}):** Verifica se o usuário ativou a função de lembrete automático, indicando engajamento com funcionalidades chave do sistema[cite: 51].
  * **erros\_no\_fluxo (Numérico):** Quantidade de erros cometidos durante o processo, como clicar em um botão desabilitado ou tentar agendar em um horário já ocupado. [cite\_start]Mede a eficácia[cite: 52, 53].

## 3\. Classe-Alvo

[cite\_start]A classe-alvo, ou seja, o atributo que desejamos prever, foi definida para representar a qualidade geral da usabilidade da sessão[cite: 55, 56].

  * [cite\_start]**Nome da Classe:** nível\_usabilidade [cite: 57]
  * [cite\_start]**Valores Possíveis:** {Alta, Media, Baixa} [cite: 58]
  * [cite\_start]**Tipo de Problema:** Multiclasse [cite: 58]

Cada valor representa uma avaliação da interação: Alta indica uma experiência fluida e eficiente; [cite\_start]Média indica que a tarefa foi concluída, mas com alguma dificuldade; e Baixa indica uma experiência frustrante e ineficiente[cite: 59, 60].

## 4\. Regras usadas para gerar a classe-alvo

  * **Usabilidade Alta:** tempo\_agendar \< 45 segundos E erros\_fluxo = 0
  * **Usabilidade Baixa:** tempo\_agendar \> 120 segundos OU erros\_fluxo \> 2
  * **Usabilidade Média:** Casos que não se enquadram nas condições anteriores.
    [cite\_start][cite: 62]

## 5\. Descrição da Base Sintética

A base de dados utilizada neste trabalho, denominada `base_sintetica.arff`, foi gerada artificialmente para simular o comportamento de usuários no aplicativo "Agenda Fácil"[cite: 64]. [cite\_start]O objetivo foi criar um conjunto de dados controlado para treinar um modelo de Machine Learning capaz de classificar o nível de usabilidade de uma interação com base em métricas de desempenho[cite: 65]. [cite\_start]A geração foi guiada por um conjunto de regras explícitas, detalhadas na proposta do projeto[cite: 66].

A base de dados contém 200 instâncias e 6 atributos, sendo 5 atributos preditores e 1 atributo-alvo (a classe)[cite: 67]. Os atributos são descritos a seguir:

  * [cite\_start]**tempo\_agendar (Numérico):** Representa o tempo total, em segundos, que o usuário levou para concluir um agendamento[cite: 70].
  * [cite\_start]**passos\_concluir (Numérico):** Indica o número de cliques ou toques que o usuário realizou para finalizar a tarefa[cite: 71].
  * [cite\_start]**usou\_lista\_clientes (Nominal: {sim, nao}):** Informa se o usuário utilizou a lista de clientes pré-cadastrados, um recurso que otimiza o fluxo[cite: 72].
  * [cite\_start]**ativou\_lembrete (Nominal: {sim, nao}):** Verifica se o usuário ativou funcionalidades adicionais, como lembretes para o agendamento[cite: 73].
  * [cite\_start]**erros\_fluxo (Numérico):** Quantifica o número de erros cometidos pelo usuário durante o processo de agendamento[cite: 74].
  * **nivel\_usabilidade (Nominal: {Alta, Media, Baixa}):** Este é o atributo-alvo (classe). [cite\_start]Ele classifica a interação do usuário em três níveis de usabilidade, com base nas regras de geração de dados.

Esse conjunto de dados serve como alicerce para os experimentos, permitindo a aplicação de algoritmos de classificação para identificar padrões que se correlacionam com uma experiência de usuário positiva ou negativa.

## 6\. Descrição dos Experimentos no Weka

Nesta etapa, foi utilizada a ferramenta Weka Explorer para a análise exploratória e experimental da base de dados `base_sintetica.arff`.

### 6.1 Análise Visual dos Dados

[cite\_start]Inicialmente, os dados foram carregados na aba "Visualize", onde foi gerada uma Matriz de Gráficos de Dispersão (Plot Matrix) para observar a distribuição dos atributos e suas possíveis correlações[cite: 81]. [cite\_start]As instâncias foram coloridas de acordo com a variável-alvo `nivel_usabilidade`, conforme a legenda[cite: 82]:

  * [cite\_start]Azul escuro: Alta usabilidade [cite: 83]
  * [cite\_start]Vermelho: Média usabilidade [cite: 84]
  * [cite\_start]Ciano: Baixa usabilidade [cite: 85]

A partir dessa análise, foi possível identificar os seguintes padrões:

  * [cite\_start]**Correlação entre atributos numéricos:** Observou-se uma correlação positiva entre os atributos `tempo_agendar` e `passos_concluir`[cite: 87]. [cite\_start]As instâncias formam uma tendência diagonal, indicando que tarefas que exigem mais passos também demandam mais tempo[cite: 88]. [cite\_start]A classe Alta (azul escuro) concentra-se em valores baixos de tempo e passos, a classe Média (vermelho) apresenta valores intermediários, e a classe Baixa (ciano) predomina em valores elevados[cite: 89, 91].
  * [cite\_start]**Separação das classes:** Os atributos numéricos demonstraram uma boa capacidade de distinguir as classes de usabilidade[cite: 92]. [cite\_start]`tempo_agendar` e `passos_concluir` baixos tendem a indicar usabilidade Alta, enquanto valores altos apontam para usabilidade Baixa[cite: 93]. [cite\_start]O atributo `erros_fluxo` também se mostrou um forte preditor: 0 erros está associado à predominância da classe Alta, 1 a 2 erros à Média, e acima de 2 erros à Baixa[cite: 94].
  * [cite\_start]**Influência dos atributos categóricos:** Verificou-se que a maioria das instâncias da classe Alta ocorre quando `usou_lista_clientes` e `ativou_lembrete` possuem valor "sim", sugerindo que o uso dessas funcionalidades está associado a uma melhor percepção de usabilidade[cite: 96, 97].

A exploração inicial indicou padrões visuais bem definidos e uma separação clara entre as classes, o que sugere que os algoritmos de aprendizado de máquina devem ser capazes de aprender regras de classificação com alta precisão[cite: 98].

## 7\. Resultados dos Experimentos de Classificação

Para avaliar a capacidade de predição do nível de usabilidade, foram treinados e testados cinco algoritmos de classificação: ZeroR, OneR, J48, Naive Bayes e IBk[cite: 100]. [cite\_start]A base de dados foi dividida com a abordagem Percentage Split, utilizando 66% dos dados para treino[cite: 101]. [cite\_start]A seguir, são apresentados os resultados detalhados para cada modelo[cite: 102].

### 7.1 ZeroR

O ZeroR, um classificador de linha de base, previu sempre a classe majoritária "Media"[cite: 104].

  * **Acurácia:** 46,9697%
  * **Matriz de Confusão:**
    ```
    a  b  c <-- classified as
    0 18  0 | a = Alta
    0 31  0 | b = Media
    0 17  0 | c = Baixa
    ```


### 7.2 OneR

[cite\_start]O OneR (One Rule) gerou uma regra de classificação baseada no atributo que melhor prediz a classe-alvo[cite: 112].

  * [cite\_start]**Acurácia:** 98,4848% [cite: 113]
  * **Matriz de Confusão:**
    ```
    a  b  c <-- classified as
    17  1  0 | a = Alta
     0 31  0 | b = Media
     0  0 17 | c = Baixa
    ```
    [cite\_start][cite: 115-118]

### 7.3 J48 (Árvore de Decisão)

[cite\_start]O J48 é uma implementação do algoritmo C4.5 que gera uma árvore de decisão para classificar as instâncias[cite: 120].

  * [cite\_start]**Acurácia:** 100% [cite: 121]
  * **Matriz de Confusão:**
    ```
    a  b  c <-- classified as
    18  0  0 | a = Alta
     0 31  0 | b = Media
     0  0 17 | c = Baixa
    ```
    [cite\_start][cite: 123-127]

### 7.4 Naive Bayes

[cite\_start]Este classificador probabilístico utiliza o teorema de Bayes com a suposição de independência entre os atributos[cite: 129].

  * [cite\_start]**Acurácia:** 100% [cite: 130]
  * **Matriz de Confusão:**
    ```
    a  b  c <-- classified as
    18  0  0 | a = Alta
     0 31  0 | b = Media
     0  0 17 | c = Baixa
    ```
    [cite\_start][cite: 132-136]

### 7.5 IBk (k-Nearest Neighbors)

O IBk é um classificador baseado em instâncias. [cite\_start]Foi utilizado com a configuração padrão (k=1)[cite: 138].

  * [cite\_start]**Acurácia:** 98,4848% [cite: 139]
  * **Matriz de Confusão:**
    ```
    a  b  c <-- classified as
    18  0  0 | a = Alta
     0 30  1 | b = Media
     0  0 17 | c = Baixa
    ```
    [cite\_start][cite: 141-147]

### 7.6 Tabela Comparativa dos Resultados

| Algoritmo | Acurácia | Instâncias Corretamente Classificadas |
| :--- | :---: | :---: |
| ZeroR | 46,97% | 31/66 |
| OneR | 98,48% | 65/66 |
| IBk (KNN) | 98,48% | 65/66 |
| J48 | 100% | 66/66 |
| Naive Bayes | 100% | 66/66 |

## 8\. Análise do Modelo da Árvore de Decisão (J48)

Uma das principais vantagens do algoritmo J48 é a alta interpretabilidade do seu modelo[cite: 151]. [cite\_start]A árvore de decisão gerada revela um conjunto de regras hierárquicas e claras que o algoritmo "descobriu" a partir dos dados, fornecendo insights valiosos sobre a relação entre os atributos e o nível de usabilidade[cite: 152].

**O Fator Decisivo: Tempo na Tarefa (tempo\_agendar)**
A raiz da árvore, e portanto o atributo mais importante, é o `tempo_agendar`[cite: 153]. O modelo aprendeu um limiar crítico de 120 segundos. [cite\_start]Se o tempo para concluir a tarefa excede esse valor, a usabilidade é incondicionalmente classificada como Baixa[cite: 154]. [cite\_start]Isso demonstra que, no contexto do sistema avaliado, a eficiência é o principal pilar da percepção de usabilidade[cite: 155].

**O Diferencial para a Qualidade: Ausência de Erros (erros\_fluxo)**
[cite\_start]Para tarefas concluídas em tempo aceitável (\<= 120 segundos), o fator determinante para a qualidade da experiência passa a ser a ocorrência de erros[cite: 157, 159]. O modelo aprendeu que:

  * [cite\_start]Se o usuário comete pelo menos um erro (\> 0), a usabilidade é classificada como Média[cite: 160].
  * [cite\_start]Apenas quando a tarefa é concluída de forma eficiente e sem nenhum erro (\<= 0) a usabilidade atinge o nível Alta[cite: 161].

As regras extraídas da árvore de decisão validam empiricamente conceitos fundamentais de Interação Humano-Computador[cite: 162]. [cite\_start]O modelo confirmou que uma boa usabilidade é uma função direta da eficiência (baixo tempo para completar a tarefa) e da eficácia (ausência de erros)[cite: 163]. [cite\_start]A clareza do modelo J48 não só resultou em uma acurácia perfeita, mas também forneceu uma explicação lógica e alinhada com a teoria de IHC para o problema de classificação proposto[cite: 164].

## 9\. Resultados (tabelas, matrizes de confusão, prints de tela)

#### Figura 1 - Aba "Visualize"
<img width="892" height="688" alt="Captura de tela 2025-10-28 195730" src="https://github.com/user-attachments/assets/31e12011-6949-43ff-baeb-774de27605da" />



#### Figura 2 - Gráfico de Dispersão: tempo\_agendar

<img width="901" height="658" alt="Captura de tela 2025-10-28 195912" src="https://github.com/user-attachments/assets/a893653b-aedb-4bad-8325-31898e63b964" />


#### Figura 3 - Gráfico de Dispersão: passos\_concluir

<img width="900" height="707" alt="Captura de tela 2025-10-28 200041" src="https://github.com/user-attachments/assets/91d0025d-81c0-44bd-8f1f-e494e1aabbf7" />


#### Figura 4 - ZeroR (Baseline)
<img width="919" height="744" alt="Captura de tela 2025-10-28 200213" src="https://github.com/user-attachments/assets/b79d83d6-985f-41cc-9896-38e343c3ad1c" />



#### Figura 5 - OneR (Baseline)
<img width="910" height="731" alt="Captura de tela 2025-10-28 200256" src="https://github.com/user-attachments/assets/70da1670-20b6-4ee2-9e35-f3109d5a6975" />



#### Figura 6 - Algoritmo Naive Bayes
<img width="913" height="700" alt="Captura de tela 2025-10-28 200345" src="https://github.com/user-attachments/assets/3efd59e3-725b-418f-98d6-99b15025e21d" />


#### Figura 7 - Algoritmo IBk (k-NN)

<img width="871" height="712" alt="Captura de tela 2025-10-28 200435" src="https://github.com/user-attachments/assets/7e228fc1-fe5f-4717-8834-194858366446" />


#### Figura 8 - J48 (Árvore de Decisão)


<img width="833" height="592" alt="J48" src="https://github.com/user-attachments/assets/f7ccb22d-c7ca-47a8-85bb-d5d042df6a9d" />


## 10\. Análise crítica dos resultados em relação ao domínio de IHС

A análise comparativa do desempenho dos modelos no conjunto de teste (66 instâncias) revelou uma alta previsibilidade dos dados, permitindo extrair conclusões significativas sobre a avaliação da experiência do usuário no domínio de IHC aplicado ao sistema "Agenda Fácil"[cite: 554].

  * [cite\_start]**ZeroR (Baseline):** Atingiu apenas 46,97% de acurácia[cite: 555]. [cite\_start]Como esperado, ele classificou todas as instâncias de teste como a classe majoritária, "Media"[cite: 555]. [cite\_start]Isso define a linha de base: qualquer modelo útil deve superar esse valor[cite: 556].
  * [cite\_start]**OneR (Baseline):** Demonstrou um salto significativo, alcançando 98,48% de acurácia[cite: 557]. [cite\_start]Ele errou apenas 1 das 66 instâncias, indicando que um único atributo (provavelmente `tempo_agendar` ou `erros_fluxo`) era um preditor muito forte[cite: 558].
  * [cite\_start]**IBk (k-NN):** Teve um desempenho idêntico ao OneR, com 98,48% de acurácia[cite: 559]. [cite\_start]Sua matriz de confusão mostra que também cometeu apenas um erro, classificando uma instância "Media" como "Alta"[cite: 560].
  * [cite\_start]**J48 e Naive Bayes:** Ambos os modelos atingiram o desempenho máximo de 100% de acurácia[cite: 561]. [cite\_start]Eles conseguiram classificar corretamente todas as 66 instâncias de teste sem nenhum erro[cite: 562].

[cite\_start]Os resultados demonstram que a usabilidade, neste contexto, não é um conceito puramente subjetivo[cite: 563]. [cite\_start]Pelo contrário, ela pode ser quantificada e prevista com um nível de precisão notavelmente alto[cite: 564]. [cite\_start]O desempenho perfeito dos algoritmos J48 e Naive Bayes indica que os atributos de interação selecionados possuem uma forte correlação com a classificação da experiência do usuário[cite: 565].

[cite\_start]A análise do modelo J48 (Árvore de Decisão), que se destaca pela sua interpretabilidade, oferece os insights mais claros[cite: 566]:

1.  [cite\_start]**A Eficiência como Pilar Central:** A árvore elegeu o atributo `tempo_agendar` como o nó raiz, identificando-o como o fator mais decisivo para a classificação da usabilidade[cite: 567]. [cite\_start]O modelo aprendeu que um tempo de tarefa superior a 120 segundos resulta, incondicionalmente, em uma classificação de usabilidade "Baixa"[cite: 568]. [cite\_start]Isso sugere que, para o perfil de usuário deste aplicativo, a eficiência e a velocidade na conclusão da tarefa são os principais pilares da experiência percebida[cite: 571].

2.  [cite\_start]**A Eficácia como Diferencial para a Excelência:** Após o critério de eficiência ser atendido (tempo \<= 120s), o modelo utiliza a eficácia (`erros_fluxo`) como o fator de desempate[cite: 572]. [cite\_start]A árvore demonstra que apenas as interações concluídas sem nenhum erro (`erros_fluxo` \<= 0) alcançam o nível "Alta"[cite: 572]. [cite\_start]A ocorrência de qualquer erro (`erros_fluxo` \> 0), mesmo que o tempo tenha sido satisfatório, rebaixa a classificação para "Média"[cite: 572].

3.  **A Validação das Regras: O que o J48 "Descobriu" vs o que foi Definido.**
    [cite\_start]Um dos objetivos centrais do trabalho era verificar se o modelo conseguiria "aprender" os padrões de usabilidade predefinidos[cite: 574]. [cite\_start]Ao comparar as regras originais com as extraídas da árvore de decisão J48, confirma-se que o modelo não só encontrou os padrões, como também os otimizou[cite: 575].

      * **Para a classe Baixa:** A regra original era `tempo_agendar > 120 segundos OU erros_fluxo > 2`. [cite\_start]O J48 aprendeu uma regra mais direta: apenas `tempo_agendar > 120`[cite: 575]. [cite\_start]Isso revela que o tempo de tarefa foi um indicador tão forte que se sobrepôs à necessidade de analisar os erros para identificar uma experiência ruim[cite: 576].
      * **Para a classe Alta:** A regra original era `tempo_agendar < 45 segundos E erros_fluxo = 0`. [cite\_start]O J48 generalizou essa condição para `tempo_agendar <= 120 E erros_fluxo <= 0`[cite: 577]. [cite\_start]O modelo expandiu o critério de tempo, entendendo que qualquer tarefa concluída em um tempo razoável e sem erros poderia ser classificada como de alta usabilidade[cite: 577].

[cite\_start]Em suma, os resultados validam empiricamente que a experiência do usuário no "Agenda Fácil" é uma função direta dos dois principais pilares da usabilidade: eficiência (tempo) e eficácia (erros)[cite: 578]. [cite\_start]Notavelmente, atributos secundários de engajamento, como `usou_lista_clientes` ou `ativou_lembrete`, não foram selecionados pela árvore J48, indicando que seu impacto na classificação da usabilidade é irrelevante quando comparado à velocidade e à ausência de erros[cite: 579].

[cite\_start]Para o domínio de IHC, isso comprova que um modelo de machine learning pode ser uma ferramenta poderosa de diagnóstico[cite: 580]. [cite\_start]Ele permite à equipe de design focar em métricas objetivas: para otimizar a experiência do usuário deste sistema, os esforços devem ser direcionados a garantir que o fluxo da tarefa principal possa ser concluído em menos de 120 segundos e de forma tão intuitiva que minimize a ocorrência de erros[cite: 581, 583].
