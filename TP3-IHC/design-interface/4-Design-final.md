# E-Project - Sistema de Gestão de Projetos Acadêmicos UFAM

[![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)]()

##  Sobre o Projeto

O **E-Project** é um sistema de gestão acadêmica desenvolvido especificamente para a Universidade Federal do Amazonas (UFAM), focado no gerenciamento e acompanhamento de projetos de pesquisa, extensão e ensino.

("https://www.figma.com/design/lLDopNGZcEgvP0ihCUu2W0/E-Project?node-id=0-1&t=hEyeKuFrlvNCNUQj-1")


###  Objetivo

Criar uma solução **prática, dinâmica e simples** que elimine o retrabalho de adaptação exigido por ferramentas genéricas (como Trello ou Excel), oferecendo um sistema pré-configurado com as características específicas dos projetos da UFAM.

##  Interfaces do Sistema

### Tela de Login
<img width="874" height="1702" alt="Tela de Login do E-Project" src="https://github.com/user-attachments/assets/a7bd9d1f-174c-4f28-9653-b406f52c8498"/>

A tela inicial do E-Project apresenta:
- Logo institucional da UFAM
- Identificação do sistema "E-Project"
- Opções de acesso diferenciadas:
  - **Orientador**: Para professores e coordenadores
  - **Orientando**: Para alunos e bolsistas
- Sistema específico para projetos: PIBIC, PACE, Pibex, PIBID e Mestrado

### Dashboard do Orientador

<img width="958" height="810" alt="Dashboard do E-Project" src="https://github.com/user-attachments/assets/790f45c0-59a5-4693-84e3-b1edcd0dde3f" />
<img width="630" height="876" alt="Captura de tela 2025-11-28 200321" src="https://github.com/user-attachments/assets/6532bc62-b25e-43c3-8158-24b5ad076a5f" />

O painel do orientador oferece uma visão completa com:

**Métricas Principais:**
- Total de Projetos (6)
- Projetos em Andamento (4)
- Projetos Concluídos (0)
- Projetos Atrasados (1)

**Funcionalidades:**
-  **Ver Editais**: Acesso a 3 novos editais disponíveis
-  **Controle de Presença**: Registro específico de presença dos orientandos
-  **Novo Projeto**: Cadastro rápido de projetos

**Filtros por Tipo:**
- Todos
- PIBIC
- PACE
- Pibex
- PIBID
- Mestrado

**Lista de Projetos Ativos:**
Cada projeto exibe:
- Nome e descrição
- Status (tag colorida)
- Orientador responsável
- Datas de início e término
- Pró-reitoria vinculada
- Progresso visual (%)
- Número do edital

### Dashboard do Orientando

<img width="809" height="821" alt="Captura de tela 2025-11-28 200356" src="https://github.com/user-attachments/assets/eeb4d84d-4ff9-43d4-af55-e4982e5ea54f" />

<img width="512" height="554" alt="Captura de tela 2025-11-28 200409" src="https://github.com/user-attachments/assets/0728dfa5-3330-4067-8f35-a0ec83abc8c5" />

O painel do orientando apresenta:

**Informações Centralizadas:**
- Nome do projeto vinculado
- Orientador responsável
- Acesso aos editais das Pró-Reitorias

**Filtros de Visualização:**
- Todas
- Propesp (Pesquisa)
- Proext (Extensão)
- Proeg (Ensino)
- Proplan (Planejamento)

**Status das Atividades:**
- Total de Editais (8)
- Editais Abertos (5)
- Encerramento em Breve (3)
- Novos (últimos 7 dias) (0)

**Lista de Editais Disponíveis:**
Cada edital mostra:
- Tipo (PIBIC, PACE, Pibex, PIBID)
- Título do programa
- Descrição resumida
- Data de publicação
- Prazo final (destacado em vermelho quando próximo)
- Pró-reitoria responsável
- Número do edital
- Botão "Acessar Edital"

##  Funcionalidades Principais

### Para Orientadores
-  Gestão completa de projetos acadêmicos
-  Acompanhamento de progresso em tempo real
-  Controle de presença específico para bolsistas
-  Visualização integrada de projetos relacionados
-  Envio de demandas aos orientandos
-  Dashboard com métricas e indicadores
-  Filtros por tipo de projeto e pró-reitoria

### Para Orientandos
-  Visualização de tarefas e demandas
-  Acompanhamento do próprio progresso
-  Acesso centralizado aos editais abertos
-  Notificações de prazos importantes
-  Interface simplificada e intuitiva

