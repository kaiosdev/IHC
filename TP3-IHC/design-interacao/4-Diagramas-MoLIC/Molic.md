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

O sistema E-Project possui **4 fluxos principais** baseados nas personas:

1. **Fluxo do Orientador (O)** - Gestão de Tarefas e Projetos
2. **Fluxo do Aluno Orientado (AO)** - Execução e Entrega de Tarefas
3. **Fluxo de Acessibilidade Visual (PAV)** - Configurações de Visibilidade
4. **Fluxo de Acessibilidade Cognitiva (AAC)** - Recursos de Foco e Organização

---

##  Diagrama MoLIC Geral

> **Visualização completa do sistema mostrando todos os fluxos integrados**

![Diagrama MoLIC Geral](https://drive.google.com/uc?export=view&id=1xXgckQfj9p9489SyBuRJUnmdrkvxfNKs)

*Diagrama MoLIC Geral - Visão completa dos fluxos de interação do E-Project*

### Descrição Geral

O diagrama apresenta a arquitetura conversacional completa do sistema, onde:

- **Ponto de Entrada**: Login/Autenticação (cena inicial comum a todos)
- **Bifurcação por Perfil**: Após autenticação, o sistema direciona para o dashboard específico
- **Fluxos Paralelos**: Cada persona tem seu próprio caminho de navegação
- **Pontos de Convergência**: Configurações de acessibilidade podem ser acessadas de qualquer fluxo
- **Saídas**: Logout e conclusão de tarefas como pontos finais

---

##  Zoom 1: Fluxo de Autenticação e Entrada

![Cena de Login e Seleção de Perfil](https://drive.google.com/uc?export=view&id=ZOOM1_ID)

*Cena de Login e Seleção de Perfil*

### Cenas e Transições

#### **Cena 1: Tela de Login**

**Fala do Designer:**
> "Bem-vindo ao E-Project. Para começar, preciso que você se identifique com seu e-mail institucional e senha."

**Falas do Usuário (ações possíveis):**
- "Vou inserir meu e-mail e senha" → transição para validação
- "Esqueci minha senha" → transição para recuperação
- "Preciso criar uma conta" → transição para cadastro

**Processamento:**
- Sistema valida credenciais no banco de dados
- Verifica tipo de perfil (Orientador/Aluno/Coordenador)

#### **Ponto de Decisão 1: Autenticação**

**Condições:**
-  **Credenciais válidas** → transição para Dashboard correspondente
-  **Credenciais inválidas** → ruptura: "Usuário ou senha incorretos"
-  **Conta bloqueada** → ruptura: "Entre em contato com suporte"

#### **Cena 2: Dashboard Personalizado**

**Fala do Designer:**
- Para Orientador: "Aqui estão seus projetos ativos e tarefas pendentes dos orientandos"
- Para Aluno: "Estas são suas tarefas pendentes e próximos prazos"
- Para Coordenador: "Visão geral dos cursos e projetos sob sua coordenação"

---

## Zoom 2: Fluxo do Orientador - Criação de Tarefa

![Sequência de criação e atribuição de tarefa pelo orientador](https://drive.google.com/uc?export=view&id=ZOOM2_ID)

*Sequência de criação e atribuição de tarefa pelo orientador*

### Cenas e Transições

#### **Cena 3: Painel de Gerenciamento de Tarefas**

**Fala do Designer:**
> "Você pode criar uma nova tarefa, visualizar tarefas pendentes ou revisar entregas dos seus orientandos."

**Falas do Usuário:**
- "Quero criar uma nova tarefa" → transição para formulário
- "Quero ver entregas recentes" → transição para lista de revisão
- "Preciso acompanhar um projeto específico" → transição para detalhes do projeto

#### **Cena 4: Formulário de Nova Tarefa**

**Fala do Designer:**
> "Preencha os detalhes da tarefa: título, descrição, prazo e selecione o orientando responsável."

**Falas do Usuário:**
- "Preencho todos os campos obrigatórios" → habilita botão de envio
- "Quero anexar um arquivo de referência" → abre seletor de arquivos
- "Preciso definir uma data de entrega" → abre calendário

**Processamento:**
- Validação de campos obrigatórios em tempo real
- Formatação automática de datas

#### **Transição: Confirmação de Envio**

**Fala do Designer:**
> "Tarefa criada com sucesso! O orientando receberá uma notificação."

**Feedback Visual:**
-  Card verde com mensagem de confirmação
-  Indicador de notificação enviada
- ↩ Botão para voltar ao painel

#### **Ruptura Possível:**
-  **Campos obrigatórios vazios**: "Por favor, preencha todos os campos marcados com *"
-  **Data inválida**: "A data de entrega deve ser futura"
-  **Falha no envio**: "Erro ao criar tarefa. Tente novamente."

---

##  Zoom 3: Fluxo do Aluno - Visualização e Entrega de Tarefa

![Sequência de visualização, execução e submissão de tarefa pelo aluno](https://drive.google.com/uc?export=view&id=ZOOM3_ID)

*Sequência de visualização, execução e submissão de tarefa pelo aluno*

### Cenas e Transições

#### **Cena 5: Lista de Tarefas Pendentes**

**Fala do Designer:**
> "Você tem [N] tarefas pendentes. As mais urgentes estão destacadas em vermelho."

**Organização Visual:**
- 🔴 Tarefas urgentes (prazo < 3 dias)
- 🟡 Tarefas próximas (prazo 3-7 dias)
- 🟢 Tarefas no prazo (prazo > 7 dias)

**Falas do Usuário:**
- "Vou abrir esta tarefa" → transição para detalhes
- "Quero filtrar por projeto" → aplica filtro na lista
- "Preciso ver meu histórico" → transição para tarefas concluídas

#### **Cena 6: Detalhes da Tarefa**

**Fala do Designer:**
> "Esta tarefa foi enviada por [Nome do Orientador] em [Data]. Prazo: [Data de entrega]."

**Informações Exibidas:**
-  Título e descrição completa
-  Arquivos de referência (se houver)
-  Contador regressivo até o prazo
- Checklist de requisitos (para AAC)

**Falas do Usuário:**
- "Vou fazer upload do meu arquivo" → transição para submissão
- "Preciso de mais informações" → abre chat/comentários
- "Não consigo fazer esta tarefa" → opção de solicitar ajuda

#### **Cena 7: Submissão de Arquivo**

**Fala do Designer:**
> "Arraste seu arquivo aqui ou clique para selecionar. Formatos aceitos: PDF, DOC, DOCX, ZIP."

**Processamento:**
- Validação de formato de arquivo
- Upload com barra de progresso
- Geração de hash para verificação de integridade

**Feedback:**
-  "Enviando... 45%"
-  "Arquivo enviado com sucesso!"
-  "Tamanho: 2.3 MB | Enviado em: [hora]"

#### **Ponto de Decisão 2: Validação de Upload**

**Condições:**
-  **Upload bem-sucedido** → cena de confirmação
-  **Formato inválido** → ruptura: "Este formato não é aceito"
-  **Arquivo muito grande** → ruptura: "Limite de 10 MB excedido"
-  **Falha na conexão** → ruptura: "Erro de rede. Tente novamente"

#### **Cena 8: Confirmação de Entrega**

**Fala do Designer:**
> "Sua entrega foi registrada! O orientador receberá uma notificação para revisão."

**Ações Disponíveis:**
- ↩ Voltar para lista de tarefas
-  Ver comprovante de entrega
-  Enviar arquivo adicional (se permitido)

---

##  Zoom 4: Fluxo de Acessibilidade Visual

![Configurações de acessibilidade para usuários com baixa visão](https://drive.google.com/uc?export=view&id=ZOOM4_ID)

*Configurações de acessibilidade para usuários com baixa visão*

### Cenas e Transições

#### **Cena 9: Painel de Configurações de Acessibilidade**

**Fala do Designer:**
> "Ajuste a interface para melhor atender suas necessidades visuais. Todas as configurações são salvas automaticamente."

**Opções Disponíveis:**

1. **Tamanho da Fonte**
   -  Pequeno (14px)
   -  Médio (16px - padrão)
   -  Grande (20px)
   -  Muito Grande (24px)

2. **Contraste**
   -  Padrão
   -  Alto Contraste (fundo escuro)
   -  Contraste Máximo (preto e branco)

3. **Espaçamento**
   - 📏 Compacto
   - 📏 Normal
   - 📏 Amplo (recomendado para baixa visão)

**Falas do Usuário:**
- "Vou aumentar a fonte para 20px" → aplica mudança em tempo real
- "Preciso de mais contraste" → ativa modo alto contraste
- "Quero testar as configurações" → preview em tela separada

**Processamento:**
- Aplicação instantânea das mudanças (sem reload)
- Persistência no localStorage
- Sincronização com perfil do usuário

#### **Preview em Tempo Real**

**Fala do Designer:**
> "Veja como a interface fica com suas configurações. Se não gostar, é só ajustar novamente."

**Feedback Visual:**
- Antes ↔️ Depois (comparação lado a lado)
- Demonstração em diferentes telas do sistema
- Opção de resetar para padrão

---

## 🔍 Zoom 5: Fluxo de Acessibilidade Cognitiva

![Recursos para usuários com TDAH e Dislexia](https://drive.google.com/uc?export=view&id=ZOOM5_ID)

*Recursos para usuários com TDAH e Dislexia*

### Cenas e Transições

#### **Cena 10: Modo Foco**

**Fala do Designer:**
> "Ative o Modo Foco para esconder distrações e concentrar-se apenas na tarefa atual."

**Transformações Visuais:**
- 🚫 Remove menu lateral
- 🚫 Esconde notificações
- 🚫 Desativa animações
- ✅ Destaca apenas a tarefa em foco
- ⏱️ Timer Pomodoro opcional (25min trabalho / 5min pausa)

**Falas do Usuário:**
- "Quero ativar o modo foco" → tela minimalista
- "Preciso de um timer" → configura Pomodoro
- "Quero voltar ao normal" → desativa modo foco

#### **Cena 11: Checklist Visual da Tarefa**

**Fala do Designer:**
> "Siga estes passos para completar a tarefa. Marque cada item conforme avançar."

**Elementos Visuais:**
- ✅ Passo concluído (verde)
- 🔵 Passo atual (azul pulsante)
- ⚪ Passo pendente (cinza)

**Exemplo de Checklist:**
```
✅ 1. Ler as instruções da tarefa
🔵 2. Baixar arquivos de referência
⚪ 3. Produzir o conteúdo solicitado
⚪ 4. Revisar o trabalho
⚪ 5. Fazer upload do arquivo
⚪ 6. Confirmar entrega
```

**Falas do Usuário:**
- "Marquei este passo como concluído" → avança barra de progresso
- "Preciso voltar ao passo anterior" → permite navegação livre
- "Não entendi este passo" → abre ajuda contextual

#### **Feedback Progressivo**

**Fala do Designer:**
- 25%: "Você está indo bem! Continue assim."
- 50%: "Metade do caminho! Falta pouco."
- 75%: "Quase lá! Mais um esforço."
- 100%: "🎉 Parabéns! Você completou todos os passos!"

---

## 🔍 Zoom 6: Fluxo de Revisão pelo Orientador

![Análise e feedback sobre entregas dos alunos](https://drive.google.com/uc?export=view&id=ZOOM6_ID)

*Análise e feedback sobre entregas dos alunos*

### Cenas e Transições

#### **Cena 12: Fila de Revisão**

**Fala do Designer:**
> "Você tem [N] entregas aguardando revisão. As mais antigas estão destacadas."

**Organização:**
- 🔴 Entregas com > 7 dias sem revisão
- 🟡 Entregas com 3-7 dias
- 🟢 Entregas recentes (< 3 dias)

**Informações por Card:**
- 👤 Nome do aluno
- 📋 Título da tarefa
- 📅 Data de entrega
- 📎 Tipo de arquivo enviado

**Falas do Usuário:**
- "Vou revisar esta entrega" → abre visualizador
- "Quero filtrar por projeto" → aplica filtro
- "Preciso priorizar as mais antigas" → ordena por data

#### **Cena 13: Visualizador de Entrega**

**Fala do Designer:**
> "Arquivo enviado por [Aluno] em [Data]. Você pode visualizar, baixar ou abrir em nova aba."

**Ferramentas Disponíveis:**
- 📄 Preview do documento (se possível)
- ⬇️ Download do arquivo
- 🖊️ Adicionar comentários
- ✅ Aprovar
- ❌ Solicitar correções

**Falas do Usuário:**
- "Vou adicionar um comentário" → abre editor de texto
- "Esta entrega está aprovada" → transição para aprovação
- "Precisa de correções" → transição para feedback

#### **Ponto de Decisão 3: Avaliação**

**Condições:**

**✅ Aprovação:**
- Sistema marca tarefa como concluída
- Aluno recebe notificação de aprovação
- Registro fica no histórico

**❌ Solicitar Correções:**
- Abre formulário de feedback
- Tarefa volta para "Pendente" do aluno
- Aluno recebe notificação com comentários

#### **Cena 14: Formulário de Feedback**

**Fala do Designer:**
> "Explique o que precisa ser corrigido. Seja específico para ajudar o aluno a entender."

**Campos:**
- 📝 Comentários gerais
- 🎯 Pontos específicos a corrigir
- 📅 Nova data de entrega (opcional)
- 📎 Anexar arquivo de referência (opcional)

**Falas do Usuário:**
- "Envio o feedback" → aluno é notificado
- "Quero cancelar" → retorna sem salvar
- "Preciso anexar um exemplo" → upload de arquivo

---

## 📊 Tabela Resumo das Cenas e Transições

| Cena | Papel | Objetivo | Transições Principais |
|------|-------|----------|----------------------|
| 1. Login | Todos | Autenticar usuário | Dashboard Orientador / Aluno |
| 2. Dashboard | Todos | Visão geral | Tarefas / Projetos / Configurações |
| 3. Painel Tarefas | Orientador | Gerenciar demandas | Criar Tarefa / Revisar Entregas |
| 4. Formulário Tarefa | Orientador | Criar demanda | Confirmação / Cancelar |
| 5. Lista Pendentes | Aluno | Ver obrigações | Detalhes Tarefa / Histórico |
| 6. Detalhes Tarefa | Aluno | Entender requisitos | Submissão / Comentários |
| 7. Submissão | Aluno | Enviar arquivo | Confirmação / Erro |
| 8. Confirmação | Aluno | Feedback de sucesso | Voltar / Ver Comprovante |
| 9. Config. Visual | PAV | Ajustar interface | Preview / Salvar |
| 10. Modo Foco | AAC | Reduzir distração | Checklist / Desativar |
| 11. Checklist | AAC | Guiar execução | Próximo Passo / Ajuda |
| 12. Fila Revisão | Orientador | Organizar correções | Visualizador / Filtros |
| 13. Visualizador | Orientador | Analisar entrega | Aprovar / Solicitar Correção |
| 14. Feedback | Orientador | Comunicar ajustes | Enviar / Cancelar |

---

## 🔄 Rupturas de Comunicação Mapeadas

### Tipo 1: Rupturas Temporárias (Recuperáveis)

| Situação | Causa | Solução |
|----------|-------|---------|
| Campos obrigatórios vazios | Usuário tenta enviar formulário incompleto | Destaque em vermelho + mensagem específica |
| Formato de arquivo inválido | Usuário envia tipo não suportado | Mensagem de erro + lista de formatos aceitos |
| Falha de conexão | Instabilidade de rede | Botão "Tentar novamente" + salvamento local |
| Data inválida | Usuário seleciona data passada | Bloqueio no calendário + mensagem explicativa |

### Tipo 2: Rupturas Permanentes (Requerem Intervenção)

| Situação | Causa | Solução |
|----------|-------|---------|
| Conta bloqueada | Múltiplas tentativas de login | Contato com suporte técnico |
| Permissões insuficientes | Usuário tenta acessar área restrita | Redirecionamento + mensagem de acesso negado |
| Arquivo corrompido | Upload com erro de integridade | Solicitação de novo envio |
| Prazo expirado | Tentativa de entrega após deadline | Mensagem + opção de solicitar extensão |

---

## 🎨 Princípios de Design Aplicados

### 1. Visibilidade do Status do Sistema
- ✅ Feedback imediato para todas as ações
- ⏱️ Indicadores de progresso em uploads
- 🔔 Notificações claras e contextuais

### 2. Correspondência com o Mundo Real
- 📋 Linguagem acadêmica familiar (tarefa, orientador, entrega)
- 📅 Calendário visual para prazos
- 🎯 Cores semânticas (vermelho = urgente, verde = ok)

### 3. Controle e Liberdade do Usuário
- ↩️ Sempre há uma opção "Voltar"
- 💾 Salvamento automático de rascunhos
- ↶ Opção de desfazer ações críticas

### 4. Consistência e Padrões
- 🎨 Mesma paleta de cores em todo o sistema
- 📐 Botões e formulários padronizados
- 🔤 Tipografia uniforme (ajustável para PAV)

### 5. Prevenção de Erros
- 🚫 Validação em tempo real de formulários
- ⚠️ Confirmação para ações irreversíveis
- 💡 Tooltips explicativos em campos complexos

### 6. Reconhecimento em vez de Memorização
- 🔍 Busca e filtros visuais
- 📊 Dashboard com cards informativos
- ✅ Checklist para AAC

### 7. Flexibilidade e Eficiência
- ⌨️ Atalhos de teclado para usuários avançados
- 📱 Interface responsiva (mobile/desktop)
- 🎚️ Configurações personalizáveis

### 8. Design Estético e Minimalista
- 🧹 Interface limpa, sem elementos desnecessários
- 🎯 Foco na tarefa atual (Modo Foco para AAC)
- 🖼️ Espaço em branco adequado (PAV)

### 9. Ajuda aos Usuários para Reconhecer, Diagnosticar e Recuperar Erros
- ❌ Mensagens de erro claras e específicas
- 💡 Sugestões de correção
- 📚 Links para documentação contextual

### 10. Ajuda e Documentação
- ❓ Ícone de ajuda sempre visível
- 📖 Tutoriais contextuais
- 💬 Chat de suporte integrado

---

## 🔗 Relação com Artefatos Anteriores

### Com as Metamensagens:
- **Victor (Orientador)**: Cenas 3, 4, 12, 13, 14 implementam a visão de "centralização e eficiência"
- **Ana (Aluna)**: Cenas 5, 6, 7, 8 materializam o "medo de perder prazos" com feedback claro
- **Carlos (PAV)**: Cena 9 concretiza a "interface limpa e ajustável"
- **João (AAC)**: Cenas 10, 11 implementam o "foco e organização visual"

### Com os Mapas de Objetivos:
- Cada objetivo do mapa possui pelo menos uma cena correspondente
- Transições refletem a sequência natural dos objetivos
- Rupturas mapeadas antecipam obstáculos identificados nas personas

### Com os HTAs:
- Planos do HTA viram transições no MoLIC
- Operações atômicas viram falas do usuário
- Decisões binárias viram pontos de decisão

---

## 📝 Considerações Finais

Os diagramas MoLIC apresentados capturam a **essência conversacional** do sistema E-Project, onde:

1. **Cada interação é um diálogo** entre usuário e designer
2. **Rupturas são previstas e tratadas** com empatia
3. **Acessibilidade é nativa**, não um complemento
4. **Feedback é constante e claro**, reduzindo ansiedade
5. **Flexibilidade atende diferentes perfis** sem comprometer a simplicidade

Este modelo de interação será a base para os protótipos de alta fidelidade, garantindo que a implementação respeite a metacomunicação projetada e atenda às necessidades reais dos usuários acadêmicos da UFAM.

---

**Próxima etapa:** Sketches de baixa fidelidade baseados nestas cenas e transições.

---


1. **Fluxo do Orientador (O)** - Gestão de Tarefas e Projetos
2. **Fluxo do Aluno Orientado (AO)** - Execução e Entrega de Tarefas
3. **Fluxo de Acessibilidade Visual (PAV)** - Configurações de Visibilidade
4. **Fluxo de Acessibilidade Cognitiva (AAC)** - Recursos de Foco e Organização

---

##  Diagrama MoLIC Geral

> **Visualização completa do sistema mostrando todos os fluxos integrados**

![Diagrama MoLIC Geral](https://drive.google.com/uc?export=view&id=1xXgckQfj9p9489SyBuRJUnmdrkvxfNKs)

*Diagrama MoLIC Geral - Visão completa dos fluxos de interação do E-Project*

### Descrição Geral

O diagrama apresenta a arquitetura conversacional completa do sistema, onde:

- **Ponto de Entrada**: Login/Autenticação (cena inicial comum a todos)
- **Bifurcação por Perfil**: Após autenticação, o sistema direciona para o dashboard específico
- **Fluxos Paralelos**: Cada persona tem seu próprio caminho de navegação
- **Pontos de Convergência**: Configurações de acessibilidade podem ser acessadas de qualquer fluxo
- **Saídas**: Logout e conclusão de tarefas como pontos finais

---

##  Zoom 1: Fluxo de Autenticação e Entrada

![Cena de Login e Seleção de Perfil](https://drive.google.com/uc?export=view&id=ZOOM1_ID)

*Cena de Login e Seleção de Perfil*

### Cenas e Transições

#### **Cena 1: Tela de Login**

**Fala do Designer:**
> "Bem-vindo ao E-Project. Para começar, preciso que você se identifique com seu e-mail institucional e senha."

**Falas do Usuário (ações possíveis):**
- "Vou inserir meu e-mail e senha" → transição para validação
- "Esqueci minha senha" → transição para recuperação
- "Preciso criar uma conta" → transição para cadastro

**Processamento:**
- Sistema valida credenciais no banco de dados
- Verifica tipo de perfil (Orientador/Aluno/Coordenador)

#### **Ponto de Decisão 1: Autenticação**

**Condições:**
-  **Credenciais válidas** → transição para Dashboard correspondente
-  **Credenciais inválidas** → ruptura: "Usuário ou senha incorretos"
-  **Conta bloqueada** → ruptura: "Entre em contato com suporte"

#### **Cena 2: Dashboard Personalizado**

**Fala do Designer:**
- Para Orientador: "Aqui estão seus projetos ativos e tarefas pendentes dos orientandos"
- Para Aluno: "Estas são suas tarefas pendentes e próximos prazos"
- Para Coordenador: "Visão geral dos cursos e projetos sob sua coordenação"

---

## Zoom 2: Fluxo do Orientador - Criação de Tarefa

![Sequência de criação e atribuição de tarefa pelo orientador](https://drive.google.com/uc?export=view&id=ZOOM2_ID)

*Sequência de criação e atribuição de tarefa pelo orientador*

### Cenas e Transições

#### **Cena 3: Painel de Gerenciamento de Tarefas**

**Fala do Designer:**
> "Você pode criar uma nova tarefa, visualizar tarefas pendentes ou revisar entregas dos seus orientandos."

**Falas do Usuário:**
- "Quero criar uma nova tarefa" → transição para formulário
- "Quero ver entregas recentes" → transição para lista de revisão
- "Preciso acompanhar um projeto específico" → transição para detalhes do projeto

#### **Cena 4: Formulário de Nova Tarefa**

**Fala do Designer:**
> "Preencha os detalhes da tarefa: título, descrição, prazo e selecione o orientando responsável."

**Falas do Usuário:**
- "Preencho todos os campos obrigatórios" → habilita botão de envio
- "Quero anexar um arquivo de referência" → abre seletor de arquivos
- "Preciso definir uma data de entrega" → abre calendário

**Processamento:**
- Validação de campos obrigatórios em tempo real
- Formatação automática de datas

#### **Transição: Confirmação de Envio**

**Fala do Designer:**
> "Tarefa criada com sucesso! O orientando receberá uma notificação."

**Feedback Visual:**
-  Card verde com mensagem de confirmação
-  Indicador de notificação enviada
- ↩ Botão para voltar ao painel

#### **Ruptura Possível:**
-  **Campos obrigatórios vazios**: "Por favor, preencha todos os campos marcados com *"
-  **Data inválida**: "A data de entrega deve ser futura"
-  **Falha no envio**: "Erro ao criar tarefa. Tente novamente."

---

##  Zoom 3: Fluxo do Aluno - Visualização e Entrega de Tarefa

![Sequência de visualização, execução e submissão de tarefa pelo aluno](https://drive.google.com/uc?export=view&id=ZOOM3_ID)

*Sequência de visualização, execução e submissão de tarefa pelo aluno*

### Cenas e Transições

#### **Cena 5: Lista de Tarefas Pendentes**

**Fala do Designer:**
> "Você tem [N] tarefas pendentes. As mais urgentes estão destacadas em vermelho."

**Organização Visual:**
- 🔴 Tarefas urgentes (prazo < 3 dias)
- 🟡 Tarefas próximas (prazo 3-7 dias)
- 🟢 Tarefas no prazo (prazo > 7 dias)

**Falas do Usuário:**
- "Vou abrir esta tarefa" → transição para detalhes
- "Quero filtrar por projeto" → aplica filtro na lista
- "Preciso ver meu histórico" → transição para tarefas concluídas

#### **Cena 6: Detalhes da Tarefa**

**Fala do Designer:**
> "Esta tarefa foi enviada por [Nome do Orientador] em [Data]. Prazo: [Data de entrega]."

**Informações Exibidas:**
-  Título e descrição completa
-  Arquivos de referência (se houver)
-  Contador regressivo até o prazo
- Checklist de requisitos (para AAC)

**Falas do Usuário:**
- "Vou fazer upload do meu arquivo" → transição para submissão
- "Preciso de mais informações" → abre chat/comentários
- "Não consigo fazer esta tarefa" → opção de solicitar ajuda

#### **Cena 7: Submissão de Arquivo**

**Fala do Designer:**
> "Arraste seu arquivo aqui ou clique para selecionar. Formatos aceitos: PDF, DOC, DOCX, ZIP."

**Processamento:**
- Validação de formato de arquivo
- Upload com barra de progresso
- Geração de hash para verificação de integridade

**Feedback:**
-  "Enviando... 45%"
-  "Arquivo enviado com sucesso!"
-  "Tamanho: 2.3 MB | Enviado em: [hora]"

#### **Ponto de Decisão 2: Validação de Upload**

**Condições:**
-  **Upload bem-sucedido** → cena de confirmação
-  **Formato inválido** → ruptura: "Este formato não é aceito"
-  **Arquivo muito grande** → ruptura: "Limite de 10 MB excedido"
-  **Falha na conexão** → ruptura: "Erro de rede. Tente novamente"

#### **Cena 8: Confirmação de Entrega**

**Fala do Designer:**
> "Sua entrega foi registrada! O orientador receberá uma notificação para revisão."

**Ações Disponíveis:**
- ↩ Voltar para lista de tarefas
-  Ver comprovante de entrega
-  Enviar arquivo adicional (se permitido)

---

##  Zoom 4: Fluxo de Acessibilidade Visual

![Configurações de acessibilidade para usuários com baixa visão](https://drive.google.com/uc?export=view&id=ZOOM4_ID)

*Configurações de acessibilidade para usuários com baixa visão*

### Cenas e Transições

#### **Cena 9: Painel de Configurações de Acessibilidade**

**Fala do Designer:**
> "Ajuste a interface para melhor atender suas necessidades visuais. Todas as configurações são salvas automaticamente."

**Opções Disponíveis:**

1. **Tamanho da Fonte**
   -  Pequeno (14px)
   -  Médio (16px - padrão)
   -  Grande (20px)
   -  Muito Grande (24px)

2. **Contraste**
   -  Padrão
   -  Alto Contraste (fundo escuro)
   -  Contraste Máximo (preto e branco)

3. **Espaçamento**
   - 📏 Compacto
   - 📏 Normal
   - 📏 Amplo (recomendado para baixa visão)

**Falas do Usuário:**
- "Vou aumentar a fonte para 20px" → aplica mudança em tempo real
- "Preciso de mais contraste" → ativa modo alto contraste
- "Quero testar as configurações" → preview em tela separada

**Processamento:**
- Aplicação instantânea das mudanças (sem reload)
- Persistência no localStorage
- Sincronização com perfil do usuário

#### **Preview em Tempo Real**

**Fala do Designer:**
> "Veja como a interface fica com suas configurações. Se não gostar, é só ajustar novamente."

**Feedback Visual:**
- Antes ↔️ Depois (comparação lado a lado)
- Demonstração em diferentes telas do sistema
- Opção de resetar para padrão

---

## 🔍 Zoom 5: Fluxo de Acessibilidade Cognitiva

![Recursos para usuários com TDAH e Dislexia](https://drive.google.com/uc?export=view&id=ZOOM5_ID)

*Recursos para usuários com TDAH e Dislexia*

### Cenas e Transições

#### **Cena 10: Modo Foco**

**Fala do Designer:**
> "Ative o Modo Foco para esconder distrações e concentrar-se apenas na tarefa atual."

**Transformações Visuais:**
- 🚫 Remove menu lateral
- 🚫 Esconde notificações
- 🚫 Desativa animações
- ✅ Destaca apenas a tarefa em foco
- ⏱️ Timer Pomodoro opcional (25min trabalho / 5min pausa)

**Falas do Usuário:**
- "Quero ativar o modo foco" → tela minimalista
- "Preciso de um timer" → configura Pomodoro
- "Quero voltar ao normal" → desativa modo foco

#### **Cena 11: Checklist Visual da Tarefa**

**Fala do Designer:**
> "Siga estes passos para completar a tarefa. Marque cada item conforme avançar."

**Elementos Visuais:**
- ✅ Passo concluído (verde)
- 🔵 Passo atual (azul pulsante)
- ⚪ Passo pendente (cinza)

**Exemplo de Checklist:**
```
✅ 1. Ler as instruções da tarefa
🔵 2. Baixar arquivos de referência
⚪ 3. Produzir o conteúdo solicitado
⚪ 4. Revisar o trabalho
⚪ 5. Fazer upload do arquivo
⚪ 6. Confirmar entrega
```

**Falas do Usuário:**
- "Marquei este passo como concluído" → avança barra de progresso
- "Preciso voltar ao passo anterior" → permite navegação livre
- "Não entendi este passo" → abre ajuda contextual

#### **Feedback Progressivo**

**Fala do Designer:**
- 25%: "Você está indo bem! Continue assim."
- 50%: "Metade do caminho! Falta pouco."
- 75%: "Quase lá! Mais um esforço."
- 100%: "🎉 Parabéns! Você completou todos os passos!"

---

## 🔍 Zoom 6: Fluxo de Revisão pelo Orientador

![Análise e feedback sobre entregas dos alunos](https://drive.google.com/uc?export=view&id=ZOOM6_ID)

*Análise e feedback sobre entregas dos alunos*

### Cenas e Transições

#### **Cena 12: Fila de Revisão**

**Fala do Designer:**
> "Você tem [N] entregas aguardando revisão. As mais antigas estão destacadas."

**Organização:**
- 🔴 Entregas com > 7 dias sem revisão
- 🟡 Entregas com 3-7 dias
- 🟢 Entregas recentes (< 3 dias)

**Informações por Card:**
- 👤 Nome do aluno
- 📋 Título da tarefa
- 📅 Data de entrega
- 📎 Tipo de arquivo enviado

**Falas do Usuário:**
- "Vou revisar esta entrega" → abre visualizador
- "Quero filtrar por projeto" → aplica filtro
- "Preciso priorizar as mais antigas" → ordena por data

#### **Cena 13: Visualizador de Entrega**

**Fala do Designer:**
> "Arquivo enviado por [Aluno] em [Data]. Você pode visualizar, baixar ou abrir em nova aba."

**Ferramentas Disponíveis:**
-  Preview do documento (se possível)
-  Download do arquivo
-  Adicionar comentários
-  Aprovar
-  Solicitar correções

**Falas do Usuário:**
- "Vou adicionar um comentário" → abre editor de texto
- "Esta entrega está aprovada" → transição para aprovação
- "Precisa de correções" → transição para feedback

#### **Ponto de Decisão 3: Avaliação**

**Condições:**

** Aprovação:**
- Sistema marca tarefa como concluída
- Aluno recebe notificação de aprovação
- Registro fica no histórico

** Solicitar Correções:**
- Abre formulário de feedback
- Tarefa volta para "Pendente" do aluno
- Aluno recebe notificação com comentários

#### **Cena 14: Formulário de Feedback**

**Fala do Designer:**
> "Explique o que precisa ser corrigido. Seja específico para ajudar o aluno a entender."

**Campos:**
-  Comentários gerais
-  Pontos específicos a corrigir
-  Nova data de entrega (opcional)
-  Anexar arquivo de referência (opcional)

**Falas do Usuário:**
- "Envio o feedback" → aluno é notificado
- "Quero cancelar" → retorna sem salvar
- "Preciso anexar um exemplo" → upload de arquivo

---

##  Tabela Resumo das Cenas e Transições

| Cena | Papel | Objetivo | Transições Principais |
|------|-------|----------|----------------------|
| 1. Login | Todos | Autenticar usuário | Dashboard Orientador / Aluno |
| 2. Dashboard | Todos | Visão geral | Tarefas / Projetos / Configurações |
| 3. Painel Tarefas | Orientador | Gerenciar demandas | Criar Tarefa / Revisar Entregas |
| 4. Formulário Tarefa | Orientador | Criar demanda | Confirmação / Cancelar |
| 5. Lista Pendentes | Aluno | Ver obrigações | Detalhes Tarefa / Histórico |
| 6. Detalhes Tarefa | Aluno | Entender requisitos | Submissão / Comentários |
| 7. Submissão | Aluno | Enviar arquivo | Confirmação / Erro |
| 8. Confirmação | Aluno | Feedback de sucesso | Voltar / Ver Comprovante |
| 9. Config. Visual | PAV | Ajustar interface | Preview / Salvar |
| 10. Modo Foco | AAC | Reduzir distração | Checklist / Desativar |
| 11. Checklist | AAC | Guiar execução | Próximo Passo / Ajuda |
| 12. Fila Revisão | Orientador | Organizar correções | Visualizador / Filtros |
| 13. Visualizador | Orientador | Analisar entrega | Aprovar / Solicitar Correção |
| 14. Feedback | Orientador | Comunicar ajustes | Enviar / Cancelar |

---

##  Rupturas de Comunicação Mapeadas

### Tipo 1: Rupturas Temporárias (Recuperáveis)

| Situação | Causa | Solução |
|----------|-------|---------|
| Campos obrigatórios vazios | Usuário tenta enviar formulário incompleto | Destaque em vermelho + mensagem específica |
| Formato de arquivo inválido | Usuário envia tipo não suportado | Mensagem de erro + lista de formatos aceitos |
| Falha de conexão | Instabilidade de rede | Botão "Tentar novamente" + salvamento local |
| Data inválida | Usuário seleciona data passada | Bloqueio no calendário + mensagem explicativa |

### Tipo 2: Rupturas Permanentes (Requerem Intervenção)

| Situação | Causa | Solução |
|----------|-------|---------|
| Conta bloqueada | Múltiplas tentativas de login | Contato com suporte técnico |
| Permissões insuficientes | Usuário tenta acessar área restrita | Redirecionamento + mensagem de acesso negado |
| Arquivo corrompido | Upload com erro de integridade | Solicitação de novo envio |
| Prazo expirado | Tentativa de entrega após deadline | Mensagem + opção de solicitar extensão |

---

##  Princípios de Design Aplicados

### 1. Visibilidade do Status do Sistema
-  Feedback imediato para todas as ações
-  Indicadores de progresso em uploads
-  Notificações claras e contextuais

### 2. Correspondência com o Mundo Real
-  Linguagem acadêmica familiar (tarefa, orientador, entrega)
-  Calendário visual para prazos
-  Cores semânticas (vermelho = urgente, verde = ok)

### 3. Controle e Liberdade do Usuário
-  Sempre há uma opção "Voltar"
-  Salvamento automático de rascunhos
-  Opção de desfazer ações críticas

### 4. Consistência e Padrões
-  Mesma paleta de cores em todo o sistema
-  Botões e formulários padronizados
-  Tipografia uniforme (ajustável para PAV)

### 5. Prevenção de Erros
-  Validação em tempo real de formulários
-  Confirmação para ações irreversíveis
-  Tooltips explicativos em campos complexos

### 6. Reconhecimento em vez de Memorização
-  Busca e filtros visuais
-  Dashboard com cards informativos
-  Checklist para AAC

### 7. Flexibilidade e Eficiência
-  Atalhos de teclado para usuários avançados
-  Interface responsiva (mobile/desktop)
-  Configurações personalizáveis

### 8. Design Estético e Minimalista
-  Interface limpa, sem elementos desnecessários
-  Foco na tarefa atual (Modo Foco para AAC)
-  Espaço em branco adequado (PAV)

### 9. Ajuda aos Usuários para Reconhecer, Diagnosticar e Recuperar Erros
-  Mensagens de erro claras e específicas
-  Sugestões de correção
-  Links para documentação contextual

### 10. Ajuda e Documentação
-  Ícone de ajuda sempre visível
-  Tutoriais contextuais
-  Chat de suporte integrado

---

##  Relação com Artefatos Anteriores

### Com as Metamensagens:
- **Victor (Orientador)**: Cenas 3, 4, 12, 13, 14 implementam a visão de "centralização e eficiência"
- **Ana (Aluna)**: Cenas 5, 6, 7, 8 materializam o "medo de perder prazos" com feedback claro
- **Carlos (PAV)**: Cena 9 concretiza a "interface limpa e ajustável"
- **João (AAC)**: Cenas 10, 11 implementam o "foco e organização visual"

### Com os Mapas de Objetivos:
- Cada objetivo do mapa possui pelo menos uma cena correspondente
- Transições refletem a sequência natural dos objetivos
- Rupturas mapeadas antecipam obstáculos identificados nas personas

### Com os HTAs:
- Planos do HTA viram transições no MoLIC
- Operações atômicas viram falas do usuário
- Decisões binárias viram pontos de decisão

---

##  Considerações Finais

Os diagramas MoLIC apresentados capturam a **essência conversacional** do sistema E-Project, onde:

1. **Cada interação é um diálogo** entre usuário e designer
2. **Rupturas são previstas e tratadas** com empatia
3. **Acessibilidade é nativa**, não um complemento
4. **Feedback é constante e claro**, reduzindo ansiedade
5. **Flexibilidade atende diferentes perfis** sem comprometer a simplicidade

Este modelo de interação será a base para os protótipos de alta fidelidade, garantindo que a implementação respeite a metacomunicação projetada e atenda às necessidades reais dos usuários acadêmicos da UFAM.

---

**Próxima etapa:** Sketches de baixa fidelidade baseados nestas cenas e transições.

---

## 📌 Informações do Projeto

**Sistema:** E-Project - Sistema de Gestão Acadêmica UFAM  
**Disciplina:** Interação Humano-Computador  
**Docente:** Prof. Dr. Andrey Rodrigues  
**Curso:** Engenharia de Software  
**Universidade:** Universidade Federal do Amazonas (ICET)

### Equipe de Desenvolvimento

| Membro | Nome Completo |
|--------|---------------|
| A1 | Geovanna Beathryz |
| A2 | Gustavo Souza |
| A3 | Iasmim Braga |
| A4 | Jean Barauna |
| A5 | Kaio Sobral |
| A6 | Pedro Jheivison |
