
<div align="center">

<h1>ANÁLISE HIERÁRQUICA DE TAREFAS (HTA)</h1>

<img src="https://img.shields.io/badge/Disciplina-IHC-791297?style=for-the-badge&logo=googlescholar&logoColor=white" alt="Disciplina IHC">
<img src="https://img.shields.io/badge/Artefato-Análise_de_Tarefas-c38ae2?style=for-the-badge&logo=googletasks&logoColor=white" alt="Análise de Tarefas">

<br><br>

> **Estrutura de Ação**
> <br>Decomposição sistemática dos objetivos dos usuários em subobjetivos, operações e planos de execução.

<a href="https://miro.com/app/board/uXjVJmtNoj8=/">
  <img src="https://img.shields.io/badge/ACESSAR_DIAGRAMAS_NO_MIRO_➔-791297?style=for-the-badge&logoColor=white" alt="Acessar Miro">
</a> 

</div>

---

## 1. Visão Geral dos Fluxos

<div align="center">
  
Abaixo apresentamos a descrição granular de cada Análise Hierárquica de Tarefas. Cada seção detalha as entradas, processamentos e saídas esperadas em cada nó do diagrama, divididos entre **Tarefas Essenciais** e **Tarefas de Acessibilidade**.

  <img src="https://drive.google.com/uc?export=view&id=19CSfmVbT589rpJxJybBW_UDqX5XHq7O8" width="90%">

</div>

---

## 2. Fluxos Essenciais do Sistema

