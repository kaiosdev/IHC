<div align="center">

<h1>DIAGRAMAS DE INTERAÇÃO (MoLIC)</h1>

<img src="https://img.shields.io/badge/Disciplina-IHC-791297?style=for-the-badge&logo=googlescholar&logoColor=white" alt="Disciplina IHC">
<img src="https://img.shields.io/badge/Artefato-Engenharia_Semiótica-c38ae2?style=for-the-badge&logo=wechat&logoColor=white" alt="Engenharia Semiótica">

<br><br>

> **A Interação como Conversa**
> <br>Modelagem dos fluxos de diálogo entre o usuário e o sistema, focando nas rupturas e na comunicabilidade.

<a href="https://miro.com/app/board/uXjVJl0c37E=/">
  <img src="https://img.shields.io/badge/ACESSAR_MOLIC_NO_MIRO_➔-791297?style=for-the-badge&logo=miro&logoColor=white" alt="Acessar Miro">
</a> 

</div>

---

## 1. Fundamentos da Linguagem

A linguagem MoLIC (Modeling Language for Interaction as Conversation) baseia-se na **Engenharia Semiótica** para tratar a interação como um processo de comunicação.

| Elemento | Descrição |
| :--- | :--- |
| **Cena (Scene)** | Representa um momento de interação onde o usuário pode realizar ações. |
| **Transição** | Mostra como o usuário passa de uma cena para outra. |
| **Ponto de Decisão** | Representa escolhas que o sistema faz com base em condições pré-definidas. |
| **Fala do Designer** | Mensagens, feedbacks ou rótulos que o sistema comunica ao usuário. |
| **Fala do Usuário** | Ações, cliques e intenções expressas pelo usuário. |
| **Processamento** | Operações internas do sistema que não envolvem interação direta. |
| **Ruptura** | Pontos onde a conversa pode falhar ou ser interrompida (erros). |

---

## 2. Visão Geral do Sistema

### 🗺️ Diagrama MoLIC Geral
> **Arquitetura conversacional completa do E-Project**

<div align="center">
  <img width="100%" src="LINK_DA_SUA_IMAGEM_GERAL_AQUI" alt="Diagrama Geral">
  <br>
  <sub><b>Figura 1:</b> Visão panorâmica dos fluxos de interação (Fonte: Elaboração própria/Miro)</sub>
</div>

**Descrição do Fluxo Macro:**
* **Ponto de Entrada:** Autenticação (cena comum a todos).
* **Bifurcação:** Direcionamento para dashboards específicos após login.
* **Convergência:** Configurações de acessibilidade acessíveis de qualquer ponto.
* **Saída:** Logout e conclusão de tarefas como encerramento da conversa.

---

## 3. Detalhamento dos Fluxos de Conversa

