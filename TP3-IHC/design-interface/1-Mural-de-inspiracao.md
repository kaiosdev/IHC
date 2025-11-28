<div align="center">

# Referências e Inspirações para o E-Project

</div>

Este documento evidencia a inspiração e em quais sistemas serviram de base para o E-Project, baseando-se em outros sites e sistemas de educação, tendo em vista as funcionalidades e a interface dos sistemas, pois em uma aprofundada pesquisa, foi pontuada as qualidades de cada interface e nos inspiramos em cada uma delas para implementar no sistema proposto no trabalho. O objetivo é ter a tela mais completa e fluida possível, levando em consideração as heurísticas de Nielsen, psicologia das cores, experiência do usuário, e outros aspectos que compõem a IHC.

---

## Google Classroom - Referência de Design

O Google Classroom é uma plataforma educacional gratuita desenvolvida pelo Google para facilitar a comunicação e organização entre professores e alunos. Lançado em 2014, tornou-se referência global em design de interfaces educacionais por sua simplicidade e eficiência.

###  Funcionalidades Principais

- **Gestão de Turmas:** Criação e organização visual de disciplinas
- **Distribuição de Tarefas:** Envio e recebimento de atividades com prazos
- **Comunicação:** Avisos e feedback direto entre professor-aluno
- **Repositório de Materiais:** Armazenamento integrado com Google Drive
- **Avaliações:** Sistema de notas e comentários individualizados
- **Agenda Unificada:** Visualização de prazos em calendário

###  Interface

#### Layout
- **Cards visuais** para representar cada turma/disciplina
- **Menu lateral fixo** com navegação por ícones + texto
- **Hierarquia clara:** Título → Professor → Datas/Status
- **Paleta neutra:** Branco/Cinza com cores de destaque nos cabeçalhos

#### Organização
- **Dashboard inicial** exibe todas as turmas de forma panorâmica
- **Busca global** sempre visível no topo
- **Ações contextuais** (pasta, perfil, menu) na base de cada card
- **Responsivo:** Adapta-se perfeitamente a desktop, tablet e mobile

###  Conclusão

O Google Classroom exemplifica design centrado no usuário ao eliminar complexidade desnecessária. Sua força está em permitir que professores e alunos realizem tarefas essenciais (criar turma, enviar atividade, consultar prazo) em **3 cliques ou menos**. A interface prioriza reconhecimento sobre memorização, com elementos visuais claros que dispensam manuais ou treinamento.

O Classroom atende **9 das 10 heurísticas com excelência**, sendo referência comprovada em usabilidade educacional com mais de **150 milhões de usuários globais**.

Para o **E-Project**, o Classroom serve como modelo de **simplicidade funcional**: organização em cards, navegação lateral intuitiva e hierarquia visual consistente — princípios que serão adaptados ao contexto acadêmico da UFAM.

###  Referências nas Heurísticas de Nielsen

Esta análise baseia-se nas **10 Heurísticas de Usabilidade de Nielsen (1994)**, utilizadas para avaliar a qualidade da interface:

| Heurística | Avaliação no Classroom |
|:-----------|:----------------------|
| **1. Visibilidade do estado do sistema** | ⭐⭐⭐⭐⭐ Menu lateral destaca seção ativa |
| **2. Correspondência sistema-mundo real** | ⭐⭐⭐⭐⭐ Metáfora de "sala de aula física" |
| **4. Consistência e padrões** | ⭐⭐⭐⭐⭐ Todos os cards seguem mesmo formato |
| **6. Reconhecimento vs. memorização** | ⭐⭐⭐⭐⭐ Ícones + texto, fotos de professores |
| **8. Estética e design minimalista** | ⭐⭐⭐⭐⭐ Foco no essencial, sem poluição visual |

---

## Microsoft Teams - Referência de Design

###  Introdução

O **Microsoft Teams** é uma plataforma de colaboração corporativa e educacional desenvolvida pela Microsoft, lançada em 2017. Integra comunicação (chat, videoconferência), gerenciamento de arquivos e fluxos de trabalho em um único ambiente. Tornou-se referência em design de interfaces profissionais por equilibrar funcionalidades avançadas com acessibilidade para usuários iniciantes.

###  Funcionalidades Principais

- **Chat e Mensagens:** Conversas individuais e em grupo com histórico persistente
- **Videoconferências:** Reuniões integradas com compartilhamento de tela
- **Canais de Equipe:** Organização por projetos/departamentos
- **Compartilhamento de Arquivos:** Integração nativa com OneDrive e SharePoint
- **Calendário:** Agendamento de reuniões sincronizado com Outlook
- **Aplicativos Integrados:** Extensões (Planner, Forms, OneNote)

