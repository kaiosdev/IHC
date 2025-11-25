# Diagramas MoLIC - Modeling Language for Interaction as Conversation

##  Objetivo

Os diagramas MoLIC (Modeling Language for Interaction as Conversation) representam a interação entre usuário e sistema como uma **conversa estruturada**, onde cada cena representa um momento de diálogo e as transições mostram como o usuário navega entre diferentes contextos de interação.

---

##  Fundamentos da Linguagem MoLIC

A linguagem MoLIC é baseada na **Engenharia Semiótica** e trata a interação como um processo de comunicação. Os principais elementos são:

### Elementos Visuais

- ** Cena (Scene)**: Representa um momento de interação onde o usuário pode realizar ações
- ** Transição**: Mostra como o usuário passa de uma cena para outra
- ** Ponto de Decisão**: Representa escolhas que o sistema faz com base em condições
- ** Fala do Designer**: Mensagens que o sistema comunica ao usuário
- ** Fala do Usuário**: Ações e intenções expressas pelo usuário
- ** Processamento**: Operações do sistema que não envolvem diretamente o usuário
- ** Ruptura de Comunicação**: Pontos onde a conversa pode falhar ou ser interrompida

---

##  Visão Geral do Sistema E-Project

# Diagramas MoLIC - Modeling Language for Interaction as Conversation

##  Objetivo

Os diagramas MoLIC (Modeling Language for Interaction as Conversation) representam a interação entre usuário e sistema como uma **conversa estruturada**, onde cada cena representa um momento de diálogo e as transições mostram como o usuário navega entre diferentes contextos de interação.

---

##  Fundamentos da Linguagem MoLIC

A linguagem MoLIC é baseada na **Engenharia Semiótica** e trata a interação como um processo de comunicação. Os principais elementos são:


##  Diagrama MoLIC Geral

> **Visualização completa do sistema mostrando todos os fluxos integrados**

