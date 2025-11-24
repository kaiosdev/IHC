# Detalhamento Passo a Passo dos Fluxos do Sistema (HTA)

Abaixo apresentamos a descrição granular de cada Análise Hierárquica de Tarefas. Cada seção detalha as entradas, processamentos e saídas esperadas em cada nó do diagrama.

---

## 1. Realizar Login do Sistema
Este fluxo descreve a porta de entrada do usuário, focando em segurança e recuperação de erros.

<img width="1000" alt="Fluxograma de Login" src="https://github.com/user-attachments/assets/9ac6a613-ea20-4d8e-9480-c8864f958210" />

**Passo a Passo do Processo:**
1.  **Acesso Inicial (1):** O usuário abre o navegador/aplicativo (1.1) e navega até a página de login (1.2).
2.  **Inserção de Dados (2):**
    * O usuário insere seu e-mail institucional (2.2) e senha (2.3).
    * *Opcional:* O usuário pode marcar "Manter conectado" (2.4) para evitar logins repetitivos.
    * *Desvio:* Se o usuário esqueceu a senha, ele aciona o sub-fluxo de "Recuperar senha" (2.1).
3.  **Confirmação e Acesso (3):**
    * O usuário clica em "Entrar" (3.2).
    * O sistema valida as credenciais (2.1 - Aguardar validação).
    * Se válido, o sistema redireciona o usuário para o Dashboard principal (3.3).

---

## 2. Cadastrar Novo Projeto
Este fluxo demonstra a integração do sistema com bancos de dados externos para reduzir a burocracia.

<img width="1000" alt="Fluxograma de Cadastro de Projeto" src="https://github.com/user-attachments/assets/7d2435a4-c02c-4176-8607-0460c4ec0f38" />

**Passo a Passo do Processo:**
1.  **Início do Cadastro (1):** O professor acessa a área de projetos e seleciona a modalidade (ex: PIBIC, Extensão).
2.  **Automação (2):** O sistema conecta-se ao E-Campus e **importa automaticamente** os dados do professor e do departamento, eliminando preenchimento manual.
3.  **Detalhamento (3):** O usuário preenche apenas os dados específicos deste projeto (título, resumo, vigência).
4.  **Formação de Equipe (4):**
    * O professor busca o aluno pelo número de matrícula (4.1).
    * Ao encontrar, clica em "Adicionar" (4.2).
    * *Loop:* Este passo pode ser repetido várias vezes para adicionar múltiplos bolsistas.
5.  **Finalização (5):** O projeto é salvo e submetido para aprovação.

---

## 3. Consultar Feed Unificado de Editais
Focado na busca eficiente de informações, permitindo filtragem e ação rápida.

<img width="1000" alt="Fluxograma de Feed de Editais" src="https://github.com/user-attachments/assets/1dfaee82-b01c-4003-95fc-e924c3257df7" />

**Passo a Passo do Processo:**
1.  **Visualização Geral (1):** O usuário acessa o feed onde todos os editais abertos são listados cronologicamente.
2.  **Refinamento de Busca (2):**
    * O usuário aplica filtros por "Pró-Reitoria" (2.1) (ex: Pesquisa, Extensão) ou por "Status" (2.2) (ex: Aberto, Encerrado).
    * O sistema atualiza a lista em tempo real.
3.  **Interação com o Edital (3):**
    * **Ação Imediata:** O usuário clica em "Baixar PDF" (3.1) para ler o edital completo.
    * **Ação de Planejamento:** O usuário clica em "Favoritar" (3.2) para salvar o edital em sua lista pessoal para ler depois.

---

## 4. Gerenciar Tarefas do Orientando (Visão do Professor)
O fluxo de controle e feedback pedagógico entre orientador e aluno.

<img width="1000" alt="Fluxograma de Gestão de Orientandos" src="https://github.com/user-attachments/assets/d89d76f2-bfcc-453b-b908-56d150be5bb2" />

