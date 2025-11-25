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

## 1. Introdução

Este documento descreve a modelagem da interação do **Sistema de Gestão de Projetos Acadêmicos** (focado em PIBIC/PACE), utilizando a notação **MoLIC** (Modeling Language for Interaction as Conversation).

O objetivo destes diagramas é mapear os diálogos entre o usuário e o sistema, prevendo fluxos de sucesso, tratamento de erros e personalização da interface.

### Legenda da Notação

A linguagem MoLIC baseia-se na Engenharia Semiótica para tratar a interação como comunicação.

| Elemento | Descrição |
| :--- | :--- |
| **u** | Ação ou fala do Usuário. |
| **d** | Ação, resposta ou fala do Designer (representado pelo sistema). |
| **Cena** | Retângulos arredondados representando momentos da interação. |
| **Caixas Internas** | Detalhes da interface ou opções disponíveis naquela cena. |
| **XOR** | Escolha exclusiva (o usuário faz um ou outro). |
| **Transição** | Setas que mostram a navegação entre cenas. |
| **Quadrado Preto** | Processamento interno do sistema ou Ponto de Decisão (chaves de verificação). |

---

## 2. Visão Geral do Sistema
![Foco](https://img.shields.io/badge/FOCO-ARQUITETURA_GERAL-791297?style=flat-square)

Visão panorâmica de todos os fluxos integrados, partindo do acesso inicial até as funcionalidades específicas.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1k4F1MjxjJWCa3nOR0ii8fFybJ7_Ynni8" width="70%">
   
<sub><b>Figura 1:</b> Visão geral da arquitetura de interação do sistema E-Project (Fonte: Autores, 2025).</sub>
</div>

---

## 3. Autenticação e Acesso
![Foco](https://img.shields.io/badge/FOCO-SEGURANÇA-c38ae2?style=flat-square)

**Objetivo:** Garantir o acesso seguro ao sistema.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=18ZkqWvfXm4490QJeAUXg2g-vhsyCwgVH" width="70%">
   
<sub><b>Figura 2:</b> Diagrama MoLIC do fluxo de Autenticação e acesso ao Dashboard (Fonte: Autores, 2025).</sub>
</div>

* **Fluxo Principal:** O usuário inicia a entrada no sistema.
* **Interação:**
    * `u`: Informa credenciais (matrícula/e-mail e senha).
    * `d`: Verifica as credenciais.
* **Desvios:**
    * Se inválido: O sistema retorna feedback de "login inválido" e permite nova tentativa.
    * Se válido: O sistema direciona o usuário para o **Dashboard**.

---

## 4. Personalização e Acessibilidade
![Foco](https://img.shields.io/badge/FOCO-ADAPTAÇÃO-791297?style=flat-square)

**Objetivo:** Permitir que o usuário adapte a interface às suas necessidades visuais e cognitivas.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1e9hRvLntzG2ntxyj9k666MWmT2JzsBWV" width="70%">
   
<sub><b>Figura 3:</b> Modelagem das opções de Personalização Visual e Suporte Cognitivo (Fonte: Autores, 2025).</sub>
</div>

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

## 5. Gestão de Projetos 
![Foco](https://img.shields.io/badge/FOCO-INTEGRAÇÃO-c38ae2?style=flat-square)

**Objetivo:** Cadastro de novos projetos acadêmicos e integração com sistemas externos.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1IWku2rBv3U90VzIYqtbV09LdGox3fgnz" width="70%">
   
<sub><b>Figura 4:</b> Fluxo de Cadastro de Novo Projeto com integração ao E-Campus (Fonte: Autores, 2025).</sub>
</div>

* **Cena: Novo Projeto Acadêmico**
    * **Integração:** O sistema permite importar dados diretamente do *E-Campus*.
        * `d`: Exibe erro na integração se falhar ou carrega dados automaticamente se sucesso.
    * **Definições:** Seleção de modalidade (PIBIC/PACE).
    * **Equipe:** Busca e adição de alunos.
        * `d`: Feedback se matrícula não for encontrada ou vínculo realizado com sucesso.
    * **Finalização:** O sistema valida campos obrigatórios antes de ativar o projeto.

---

## 6. Exploração de Editais 
![Foco](https://img.shields.io/badge/FOCO-INFORMAÇÃO-791297?style=flat-square)

**Objetivo:** Permitir que o usuário encontre oportunidades de bolsas e projetos.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1H4mO_BdIwTs7ukM4MSIM7pP9weK2H07R" width="70%">
   
<sub><b>Figura 5:</b> Fluxo de Exploração, filtragem e download de Editais (Fonte: Autores, 2025).</sub>
</div>

* **Interação:** O usuário consulta editais a partir do Dashboard.
* **Funcionalidades:**
    * Filtros por status ou pré-reitoria.
    * Download do edital (com tratamento de erro de conexão).
    * Opção de favoritar editais para acesso rápido.

---

## 7. Fluxo de Orientação 
![Foco](https://img.shields.io/badge/FOCO-FEEDBACK-c38ae2?style=flat-square)

**Objetivo:** Gerenciar as atividades dos orientandos e fornecer feedback.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1rFJsSivcnskxbUCupU7SMNPF_Jey-agF" width="70%">
   
<sub><b>Figura 6:</b> Fluxo do Orientador para gestão de atividades e feedback pedagógico (Fonte: Autores, 2025).</sub>
</div>

* **Cena: Gerenciar Atividades**
    * O orientador pode **Criar Nova Tarefa** (definindo título, prazo e anexos).
    * O orientador pode **Revisar Entregas**:
        * Visualiza a produção e histórico.
        * Decide entre **Aprovar** ou **Solicitar Correção**.
    * **Feedback:** Se solicitar correção, insere motivos/orientações que retornam ao aluno.

---

## 8. Realização de Tarefas
![Foco](https://img.shields.io/badge/FOCO-ENTREGA-791297?style=flat-square)

**Objetivo:** Acompanhar pendências e realizar entregas.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1_bawA8lx7HqWddv70ItoINkcywjODXWF" width="70%">
   
<sub><b>Figura 7:</b> Fluxo do Aluno para visualização de pendências e entrega de tarefas (Fonte: Autores, 2025).</sub>
</div>

* **Cena: Lista de Pendências**
    * O aluno visualiza prazos e status.
* **Cena: Detalhes da Tarefa**
    * Lê orientações.
    * Realiza o upload do arquivo (entrega).
    * `d`: Sistema confirma entrega ou alerta sobre erro no upload.

---

## 9. Geração de Documentos
![Foco](https://img.shields.io/badge/FOCO-AUTOMAÇÃO-c38ae2?style=flat-square)

**Objetivo:** Automatizar a criação de relatórios e requerimentos.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1Uxlbsnfh3MwiXkfnGDE7wjXCF-I_MjAB" width="70%">
   
<sub><b>Figura 8:</b> Fluxo de Geração Automática de Documentos e Relatórios (Fonte: Autores, 2025).</sub>
</div>

* **Fluxo:**
    1.  **Configurar Documento:** Seleciona modelo (Relatório de Atividades ou Requerimento).
    2.  **Dados:** O sistema preenche o cabeçalho vinculado automaticamente, usuário edita dados específicos.
    3.  **Pré-visualização:** O sistema exibe o documento gerado.
    4.  **Exportação:** Usuário baixa o arquivo final.

---
<div align="center">
<sub>Documentação de Design de Interação • Atualizado em 2025</sub>
</div>

