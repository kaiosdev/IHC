
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

---

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
 <img width="895" height="724" alt="Captura de tela 2025-11-03 140331" src="https://github.com/user-attachments/assets/a7c60da5-87d0-4887-9a7a-ec2bb2791773" />

  * [7.2 OneR](#72-oner)

 <img width="829" height="672" alt="Captura de tela 2025-11-03 140612" src="https://github.com/user-attachments/assets/bb55a3f9-da6a-4ed9-95ec-0206dbbc4964" />

  * [7.3 J48 (Árvore de Decisão)](#73-j48-árvore-de-decisão)

 <img width="920" height="666" alt="Captura de tela 2025-11-03 140725" src="https://github.com/user-attachments/assets/c5d57ce9-73e5-4695-98ae-33ee6f2c0749" />

  * [7.4 Naive Bayes](#74-naive-bayes)

<img width="829" height="651" alt="Captura de tela 2025-11-03 141122" src="https://github.com/user-attachments/assets/c145559f-e4a8-4a46-bab3-637e373e0354" />
 
  * [7.5 IBk (k-Nearest Neighbors)](#75-ibk-k-nearest-neighbors)

<img width="799" height="660" alt="Captura de tela 2025-11-03 141228" src="https://github.com/user-attachments/assets/aadda2c5-e3bf-4905-b852-e297f876b0cf" />

 
  * [7.6 Tabela Comparativa dos Resultados](#76-tabela-comparativa-dos-resultados)
* [8. Análise do Modelo da Árvore de Decisão (J48)](#8-análise-do-modelo-da-árvore-de-decisão-j48)
* [9. Resultados (tabelas, matrizes de confusão, prints de tela)](#9-resultados-tabelas-matrizes-de-confusão-prints-de-tela)
* [10. Análise crítica dos resultados em relação ao domínio de IHС](#10-análise-crítica-dos-resultados-em-relação-ao-domínio-de-ihс)

---

Este trabalho tem como objetivo integrar conceitos de Interação Humano-Computador (IHC) e Aprendizado de Máquina (Machine Learning) para resolver um problema de classificação supervisionada. O foco é utilizar métricas de interação para prever a qualidade da usabilidade de um sistema, conforme proposto nos objetivos do projeto.

## 1. Contexto e Motivação

O problema de classificação foi formulado no contexto de um aplicativo hipotético chamado "Agenda Fácil", projetado para profissionais autônomos (como manicures, barbeiros e personal trainers) gerenciarem seus agendamentos de clientes. A principal proposta de valor do aplicativo é ser simples e eficiente, minimizando a chance de erros comuns em agendamentos manuais.

A motivação para este estudo é investigar se é possível treinar um modelo de machine learning para classificar automaticamente o nível de usabilidade de uma sessão de uso, com base em dados quantitativos da interação do usuário. Tal modelo poderia, no futuro, ajudar desenvolvedores a identificar pontos de atrito na interface e a validar melhorias de design de forma automatizada, prevendo se uma interação foi positiva ou negativa.

## 2. Atributos Preditores

Para treinar o modelo, foram selecionados 5 atributos preditores que representam diferentes aspectos de uma tarefa central do aplicativo: "realizar um novo agendamento". Esses atributos foram escolhidos por serem métricas clássicas de usabilidade, como tempo de tarefa e número de erros.

* **tempo_para_agendar (Numérico):** Tempo total, em segundos, que o usuário levou para concluir a tarefa de agendamento. Mede a eficiência.
* **passos_ate_concluir (Numérico):** Número total de cliques ou toques necessários para finalizar o agendamento. Mede a complexidade do fluxo de interação.
* **usou_lista_clientes (Nominal: {sim, não}):** Indica se o usuário utilizou a funcionalidade de selecionar um cliente já cadastrado, uma ação que representa um caminho mais eficiente.
* **ativou_lembrete (Nominal: {sim, nao}):** Verifica se o usuário ativou a função de lembrete automático, indicando engajamento com funcionalidades chave do sistema.
* **erros_no_fluxo (Numérico):** Quantidade de erros cometidos durante o processo, como clicar em um botão desabilitado ou tentar agendar em um horário já ocupado. Mede a eficácia.

## 3. Classe-Alvo

A classe-alvo, ou seja, o atributo que desejamos prever, foi definida para representar a qualidade geral da usabilidade da sessão.

* **Nome da Classe:** nível_usabilidade
* **Valores Possíveis:** {Alta, Media, Baixa}
* **Tipo de Problema:** Multiclasse

Cada valor representa uma avaliação da interação: Alta indica uma experiência fluida e eficiente; Média indica que a tarefa foi concluída, mas com alguma dificuldade; e Baixa indica uma experiência frustrante e ineficiente.

## 4. Regras usadas para gerar a classe-alvo

* **Usabilidade Alta:** tempo_agendar < 45 segundos E erros_fluxo = 0
* **Usabilidade Baixa:** tempo_agendar > 120 segundos OU erros_fluxo > 2
* **Usabilidade Média:** Casos que não se enquadram nas condições anteriores.

## 5. Descrição da Base Sintética

A base de dados utilizada neste trabalho, denominada `base_sintetica.arff`, foi gerada artificialmente para simular o comportamento de usuários no aplicativo "Agenda Fácil". O objetivo foi criar um conjunto de dados controlado para treinar um modelo de Machine Learning capaz de classificar o nível de usabilidade de uma interação com base em métricas de desempenho. A geração foi guiada por um conjunto de regras explícitas, detalhadas na proposta do projeto.

A base de dados contém 200 instâncias e 6 atributos, sendo 5 atributos preditores e 1 atributo-alvo (a classe). Os atributos são descritos a seguir:

* **tempo_agendar (Numérico):** Representa o tempo total, em segundos, que o usuário levou para concluir um agendamento.
* **passos_concluir (Numérico):** Indica o número de cliques ou toques que o usuário realizou para finalizar a tarefa.
* **usou_lista_clientes (Nominal: {sim, nao}):** Informa se o usuário utilizou a lista de clientes pré-cadastrados, um recurso que otimiza o fluxo.
* **ativou_lembrete (Nominal: {sim, nao}):** Verifica se o usuário ativou funcionalidades adicionais, como lembretes para o agendamento.
* **erros_fluxo (Numérico):** Quantifica o número de erros cometidos pelo usuário durante o processo de agendamento.
* **nivel_usabilidade (Nominal: {Alta, Media, Baixa}):** Este é o atributo-alvo (classe). Ele classifica a interação do usuário em três níveis de usabilidade, com base nas regras de geração de dados.

Esse conjunto de dados serve como alicerce para os experimentos, permitindo a aplicação de algoritmos de classificação para identificar padrões que se correlacionam com uma experiência de usuário positiva ou negativa.

## 6. Descrição dos Experimentos no Weka

Nesta etapa, foi utilizada a ferramenta Weka Explorer para a análise exploratória e experimental da base de dados `base_sintetica.arff`.

### 6.1 Análise Visual dos Dados

Inicialmente, os dados foram carregados na aba "Visualize", onde foi gerada uma Matriz de Gráficos de Dispersão (Plot Matrix) para observar a distribuição dos atributos e suas possíveis correlações. As instâncias foram coloridas de acordo com a variável-alvo `nivel_usabilidade`, conforme a legenda:

* Azul escuro: Alta usabilidade
* Vermelho: Média usabilidade
* Ciano: Baixa usabilidade

A partir dessa análise, foi possível identificar os seguintes padrões:

* **Correlação entre atributos numéricos:** Observou-se uma correlação positiva entre os atributos `tempo_agendar` e `passos_concluir`. As instâncias formam uma tendência diagonal, indicando que tarefas que exigem mais passos também demandam mais tempo. A classe Alta (azul escuro) concentra-se em valores baixos de tempo e passos, a classe Média (vermelho) apresenta valores intermediários, e a classe Baixa (ciano) predomina em valores elevados.
* **Separação das classes:** Os atributos numéricos demonstraram uma boa capacidade de distinguir as classes de usabilidade. `tempo_agendar` e `passos_concluir` baixos tendem a indicar usabilidade Alta, enquanto valores altos apontam para usabilidade Baixa. O atributo `erros_fluxo` também se mostrou um forte preditor: 0 erros está associado à predominância da classe Alta, 1 a 2 erros à Média, e acima de 2 erros à Baixa.
* **Influência dos atributos categóricos:** Verificou-se que a maioria das instâncias da classe Alta ocorre quando `usou_lista_clientes` e `ativou_lembrete` possuem valor "sim", sugerindo que o uso dessas funcionalidades está associado a uma melhor percepção de usabilidade.

A exploração inicial indicou padrões visuais bem definidos e uma separação clara entre as classes, o que sugere que os algoritmos de aprendizado de máquina devem ser capazes de aprender regras de classificação com alta precisão.