**Passo a Passo do Processo:**
1.  **Atribuição (1):** O orientador cria uma nova tarefa (1.1), define um prazo limite (1.2) e a envia para o aluno.
2.  **Análise (2):** Quando o aluno entrega, o professor recebe uma notificação, baixa o arquivo enviado (2.1) e analisa o conteúdo.
3.  **Decisão e Feedback (3):**
    * **Caminho A (Reprovação):** O professor clica em "Solicitar Correção" (3.1) e escreve um comentário obrigatório explicando o erro.
    * **Caminho B (Aprovação):** O professor clica em "Aprovar Tarefa" (3.2), e as horas são computadas no relatório do aluno.

---

## 5. Execução de Tarefas pelo Aluno (Visão do Discente)
O espelho do fluxo anterior, focado na organização pessoal do estudante.

<img width="1000" alt="Fluxograma de Execução de Tarefas" src="https://github.com/user-attachments/assets/df35a980-e780-411b-b21a-e1ffaa5282b2" />

**Passo a Passo do Processo:**
1.  **Consultar Pendências (1):**
    * O aluno acessa o painel de tarefas (1.1).
    * Verifica o status (Pendente/Atrasado) (1.2).
    * Confere o prazo final (1.3) para priorizar o trabalho.
2.  **Realizar Entrega (2):**
    * O aluno clica na tarefa e seleciona "Anexar Arquivo" (2.1).
    * Confirma o envio para o orientador (2.2).
3.  **Acompanhamento (3):** O aluno monitora o histórico para ver se a tarefa foi aprovada ou se retornou para correção.

---

## 6. Gerar Documentação Automática
Focado na eficiência administrativa, transformando dados do sistema em documentos oficiais.

<img width="1000" alt="Fluxograma de Documentação Automática" src="https://github.com/user-attachments/assets/c0c53118-668c-461d-8a56-222ba5a8b79b" />

**Passo a Passo do Processo:**
1.  **Acesso (1):** O usuário entra na área de "Secretaria Virtual" ou "Documentos".
2.  **Seleção (2):** Escolhe o tipo de documento desejado (ex: Relatório Parcial, Declaração de Vínculo).
3.  **Processamento Automático (3):**
    * O sistema busca os dados do projeto ativo (3.1).
    * O sistema preenche o cabeçalho, nomes e datas no modelo padrão (3.2).
4.  **Conclusão (4):**
    * O sistema gera uma prévia na tela (4.1) para conferência.
    * O usuário clica em "Download" (4.2) para baixar o arquivo finalizado e assinado digitalmente.

---

## 7. Acessar Opções de Acessibilidade Visual
Detalha como o sistema se adapta a usuários com baixa visão ou daltonismo.

<img width="1000" alt="Fluxograma de Acessibilidade Visual" src="https://github.com/user-attachments/assets/dec4d78e-03c9-4944-b7ad-1178081e5e08" />

**Passo a Passo do Processo:**
1.  **Configuração de Contraste (1):** O usuário pode alternar entre "Modo Escuro", "Alto Contraste" ou "Inversão de Cores" (1.1 e 1.2).
2.  **Ajuste Tipográfico (2):** O usuário utiliza controles deslizantes para aumentar o tamanho da fonte (2.1) ou alterar a fonte para uma tipografia amigável para dislexia (2.2).
3.  **Navegação Assistiva (3):**
    * O usuário ativa "Fluxos Lineares" (3.1).
    * O sistema reorganiza o layout, removendo colunas laterais e transformando o conteúdo em uma lista vertical única, ideal para leitores de tela e navegação por teclado.

---

## 8. Acessar Opções de Acessibilidade Cognitiva
Detalha recursos para usuários com TDAH, ansiedade ou dificuldades de concentração.

<img width="1000" alt="Fluxograma de Acessibilidade Cognitiva" src="https://github.com/user-attachments/assets/69f5fd51-07a2-472f-bc27-376ad1b11fac" />

**Passo a Passo do Processo:**
1.  **Orientação de Tarefa (1):**
    * Se o usuário se sentir perdido, clica em "O que fazer agora?".
    * O sistema destaca visualmente a "Próxima Ação" prioritária (1.2), ocultando opções secundárias.
2.  **Modo de Foco (2):**
    * O usuário ativa o "Modo Sem Distrações" (2.1).
    * O sistema remove banners, notificações não urgentes e elementos decorativos, mantendo apenas a tarefa central na tela.
