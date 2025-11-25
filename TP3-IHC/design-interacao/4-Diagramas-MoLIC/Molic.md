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
**Objetivo:** Garantir o acesso seguro ao sistema.

![Diagrama de Autenticação](./caminho/para/imagem_login.jpg)
*(Substitua pelo caminho real da imagem 1001307663.jpg)*

* **Fluxo Principal:** O usuário inicia a entrada no sistema.
* **Interação:**
    * `u`: Informa credenciais (matrícula/e-mail e senha).
    * `d`: Verifica as credenciais.
* **Desvios:**
    * Se inválido: O sistema retorna feedback de "login inválido" e permite nova tentativa.
    * Se válido: O sistema direciona o usuário para o **Dashboard**.

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
* Diagramação: nome da ferramenta, MoLIC da Tarefa**
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
<sub>Documentação de Modelagem de Interação • Atualizado em 2025</sub>
</div>