### 🔐 1. Autenticação e Acesso
![Foco](https://img.shields.io/badge/FOCO-SEGURANÇA-791297?style=flat-square)

**Objetivo:** Garantir o acesso seguro através da validação de credenciais.

<div align="center">
  <img width="100%" src="./caminho/para/imagem_login.jpg" alt="MoLIC Autenticação">
</div>

* **Interação Inicial:** O usuário (`u`) manifesta intenção de entrar.
* **Diálogo de Credenciais (`d+u`):**
    * Sistema solicita: **Matrícula/e-mail** e **Senha**.
    * Usuário preenche e pode marcar "Manter conectado".
    * Usuário confirma (`u`: confirmar acesso).
* **Processamento & Desvios:**
    * **Falha:** Sistema (`d`) informa erro e retorna à cena de login.
    * **Sucesso:** Sistema (`d`) valida e transita para o **Dashboard**.

---

### ♿ 2. Personalização e Acessibilidade
![Foco](https://img.shields.io/badge/FOCO-ADAPTAÇÃO-c38ae2?style=flat-square)

**Objetivo:** Permitir a adaptação da interface às necessidades visuais e cognitivas.

<div align="center">
  <img width="100%" src="./caminho/para/imagem_acessibilidade.jpg" alt="MoLIC Acessibilidade">
</div>

O diálogo de configuração oferece dois caminhos principais:

1.  **Acessibilidade Visual (`u` seleciona):**
    * Ajuste de Contraste (Alto contraste / Padrão).
    * Tipografia (Aumentar fonte / Fonte para dislexia).
    * Zoom de navegação.
2.  **Suporte Cognitivo (`u` seleciona):**
    * **Modo de Trabalho:** Ativar "Sem distrações".
    * **Suporte Visual:** Ativar ícones com rótulos e cores semânticas.
    * **Orientação:** Exibir checklist da tarefa atual.

---

### 📂 3. Gestão de Projetos (Orientador)
![Foco](https://img.shields.io/badge/FOCO-INTEGRAÇÃO-791297?style=flat-square)

**Objetivo:** Cadastro de novos projetos acadêmicos e integração com sistemas externos.

<div align="center">
  <img width="100%" src="./caminho/para/imagem_projeto.jpg" alt="MoLIC Novo Projeto">
</div>

* **Cena: Novo Projeto Acadêmico**
    * **Integração (`System`):** Sistema tenta importar dados do *E-Campus*.
        * `d`: Exibe erro se falhar ou carrega dados se sucesso.
    * **Definições (`u`):** Seleciona modalidade (PIBIC/PACE).
    * **Equipe (`u` + `d`):**
        * Usuário busca aluno por matrícula.
        * `d`: Feedback (Aluno encontrado ou Matrícula inválida).
    * **Encerramento:** Sistema valida obrigatórios e ativa o projeto.

---

### 📢 4. Exploração de Editais
![Foco](https://img.shields.io/badge/FOCO-INFORMAÇÃO-c38ae2?style=flat-square)

**Objetivo:** Encontrar oportunidades de bolsas e projetos.

<div align="center">
  <img width="100%" src="./caminho/para/imagem_editais.jpg" alt="MoLIC Editais">
</div>

* **Interação:** Consulta iniciada a partir do Dashboard.
* **Ações do Usuário (`u`):**
    * Filtrar por Status ou Pró-Reitoria.
    * Baixar Edital (Download).
    * Favoritar para acesso rápido.
* **Tratamento de Erro:** Sistema alerta caso o download falhe por conexão.

---

### 🎓 5. Fluxo de Orientação
![Foco](https://img.shields.io/badge/FOCO-FEEDBACK-791297?style=flat-square)

**Objetivo:** Gerenciar atividades dos orientandos e fornecer feedback pedagógico.

<div align="center">
  <img width="100%" src="./caminho/para/imagem_orientador.jpg" alt="MoLIC Orientação">
</div>

* **Cena: Gerenciar Atividades**
    * **Ação 1 (`u`):** Criar Nova Tarefa (título, prazo, anexos).
    * **Ação 2 (`u`):** Revisar Entregas.
* **Ponto de Decisão (Avaliação):**
    * Caminho A: **Aprovar**.
    * Caminho B: **Solicitar Correção**.
* **Feedback (`d`):** Se houver correção, o sistema exige inserção de texto e devolve o fluxo ao aluno.

---

### 📝 6. Realização de Tarefas (Aluno)
![Foco](https://img.shields.io/badge/FOCO-ENTREGA-c38ae2?style=flat-square)

**Objetivo:** Acompanhar pendências e realizar submissões.

<div align="center">
  <img width="100%" src="./caminho/para/imagem_aluno.jpg" alt="MoLIC Tarefas">
</div>

* **Cena: Lista de Pendências**
    * Aluno visualiza prazos e status atual.
* **Cena: Detalhes da Tarefa**
    * Leitura de orientações.
    * Upload de arquivo (`u`).
* **Confirmação:**
    * `d`: Sistema confirma "Entrega realizada com sucesso" ou alerta erro de upload.

---

### 📄 7. Geração de Documentos
![Foco](https://img.shields.io/badge/FOCO-AUTOMAÇÃO-791297?style=flat-square)

**Objetivo:** Automatizar a criação de relatórios e requerimentos oficiais.

<div align="center">
  <img width="100%" src="./caminho/para/imagem_docs.jpg" alt="MoLIC Documentos">
</div>

* **Fluxo de Diálogo:**
    1.  **Configurar (`u`):** Seleciona modelo (Relatório/Requerimento).
    2.  **Processamento (`d`):** Sistema preenche cabeçalho e dados vinculados.
    3.  **Edição (`u`):** Usuário completa dados específicos.
    4.  **Prévia (`d`):** Exibição do documento gerado.
    5.  **Encerramento (`u`):** Download do arquivo final.

---
<div align="center">
<sub>Documentação de Modelagem de Interação • Atualizado em 2024</sub>
</div>