### Centralização de Editais
-  Agregação automática de editais das pró-reitorias
-  Notificações de novos editais
-  Links diretos para documentação oficial
-  Alertas de prazos próximos ao vencimento

##  Tipos de Projetos Suportados

| Tipo | Descrição | Pró-Reitoria |
|------|-----------|--------------|
| **PIBIC** | Programa Institucional de Bolsas de Iniciação Científica | Propesp |
| **PACE** | Programa de Apoio à Cultura e Extensão | Proext |
| **Pibex** | Programa Institucional de Bolsas de Extensão | Proext |
| **PIBID** | Programa Institucional de Bolsas de Iniciação à Docência | Propesp |
| **Mestrado** | Programas de Pós-Graduação Stricto Sensu | Propesp |

##  Diferenciais

###  Especificidade UFAM
- Sistema pré-configurado com as características dos projetos da UFAM
- Elimina retrabalho de adaptação de ferramentas genéricas
- Nomenclaturas, fluxos e processos alinhados com as normativas institucionais

###  Integração Planejada
- **E-campus**: Sincronização de atualizações e relatórios
- **Sites das Pró-Reitorias**: Importação automática de editais
- Conformidade com SEI e sistemas oficiais

###  Controle de Acesso
- **Nível Orientador**: Acesso total e gestão completa
- **Nível Orientando**: Acesso restrito focado em tarefas e demandas

##  Problemas Resolvidos

| Problema | Solução E-Project |
|----------|-------------------|
| Ferramentas genéricas sem especificidade | Sistema customizado para UFAM |
| Retrabalho de adaptação | Pré-configuração inteligente |
| E-campus/SEI sem acompanhamento | Dashboard com métricas e progresso |
| Dispersão de informações | Centralização de editais |
| Múltiplos acessos diários | Portal único integrado |

##  Paleta de Cores

- **Verde Institucional**: `#1B5E20` (cor principal UFAM)
- **Verde Claro**: `#4CAF50` (destaques e ações positivas)
- **Azul Escuro**: `#1565C0` (informações e links)
- **Amarelo**: `#FDD835` (alertas e destaques)
- **Vermelho**: `#D32F2F` (prazos críticos)
- **Cinza**: `#424242` (textos secundários)


##  Público-Alvo

### Primário
- **Professores/Orientadores**: Gestão completa de projetos e equipes

### Secundário
- **Alunos/Orientandos**: Acompanhamento de tarefas e demandas
- **Coordenadores**: Visão estratégica dos programas

**E-Project** - Gestão Acadêmica Inteligente para a UFAM 

*Universidade Federal do Amazonas - Simplificando a gestão de projetos acadêmicos*# Design Final - E-Project

<div align="center">


---
---

## 📱 Interface Mobile - Fluxo do Aluno (Membro 4)

Este módulo foi desenhado especificamente para a **Persona Ana Beatriz** (Estudante de Engenharia e bolsista PIBIC), focando em resolver suas dores principais: sobrecarga de tarefas e incerteza sobre a comunicação com o orientador.

### 1. Tela de Tarefas (Dashboard Mobile)
Focada na organização rápida e redução de ansiedade.
* **Card de Destaque:** Exibe a entrega mais urgente ("Relatório Parcial") com alerta de prazo em destaque, ajudando a aluna a priorizar.
* **Lista de Demandas:** Cards com áreas de toque expandidas (acessibilidade) para facilitar o uso em movimento.
* **Integração:** Exibe tarefas reais do projeto "Biodiversidade Amazônica" e obrigações administrativas (Frequência, Estágio).

<img width="631" height="1358" alt="Tela 1 - Lista de Tarefas" src="https://github.com/user-attachments/assets/30fcf375-11ac-4f23-b343-05e19292e2bb" />

### 2. Submissão e Atualização
Combina duas funcionalidades em uma única tela para otimizar o tempo do aluno:
* **Upload Intuitivo:** Área de anexo clara com padrão de traçado.
* **Canal Direto:** Campo de mensagem integrado para enviar atualizações de status junto com o arquivo, centralizando a comunicação que antes ficava dispersa no WhatsApp.
* **Botão de Ação:** Botão "Enviar Atividade" com largura total para fácil alcance do polegar.

<img width="631" height="1358" alt="Tela 2 - Upload e Envio" src="https://github.com/user-attachments/assets/b4e1b8ca-debd-4043-b829-aa01588b5226" />

### 3. Feedback do Sistema (Sucesso e Erro)
Telas essenciais para garantir a confirmação da ação e reduzir a insegurança da aluna.
* **Sucesso (Verde):** Confirmação visual clara e mensagem tranquilizadora ("O orientador recebeu sua notificação").
* **Erro (Alerta):** Instrução clara de correção ("Verifique sua conexão") para evitar frustração.