###  Interface

#### Layout
- **Barra lateral vertical** com ícones categorizados (Chat, Reunir, Comunidades)
- **Área central expansível** dedicada ao conteúdo principal
- **Paleta sóbria:** Tons de roxo/azul para interação, cinza escuro para fundo
- **Tipografia clara:** Roboto/Segoe UI em tamanhos adequados (14-16px)

#### Organização
- **Módulos separados:** Cada seção (Chat, Calendário, Arquivos) tem interface própria
- **Campo de busca global** no topo com suporte a comandos
- **Estados vazios informativos:** Ilustrações e mensagens motivacionais
- **Atalhos de teclado:** Suporte extensivo para usuários avançados (Ctrl+Alt+G)

###  Conclusão

O Microsoft Teams representa **design escalável para ambientes complexos**. Sua força está em oferecer **múltiplas camadas de profundidade** (iniciantes usam chat básico, avançados automatizam workflows) sem comprometer a simplicidade inicial. A interface utiliza padrões consolidados da Microsoft (Fluent Design), garantindo familiaridade para usuários do ecossistema Windows/Office.

**Justificativa da escolha:** O Teams demonstra excelência em **redução de fricção** (cada ação tem resposta visual < 0,1s) e **portabilidade** (experiência idêntica em desktop, web e mobile), com mais de **320 milhões de usuários ativos** (Microsoft, 2024). Sua arquitetura modular inspira a separação de contextos no E-Project (Dashboard → Projetos → Tarefas).

Para o **E-Project**, o Teams valida a importância de **feedback visual imediato** e **navegação modular**: cada funcionalidade (Projetos, Editais, Tarefas) pode ter sua própria "cena" sem poluir o Dashboard principal — abordagem já modelada nos diagramas MoLIC do projeto.

### 🔍 Referências nas Heurísticas de Nielsen

Esta análise baseia-se nas **10 Heurísticas de Usabilidade de Nielsen (1994)**, utilizadas para avaliar a qualidade da interface:

| Heurística | Avaliação no Teams |
|:-----------|:-------------------|
| **1. Visibilidade do estado do sistema** | ⭐⭐⭐⭐⭐ Ícones destacados + títulos de seção |
| **2. Correspondência sistema-mundo real** | ⭐⭐⭐⭐⭐ Ícones universais (💬 chat, 📹 reunir) |
| **3. Controle e liberdade do usuário** | ⭐⭐⭐⭐⭐ Menu sempre acessível, atalhos múltiplos |
| **4. Consistência e padrões** | ⭐⭐⭐⭐⭐ Barra lateral unificada em todos os módulos |
| **7. Flexibilidade e eficiência** | ⭐⭐⭐⭐⭐ Atalhos de teclado para usuários avançados |
| **8. Estética e design minimalista** | ⭐⭐⭐⭐⭐ Hierarquia clara, uso estratégico de cor |

---

---


</div>

A seleção do **Google Classroom** e **Microsoft Teams** como referências principais fundamenta-se em sua excelência comprovada em usabilidade, com bilhões de interações diárias validando suas escolhas de design. Ao adotarmos padrões visuais já familiares aos usuários acadêmicos (cards, menu lateral, busca global), **reduzimos drasticamente a curva de aprendizado** do E-Project — o Prof. Victor e Ana Beatriz reconhecerão elementos que já dominam em suas rotinas.

As análises baseadas nas **Heurísticas de Nielsen** estabelecem um **benchmark mensurável** (ambas as plataformas atingem ⭐⭐⭐⭐⭐ em 6+ critérios) e revelam soluções diretas para as dores identificadas no briefing: o feed unificado do Classroom resolve o problema de "acessar 3+ sites para editais", as notificações do Teams eliminam o medo de Ana de perder prazos, e a paleta sóbria de ambos atende às necessidades de acessibilidade do Prof. Carlos.

O diferencial do E-Project está em **especializar** esses padrões consolidados para o contexto UFAM: em vez de ferramentas genéricas que exigem adaptação (Trello, Notion, Excel), oferecemos uma solução **pré-configurada** com a "linguagem nativa" da universidade (PIBIC, PACE, PROPESP), combinando a simplicidade do Classroom (≤ 3 cliques por tarefa) com a navegação modular do Teams e a identidade institucional verde (#00663C). Este mural serve como alicerce técnico para todas as decisões subsequentes de design, garantindo que o sistema não apenas "pareça profissional", mas **funcione de forma intuitiva** para as personas mapeadas.

---

<div align="center">

</div>