(https://miro.com/app/board/uXjVJl0c37E=/)

*Diagrama MoLIC Geral - Visão completa dos fluxos de interação do E-Project*

### Descrição Geral

O diagrama apresenta a arquitetura conversacional completa do sistema, onde:

- **Ponto de Entrada**: Login/Autenticação (cena inicial comum a todos)
- **Bifurcação por Perfil**: Após autenticação, o sistema direciona para o dashboard específico
- **Fluxos Paralelos**: Cada persona tem seu próprio caminho de navegação
- **Pontos de Convergência**: Configurações de acessibilidade podem ser acessadas de qualquer fluxo
- **Saídas**: Logout e conclusão de tarefas como pontos finais

---

# Design de Interação - MoLIC

Este documento descreve a modelagem da interação do **Sistema de Gestão de Projetos Acadêmicos** (focado em PIBIC/PACE), utilizando a notação **MoLIC** (Modeling Language for Interaction as Conversation).

O objetivo destes diagramas é mapear os diálogos entre o usuário e o sistema, prevendo fluxos de sucesso, tratamento de erros e personalização da interface.

##  Legenda da Notação
* **u:** Ação ou fala do Usuário.
* **d:** Ação, resposta ou fala do Designer (representado pelo sistema).
* **Retângulos Arredondados:** Cenas (momentos da interação).
* **Caixas Internas:** Detalhes da interface ou opções disponíveis naquela cena.
* **XOR:** Escolha exclusiva (o usuário faz um ou outro).

---

## 1. Autenticação e Acesso
**Objetivo:** Garantir o acesso seguro ao sistema através da validação de credenciais.

![Diagrama de Autenticação e Dashboard](./caminho/para/imagem_login.jpg)

* **Fluxo Principal:** O usuário (`u`) manifesta a intenção de entrar no sistema.
* **Interação (Autenticar no Sistema):**
    * O sistema solicita e o usuário informa (`d+u`):
        * **Matrícula/e-mail**
        * **Senha**
        * **Manter conectado** (opção selecionável)
    * O usuário confirma o acesso (`u: confirmar acesso`).
* **Processamento:**
    * O sistema verifica a validade das informações.
* **Desvios:**
    * **Falha:** Se o login for inválido ou usuário não encontrado (`d`), o sistema retorna à tela de autenticação para nova tentativa.
    * **Sucesso:** Se as credenciais forem válidas (`d`), o sistema direciona o usuário para o **Dashboard**.

---

## Dashboard e Navegação
**Objetivo:** Centralizar as operações principais disponíveis para o usuário autenticado.

* **Estado Atual:** Usuário logado na tela "Dashboard".
* **Opções de Navegação (`u`):**
    O usuário pode escolher seguir para os seguintes fluxos (representados pelos conectores):
    1.  **Gerenciar orientandos** $\rightarrow$ Leva ao fluxo **A**.
    2.  **Ver minhas tarefas** $\rightarrow$ Leva ao fluxo **B**.
    3.  **Cadastrar projeto** $\rightarrow$ Leva ao fluxo **C**.
    4.  **Consultar editais** $\rightarrow$ Leva ao fluxo **D**.
    5.  **Biblioteca de modelos** $\rightarrow$ Leva ao fluxo **E**.
* **Saída:**
    * **SAIR:** O usuário opta por encerrar a sessão, finalizando a interação com o sistema (símbolo de encerramento).

---

## 2. Personalização e Acessibilidade
**Objetivo:** Permitir que o usuário adapte a interface às suas necessidades visuais e cognitivas.

![Diagrama de Acessibilidade](./caminho/para/imagem_acessibilidade.jpg)
*(Substitua pelo caminho real da imagem 1001307664.jpg)*

O sistema oferece dois caminhos principais de ajuste:
1.  **Acessibilidade Visual:**
    * Ajuste de Contraste (Alto contraste vs. Padrão).
    * Tipografia (Aumentar fonte ou Fonte para dislexia).
    * Zoom de navegação.
2.  **Suporte Cognitivo (Gerenciar Foco):**
    * **Modo de Trabalho:** Sem distrações vs. Normal.
    * **Suporte Visual:** Ícones com rótulos ou Cores semânticas.
    * **Orientação:** Exibição de checklist da tarefa atual.

---

## 3. Gestão de Projetos (Advisor/Aluno)
**Objetivo:** Cadastro de novos projetos acadêmicos e integração com sistemas externos.

![Diagrama de Novo Projeto](./caminho/para/imagem_projeto.jpg)
*(Substitua pelo caminho real da imagem 1001307667.jpg)*

* **Cena: Novo Projeto Acadêmico**
    * **Integração:** O sistema permite importar dados diretamente do *E-Campus*.
        * `d`: Exibe erro na integração se falhar ou carrega dados automaticamente se sucesso.
    * **Definições:** Seleção de modalidade (PIBIC/PACE).
    * **Equipe:** Busca e adição de alunos.
        * `d`: Feedback se matrícula não for encontrada ou vínculo realizado com sucesso.
    * **Finalização:** O sistema valida campos obrigatórios antes de ativar o projeto.

---

## 4. Exploração de Editais
**Objetivo:** Permitir que o usuário encontre oportunidades de bolsas e projetos.

![Diagrama de Editais](./caminho/para/imagem_editais.jpg)
*(Substitua pelo caminho real da imagem 1001307668.jpg)*

* **Interação:** O usuário consulta editais a partir do Dashboard.
* **Funcionalidades:**
    * Filtros por status ou pré-reitoria.
    * Download do edital (com tratamento de erro de conexão).
    * Opção de favoritar editais para acesso rápido.

---

## 5. Fluxo de Orientação (Visão do Orientador)
**Objetivo:** Gerenciar as atividades dos orientandos e fornecer feedback.

![Diagrama de Orientação](./caminho/para/imagem_orientador.jpg)
*(Substitua pelo caminho real da imagem 1001307665.jpg)*

* **Cena: Gerenciar Atividades**
    * O orientador pode **Criar Nova Tarefa** (definindo título, prazo e anexos).
    * O orientador pode **Revisar Entregas**:
        * Visualiza a produção e histórico.
        * Decide entre **Aprovar** ou **Solicitar Correção**.
    * **Feedback:** Se solicitar correção, insere motivos/orientações que retornam ao aluno.

---

## 6. Realização de Tarefas (Visão do Aluno)
**Objetivo:** Acompanhar pendências e realizar entregas.

![Diagrama de Tarefas](./caminho/para/imagem_aluno.jpg)
*(Substitua pelo caminho real da imagem 1001307666.jpg)*

* **Cena: Lista de Pendências**
    * O aluno visualiza prazos e status.
* **Cena: Detalhes da Tarefa**
    * Lê orientações.
    * Realiza o upload do arquivo (entrega).
    * `d`: Sistema confirma entrega ou alerta sobre erro no upload.

---

## 7. Geração de Documentos
**Objetivo:** Automatizar a criação de relatórios e requerimentos.

![Diagrama de Documentos](./caminho/para/imagem_docs.jpg)
*(Substitua pelo caminho real da imagem 1001307669.jpg)*

* **Fluxo:**
    1.  **Configurar Documento:** Seleciona modelo (Relatório de Atividades ou Requerimento).
    2.  **Dados:** O sistema preenche o cabeçalho vinculado automaticamente, usuário edita dados específicos.
    3.  **Pré-visualização:** O sistema exibe o documento gerado.
    4.  **Exportação:** Usuário baixa o arquivo final.

---

##  Ferramentas Utilizadas
* Diagramação: Miro
