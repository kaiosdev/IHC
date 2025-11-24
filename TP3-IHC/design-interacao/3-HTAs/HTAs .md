# Análise Hierárquica de Tarefas (HTA)

Esta pasta contém a modelagem detalhada das tarefas principais do sistema. A Análise Hierárquica de Tarefas (HTA) foi utilizada para decompor os objetivos dos usuários (definidos nos Mapas de Objetivos) em operações concretas, planos e subtarefas, garantindo que a interface ofereça suporte lógico para a realização das atividades.

---

## Critérios de Escolha das Tarefas

Para atender aos requisitos do **Trabalho Prático 3 (Design de Interação)**, selecionamos um conjunto de 8 HTAs que cobrem:

1. **Tarefas Críticas (Core Business):** O ciclo de vida dos projetos acadêmicos (Cadastro, Execução e Orientação).
2. **Automação e Eficiência:** Tarefas que demonstram integração com sistemas externos (E-Campus) para reduzir o esforço do usuário.
3. **Acessibilidade e Inclusão:** Funcionalidades específicas para remover barreiras visuais e cognitivas, atendendo à Persona PcD.
4. **Fluxos de Alta Frequência:** Ações recorrentes como Login e Consulta de Editais.

---

## Detalhamento dos HTAs

### 1. Realizar Login do Sistema
**Objetivo:** Garantir acesso seguro e personalizado ao ambiente do usuário.

<img width="1000" alt="Captura de tela 2025-11-24 165440" src="https://github.com/user-attachments/assets/9ac6a613-ea20-4d8e-9480-c8864f958210" />

* **Descrição do Processo:** O fluxo cobre o caminho feliz (inserir credenciais) e os desvios comuns, como a recuperação de senha (2.1). O sistema valida as credenciais antes de liberar o acesso ao Dashboard.
* **Comentário de Design:** Incluímos a opção "Manter conectado" (2.4) para reduzir a carga de memória e esforço físico em acessos futuros, melhorando a eficiência.

---

### 2. Cadastrar Novo Projeto (Foco: Integração)
**Objetivo:** Permitir que o professor registre um projeto aproveitando dados institucionais existentes.

<img width="1000" alt="Captura de tela 2025-11-24 165458" src="https://github.com/user-attachments/assets/7d2435a4-c02c-4176-8607-0460c4ec0f38" />

* **Descrição do Processo:** O diferencial deste fluxo é a **automação**. Ao selecionar a modalidade (1), o sistema realiza a subtarefa (2) "Importar Dados do E-Campus" automaticamente, preenchendo campos burocráticos sem intervenção do usuário.
* **Comentário de Design:** A tarefa de vincular orientandos (4) foi modelada como um ciclo (loop), permitindo buscar (4.1) e adicionar (4.2) múltiplos alunos sem sair da tela, otimizando o fluxo de cadastro de equipes grandes.

---

### 3. Consultar Feed Unificado de Editais
**Objetivo:** Centralizar oportunidades de bolsas e projetos em um único local pesquisável.

<img width="1000" alt="Captura de tela 2025-11-24 165541" src="https://github.com/user-attachments/assets/1dfaee82-b01c-4003-95fc-e924c3257df7" />

* **Descrição do Processo:** O usuário inicia com uma visão geral e utiliza filtros (2) para refinar a busca por Pró-Reitoria ou Status. A etapa de ação (3) permite tanto o download imediato quanto o "favoritar" para leitura posterior.
* **Comentário de Design:** A separação entre "Baixar" (3.1) e "Favoritar" (3.2) atende a dois contextos de uso: o usuário que está no desktop pronto para ler (baixa) e o usuário mobile que apenas quer salvar para depois (favorita).

---

### 4. Gerenciar Tarefas do Orientando (Visão do Professor)
**Objetivo:** Permitir ao orientador acompanhar e validar o progresso dos bolsistas.

<img width="1000" alt="Captura de tela 2025-11-24 165601" src="https://github.com/user-attachments/assets/d89d76f2-bfcc-453b-b908-56d150be5bb2" />

* **Descrição do Processo:** Este HTA divide-se em dois momentos: a atribuição proativa (1) e a reação reativa de análise (2). A decisão final (3) é binária: ou solicita correção ou aprova a tarefa.
* **Comentário de Design:** O fluxo enfatiza o feedback. Ao "Solicitar correção" (3.1), o sistema exige input do orientador, garantindo que o aluno saiba exatamente o que precisa ser melhorado.

---

### 5. Execução de Tarefas pelo Aluno (Visão do Discente)
**Objetivo:** Orientar o aluno na entrega de suas obrigações acadêmicas.

<img width="1000" alt="Captura de tela 2025-11-24 165614" src="https://github.com/user-attachments/assets/df35a980-e780-411b-b21a-e1ffaa5282b2" />

* **Descrição do Processo:** Espelha o HTA do orientador. O aluno consulta pendências (1), realiza a entrega via upload (2) e monitora o status no histórico (3).
* **Comentário de Design:** A subtarefa "Ver prazo da tarefa" (1.3) foi explicitada para reforçar a gestão de tempo, um ponto crítico para evitar a evasão ou perda de bolsas.

---

### 6. Gerar Documentação Automática
**Objetivo:** Reduzir a burocracia na criação de relatórios e requerimentos.

<img width="1000" alt="Captura de tela 2025-11-24 165630" src="https://github.com/user-attachments/assets/c0c53118-668c-461d-8a56-222ba5a8b79b" />

* **Descrição do Processo:** O usuário seleciona um modelo (2) e o sistema executa a tarefa crítica de "Vincular dados do projeto" (3) automaticamente, preenchendo cabeçalhos e informações repetitivas.
* **Comentário de Design:** A inclusão da etapa "Visualizar prévia" (4.1) antes do download final previne erros e o retrabalho de baixar/abrir arquivos incorretos.

---

### 7. Acessar Opções de Acessibilidade Visual
**Objetivo:** Adaptar a interface para usuários com baixa visão ou dificuldades de leitura.

<img width="1000" alt="Captura de tela 2025-11-24 165701" src="https://github.com/user-attachments/assets/dec4d78e-03c9-4944-b7ad-1178081e5e08" />

* **Descrição do Processo:** Funciona como um painel de configuração onde o usuário pode ajustar contraste (1), tipografia (2) ou simplificar a navegação (3).
* **Comentário de Design:** A opção "Navegar por fluxos lineares" (3.1) é crucial para usuários de leitores de tela, transformando grids complexos em listas sequenciais lógicas.

---

### 8. Acessar Opções de Acessibilidade Cognitiva
**Objetivo:** Reduzir a carga cognitiva para usuários com TDAH, ansiedade ou neurodivergências.

<img width="1000" alt="Captura de tela 2025-11-24 165840" src="https://github.com/user-attachments/assets/69f5fd51-07a2-472f-bc27-376ad1b11fac" />

* **Descrição do Processo:** O foco é a redução de ruído. O usuário pode ativar o "Modo sem distrações" (2.1) ou solicitar "Orientação de tarefa" (1) para saber exatamente qual o próximo passo.
* **Comentário de Design:** A funcionalidade "Identificar a próxima ação" (1.2) atua como um assistente que quebra a paralisia de decisão, guiando o usuário diretamente para o que é prioritário.

---