<img width="631" height="1358" alt="Tela 3 - Sucesso" src="https://github.com/user-attachments/assets/f3602ce5-2fec-45ba-92de-8121a8e3e812" />
<img width="392" height="851" alt="Tela 4 - Erro" src="https://github.com/user-attachments/assets/fa57e469-ada6-44d1-8fa6-08564fe11a94" />

### 🎨 Consistência Visual 
O projeto mobile segue estritamente o Design System estabelecido para a versão Desktop (Membro 3):
* **Cores:** Uso do Verde UFAM (#1B5E20) como cor primária e Vermelho (#D32F2F) para estados de erro/alerta.
* **Tipografia:** Hierarquia de textos alinhada com o sistema web.



### 4. Confirmação de Funções 
(Revisar Apresentação)
Função:
Esta tela serve como o ponto de entrada para a tarefa "Revisar Apresentação", fornecendo à Ana Beatriz todo o contexto (status, prazo, instruções) e os documentos necessários para iniciar a revisão.

Decisões de Usabilidade e Acessibilidade:
Comunicação de Urgência: O bloco Status é proeminente, usando um ícone de alerta (⚠️) e a cor vermelha/laranja para o Prazo (14/12/2025), sinalizando que a tarefa é Pendente e requer ação imediata (WCAG 1.4.1 – Uso de cor).

Acesso a Documentos (CRUCIAL):

A seção "Documentos Necessários" lista de forma clara tanto o arquivo principal (Rascunho_Projeto1.pptx) quanto o anexo de apoio (Feedback_Prof.pdf).
As ações "Baixar" e "Visualizar" são botões de alto contraste, garantindo fácil acesso aos materiais.

Hierarquia de Ação:

O botão "Abrir para Revisão" é o botão primário, com um ícone de olho (👁️) que reforça a natureza da tarefa. Ele guia o usuário para o próximo passo no fluxo de trabalho.

O botão "Marcar como Não Aplicável" é o botão secundário, posicionado de forma discreta para não desviar a atenção da ação principal, mas acessível se necessário.

Instruções Flexíveis: As instruções breves estão disponíveis, com o botão "Ver instruções completas" permitindo a expansão de detalhes sem sobrecarregar a tela.

<img width="239" height="526" alt="Captura de tela 2025-12-01 104214" src="https://github.com/user-attachments/assets/710ff398-fdb7-40cf-84c8-ad983a0bb820" />

### 5. Enviar Artigo
Função:
Permitir que o usuário, Ana Beatriz, submeta seu artigo final, garantindo que todos os requisitos de formato e conteúdo sejam atendidos antes do envio.

Decisões de Usabilidade e Acessibilidade:
Prevenção de Erros (WCAG 3.3.4): A seção "Requisitos de Submissão" atua como um checklist obrigatório. O botão "Enviar Artigo Definitivo" é desabilitado (cinza) e só é habilitado em verde após o upload e a marcação dos requisitos, minimizando erros formais de submissão.

Upload Intuitivo: A área de upload com o ícone de nuvem e a borda tracejada oferece suporte a "arrastar e soltar" e é visualmente clara. O feedback de arquivo carregado ("Tese_Final_Ana.pdf") com a opção de "Remover" permite correção imediata.

Hierarquia Visual: O prazo está destacado, e as notas opcionais estão separadas, mantendo o foco do usuário no upload e no checklist.

<img width="392" height="851" alt="Tela 6" src="https://github.com/user-attachments/assets/8df11aed-7ae9-4114-ab79-125403a3f35e" />


### 6. Registrar Presença
Função:
Oferecer um mecanismo de check-in simples e rápido para a presença da Ana Beatriz (conforme a necessidade da Persona P2), validando sua localização dentro de um raio permitido.

Decisões de Usabilidade e Acessibilidade:
Simplicidade e Rapidez (E1): O design é focado na ação de "CHECK-IN AGORA". O botão primário é grande, verde e imediatamente clicável, desde que a validação de localização seja positiva.

Clareza da Localização: A validação "✔ LOCALIZAÇÃO VÁLIDA" em verde fornece feedback visual imediato, essencial para tarefas sensíveis a localização. O ícone de localização reforça o contexto.

Contexto Temporal (E6): A data "Hoje é: Segunda-feira..." é exibida com destaque, informando imediatamente o usuário sobre o contexto da tarefa.

Organização: O link "Ver histórico de Presença" está convenientemente posicionado como um botão secundário para usuários organizados (como a Ana) que desejam conferir registros anteriores.

<img width="392" height="851" alt="Tela 7" src="https://github.com/user-attachments/assets/952fd764-57ba-4f26-8bd9-ea2c8bea9d78" />


### 7. Relatório de Estágio
Função:
Gerenciar a submissão formal do Relatório de Estágio, que requer vários anexos e o cumprimento de requisitos específicos de formatação e conteúdo.
Decisões de Usabilidade e Acessibilidade:
Clareza de Fluxo: A tela é dividida em blocos lógicos (Instruções, Checklist, Upload), guiando o usuário passo a passo pela submissão.

Instruções Detalhadas: Os links "Ver Instruções Completas" e "Ver Regras de Formatação ABNT" permitem que a Ana acesse informações adicionais sem sobrecarregar a tela principal.

Múltiplos Uploads: A seção "Upload de Arquivo" distingue claramente entre o 1. Arquivo Principal e o 2. Anexo Obrigatório, resolvendo o desafio de submissão de múltiplos documentos. Cada botão de upload é rotulado para clareza.

Requisitos Formaiss: O "Checklist" garante que itens críticos (como a assinatura do supervisor) não sejam esquecidos, fundamental para relatórios de estágio.
<img width="392" height="851" alt="Tela 8" src="https://github.com/user-attachments/assets/0f97779c-5b6d-4984-9faf-28d20ff00cc7" />


### 8. Opções de Acessibilidade
Função:
Permitir que o usuário ajuste a interface do aplicativo para atender às suas necessidades visuais, cognitivas e de interação, tornando o aplicativo mais inclusivo e aderente às diretrizes WCAG.

Decisões de Usabilidade e Acessibilidade:
Organização por Categorias: A tela é claramente dividida em três categorias lógicas (Visualização e Contraste, Auxílio à Leitura, Interação e Tempo), facilitando a navegação e o entendimento rápido das opções.

- Visualização e Contraste:

Tamanho de Texto: Uso de slider (controle deslizante) para ajuste fino do tamanho da fonte, crucial para baixa visão.

Modo de Alto Contraste: Permite ativar o modo de contraste mais alto, garantindo legibilidade (idealmente contraste de 7:1 para texto grande e 4.5:1 para texto normal).

Modo Escuro (Dark Mode): Reduz o cansaço visual.

Desativar Animações: Evita confusão e desorientação para usuários com sensibilidade a movimentos (WCAG 2.3.3).

- Auxílio à Leitura:

Destaque de Foco para Teclado: Ativa um contorno visível (anel de foco) ao redor do elemento ativo, essencial para a navegação por teclado (WCAG 2.4.7).

Simplificar Rótulos de Botão: Melhora a experiência para usuários de leitores de tela ao reduzir a complexidade textual.

- Interação e Tempo:

Aumentar Área de Toque (Hit Area): Garante que a área de toque dos botões e links atinja o mínimo recomendado de 44×44px, auxiliando usuários com dificuldades motoras (WCAG 2.5.5).

Alertas de Tempo Estendido: Permite mais tempo para o usuário responder a mensagens ou janelas de sessão, evitando que a ação expire rapidamente (WCAG 2.2.1).

Componentes de Interface: O uso de Toggle Switches para as opções binárias (Ligado/Desligado) é intuitivo e padrão em interfaces móveis.

Ação Final: O botão "SALVAR ALTERAÇÕES" é o ponto focal da tela, e o link "Restaurar Configurações Padrão" permite o reset seguro das preferências.
<img width="392" height="851" alt="Acessibilidade (2)" src="https://github.com/user-attachments/assets/2a36a26b-8afa-459e-b260-68ee77b4118e" />


- Tela de Confirmação (Pós-Ação)
Função:
Essa tela é um feedback imediato, simples e inconfundível para o usuário, confirmando que uma ação importante (como salvar configurações, enviar um artigo, ou fazer um check-in) foi concluída com êxito.

Decisões de Usabilidade:
Clareza Imediata: O ícone de check em um círculo verde é um padrão universal de "Sucesso", garantindo que o usuário não tenha dúvidas sobre o resultado.

Foco na Ação: O texto "Alterações Salvas com Sucesso!" é breve e direto.

Ação de Saída: O único botão ativo é "Voltar para o Início", guiando o usuário de volta ao ponto principal de navegação para continuar seu trabalho.

<img width="392" height="851" alt="Acessibilidade (1)" src="https://github.com/user-attachments/assets/e7431fdf-fd7c-44e3-b4b2-9824d5afb72a" />