### 🔐 1. Realizar Login do Sistema
![Perfil](https://img.shields.io/badge/PERFIL-TODOS_OS_USUÁRIOS-791297?style=flat-square)

Este fluxo descreve a porta de entrada do usuário, com foco em segurança e mecanismos de recuperação de erros.

<div align="center">
  <img width="100%" alt="Fluxograma de Login" src="https://github.com/user-attachments/assets/9ac6a613-ea20-4d8e-9480-c8864f958210" />
</div>

**Passo a Passo do Processo:**
1.  **Acesso Inicial:** O usuário abre o navegador/aplicativo e navega até a página de login.
2.  **Inserção de Dados:**
    * Usuário insere e-mail institucional e senha.
    * *(Opcional)* Marca "Manter conectado" para evitar logins repetitivos.
    * *(Desvio)* Se esqueceu a senha, aciona o sub-fluxo de "Recuperar senha".
3.  **Confirmação e Acesso:**
    * Usuário clica em "Entrar".
    * Sistema valida as credenciais.
    * **Resultado:** Redirecionamento para o Dashboard principal.

---

### 📂 2. Cadastrar Novo Projeto
![Perfil](https://img.shields.io/badge/PERFIL-ORIENTADOR-791297?style=flat-square)

Fluxo que demonstra a integração com bancos de dados externos (E-Campus) para reduzir a burocracia no preenchimento.

<div align="center">
  <img width="100%" alt="Fluxograma de Cadastro de Projeto" src="https://github.com/user-attachments/assets/7d2435a4-c02c-4176-8607-0460c4ec0f38" />
</div>

**Passo a Passo do Processo:**
1.  **Início do Cadastro:** O professor acessa a área de projetos e seleciona a modalidade (ex: PIBIC, Extensão).
2.  **Automação:** O sistema conecta-se ao E-Campus e **importa automaticamente** dados do professor/departamento.
3.  **Detalhamento:** Preenchimento apenas dos dados específicos (título, resumo, vigência).
4.  **Formação de Equipe:**
    * Busca do aluno por matrícula.
    * Adição do bolsista ao projeto (loop para múltiplos alunos).
5.  **Finalização:** Projeto salvo e submetido para aprovação.

---

### 📢 3. Consultar Feed Unificado de Editais
![Perfil](https://img.shields.io/badge/PERFIL-TODOS_OS_USUÁRIOS-c38ae2?style=flat-square)

Focado na busca eficiente de informações, permitindo filtragem e tomada de decisão rápida.

<div align="center">
  <img width="100%" alt="Fluxograma de Feed de Editais" src="https://github.com/user-attachments/assets/1dfaee82-b01c-4003-95fc-e924c3257df7" />
</div>

**Passo a Passo do Processo:**
1.  **Visualização Geral:** Acesso ao feed cronológico de editais abertos.
2.  **Refinamento de Busca:**
    * Aplicação de filtros por "Pró-Reitoria" (Pesquisa, Extensão) ou "Status".
    * Atualização da lista em tempo real.
3.  **Interação:**
    * **Ação Imediata:** "Baixar PDF" para leitura completa.
    * **Planejamento:** "Favoritar" para ler depois.

---

### 📝 4. Gerenciar Tarefas (Visão do Orientador)
![Perfil](https://img.shields.io/badge/PERFIL-ORIENTADOR-791297?style=flat-square)

O fluxo de controle pedagógico, atribuição de demandas e feedback.

<div align="center">
  <img width="100%" alt="Fluxograma de Gestão de Orientandos" src="https://github.com/user-attachments/assets/d89d76f2-bfcc-453b-b908-56d150be5bb2" />
</div>

**Passo a Passo do Processo:**
1.  **Atribuição:** Criação de nova tarefa, definição de prazo e envio ao aluno.
2.  **Análise:** Recebimento de notificação de entrega, download e análise do arquivo.
3.  **Decisão e Feedback:**
    * 🔴 **Reprovação:** Clica em "Solicitar Correção" e insere comentário obrigatório.
    * 🟢 **Aprovação:** Clica em "Aprovar Tarefa" e computa as horas.

---

### 📤 5. Execução de Tarefas (Visão do Aluno)
![Perfil](https://img.shields.io/badge/PERFIL-ALUNO_ORIENTADO-c38ae2?style=flat-square)

O espelho do fluxo anterior, focado na organização pessoal e cumprimento de prazos.

<div align="center">
  <img width="100%" alt="Fluxograma de Execução de Tarefas" src="https://github.com/user-attachments/assets/df35a980-e780-411b-b21a-e1ffaa5282b2" />
</div>

**Passo a Passo do Processo:**
1.  **Consultar Pendências:**
    * Acesso ao painel e verificação de status/prazos.
2.  **Realizar Entrega:**
    * Seleção da tarefa e upload de arquivo ("Anexar").
    * Confirmação de envio.
3.  **Acompanhamento:** Monitoramento do histórico (Aprovado ou Correção necessária).

---

### 📄 6. Gerar Documentação Automática
![Perfil](https://img.shields.io/badge/PERFIL-AMBOS-791297?style=flat-square)

Eficiência administrativa: transformando dados do sistema em documentos oficiais.

<div align="center">
  <img width="100%" alt="Fluxograma de Documentação Automática" src="https://github.com/user-attachments/assets/c0c53118-668c-461d-8a56-222ba5a8b79b" />
</div>

**Passo a Passo do Processo:**
1.  **Acesso:** Entrada na "Secretaria Virtual" ou área de "Documentos".
2.  **Seleção:** Escolha do tipo (ex: Relatório Parcial, Declaração).
3.  **Processamento Automático:** Sistema busca dados do projeto e preenche o modelo padrão.
4.  **Conclusão:** Visualização da prévia e Download do arquivo assinado.

---

## 3. Fluxos de Acessibilidade

### 👁️ 7. Acessibilidade Visual (PAV)
![Perfil](https://img.shields.io/badge/MODO-ACESSIBILIDADE_VISUAL-791297?style=flat-square)

Adaptação do sistema para usuários com baixa visão, daltonismo ou presbiopia.

<div align="center">
  <img width="100%" alt="Fluxograma de Acessibilidade Visual" src="https://github.com/user-attachments/assets/dec4d78e-03c9-4944-b7ad-1178081e5e08" />
</div>

**Passo a Passo do Processo:**
1.  **Configuração de Contraste:** Alternância entre Modo Escuro, Alto Contraste ou Inversão.
2.  **Ajuste Tipográfico:** Controle deslizante para tamanho de fonte e tipografia para dislexia.
3.  **Navegação Assistiva:**
    * Ativação de "Fluxos Lineares".
    * Reorganização do layout (lista vertical única) para leitores de tela.

---

### 🧠 8. Acessibilidade Cognitiva (AAC)
![Perfil](https://img.shields.io/badge/MODO-ACESSIBILIDADE_COGNITIVA-c38ae2?style=flat-square)

Recursos para usuários com TDAH, ansiedade ou dificuldades de concentração.

<div align="center">
  <img width="100%" alt="Fluxograma de Acessibilidade Cognitiva" src="https://github.com/user-attachments/assets/69f5fd51-07a2-472f-bc27-376ad1b11fac" />
</div>

**Passo a Passo do Processo:**
1.  **Orientação de Tarefa:**
    * Acionamento do botão "O que fazer agora?".
    * Destaque visual na Próxima Ação prioritária.
2.  **Modo de Foco:**
    * Ativação do "Modo Sem Distrações".
    * Remoção de banners e elementos decorativos, mantendo apenas o foco central.

---
<div align="center">
<sub>Documentação de Análise de Tarefas • Atualizado em 2025</sub>
</div>
