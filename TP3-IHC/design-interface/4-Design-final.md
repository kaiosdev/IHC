# Design Final - E-Project

<div align="center">

## Sistema de Gestão de Projetos Acadêmicos da UFAM

</div>

Este documento apresenta o design final da interface do **E-Project**, consolidando todas as diretrizes estabelecidas nos documentos anteriores (Mural de Inspiração, Paleta & Tipografia, Ícones & Ilustrações). As telas demonstram a aplicação prática dos princípios de usabilidade, acessibilidade e identidade visual institucional.

---

## 1. Tela de Login

<div align="center">

<img width="874" height="1702" alt="Tela de Login do E-Project" src="https://github.com/user-attachments/assets/a7bd9d1f-174c-4f28-9653-b406f52c8498"/>

</div>

### Descrição
A tela de login apresenta a identidade visual do E-Project com destaque para o verde institucional da UFAM (`#00663C`).

#### Elementos Principais
- **Cabeçalho Verde:** Topo da tela com a cor primária da UFAM, estabelecendo imediatamente a identidade institucional
- **Logo E-Project:** Centralizado no topo com tipografia **Montserrat Bold** em branco sobre o fundo verde
- **Ilustração de Boas-vindas:** Ícone representando gestão acadêmica (notebook/documentos) no estilo Material Rounded
- **Formulário de Login:**
  - Campos com bordas arredondadas e placeholders descritivos
  - Ícones de pessoa (`person`) e cadeado (`lock`) identificando cada campo
  - Tipografia **Roboto Regular 16px** garantindo legibilidade
- **Botão "Entrar":** Verde UFAM com texto branco em **Roboto Bold**
- **Link "Esqueci a senha":** Em azul (`#005875`) com sublinhado ao passar o mouse
- **Fundo:** Cinza Gelo (`#F5F5F5`) reduzindo fadiga visual

#### Heurísticas Aplicadas
- **Visibilidade do Estado:** Campos indicam foco através de borda destacada
- **Correspondência com o Mundo Real:** Ícones universais (pessoa = usuário, cadeado = senha)
- **Prevenção de Erros:** Validação em tempo real dos campos obrigatórios

---

## 2. Dashboard Principal

<div align="center">

<img width="958" height="810" alt="Dashboard do E-Project" src="https://github.com/user-attachments/assets/790f45c0-59a5-4693-84e3-b1edcd0dde3f" />

</div>

### Descrição
O Dashboard é o hub central do sistema, inspirado no layout em cards do Google Classroom e na navegação lateral do Microsoft Teams.

#### Estrutura da Interface

**A. Barra Superior (Header)**
- **Fundo:** Verde UFAM (`#00663C`)
- **Logo E-Project:** Canto superior esquerdo com ícone home
- **Barra de Busca Global:** Campo centralizado com ícone de lupa (`search`)
- **Ícones de Utilidade:** Notificações (`notifications`) e perfil do usuário (`person`)
- **Tipografia:** **Montserrat SemiBold 20px** para o título

**B. Menu Lateral Esquerdo**
Inspirado no Microsoft Teams, com ícones + texto em estrutura vertical:
- 🏠 **Início** (home) - Estado ativo destacado em verde
- 📁 **Meus Projetos** (folder_open)
- 📄 **Editais** (source_notes)
- 📝 **Documentos** (description)
- 👤 **Perfil** (person)
- 👁️ **Acessibilidade** (visibility)

Cada item possui:
- Ícone Material Rounded 24px
- Rótulo em **Roboto Medium 16px**
- Área de toque 48x48dp (mobile)

**C. Área de Conteúdo Principal**
- **Cards de Projetos:** Layout em grid 3 colunas (desktop) / 1 coluna (mobile)
  - **Cabeçalho do Card:** Verde com título do projeto em branco
  - **Corpo do Card:** Informações do orientador, tipo de projeto (PIBIC/PACE), status
  - **Rodapé do Card:** Ícones de ação (editar, favoritar, arquivar)
- **Botão Flutuante (+):** Canto inferior direito em Amarelo (`#FFF700`) para adicionar novo projeto

#### Informações Exibidas nos Cards
1. **Título do Projeto:** **Montserrat Bold 18px**
2. **Orientador:** **Roboto Regular 14px** com ícone de pessoa
3. **Tipo:** Badge colorido (PIBIC = Azul, PACE = Verde)
4. **Status:** Indicador visual (Em Andamento/Concluído/Atrasado)
5. **Prazo:** Data de entrega com ícone de calendário (`calendar_today`)

#### Heurísticas Aplicadas
- **Reconhecimento vs. Memorização:** Ícones com rótulos textuais eliminam necessidade de memorizar funções
- **Consistência:** Todos os cards seguem o mesmo padrão visual
- **Estética Minimalista:** Informações essenciais sem poluição visual

---

## 3. Detalhes do Projeto

<div align="center">

<img width="630" height="876" alt="Tela de Detalhes do Projeto" src="https://github.com/user-attachments/assets/f200afae-afd2-4139-ad06-81fdb82a8844" />

</div>

### Descrição
Tela de visualização completa de um projeto individual, acessada ao clicar em um card do Dashboard.

#### Estrutura

**A. Cabeçalho do Projeto**
- **Fundo Verde UFAM** com título do projeto em branco
- **Breadcrumb:** "Início > Meus Projetos > [Nome do Projeto]" para contexto de navegação
- **Botão Voltar:** Seta esquerda (`arrow_back`) no canto superior esquerdo

**B. Informações Detalhadas**
Organizadas em seções com ícones identificadores:

1. **Dados Gerais**
   - 👤 Orientador(a)
   - 📅 Data de Início/Término
   - 🏷️ Tipo de Projeto (PIBIC/PACE/PAIC)
   - ⚠️ Status Atual

2. **Descrição e Objetivos**
   - Campo de texto expandido com **Roboto Regular 16px**
   - Ícone de documento (`description`)

3. **Tarefas e Cronograma**
   - Lista de tarefas com checkboxes
   - Barra de progresso visual (% de conclusão)
   - Ícone de checklist (`checklist`)

4. **Documentos Anexados**
   - Lista de arquivos com ícones de tipo (PDF, DOCX, etc.)
   - Botões de download e visualização
   - Ícone de anexo (`attach_file`)

**C. Ações Contextuais**
- **Botões Principais:**
  - "Editar Projeto" (Azul `#005875`)
  - "Gerar Relatório" (Verde `#00663C`)
  - "Arquivar" (Cinza)

#### Heurísticas Aplicadas
- **Flexibilidade:** Usuários avançados podem usar atalhos de teclado (Alt+E para editar)
- **Controle do Usuário:** Botão "Voltar" sempre visível
- **Prevenção de Erros:** Confirmação modal antes de arquivar projeto

---

## 4. Tela de Editais

<div align="center">

<img width="809" height="821" alt="Tela de Editais" src="https://github.com/user-attachments/assets/8040f874-0163-433a-855a-bed0ecedfc0e" />

</div>

### Descrição
Feed unificado de oportunidades acadêmicas (PIBIC, PACE, PAIC) com filtros inteligentes.

#### Elementos Principais

**A. Barra de Filtros**
- **Dropdowns de Seleção:**
  - Tipo de Edital (PIBIC/PACE/PAIC/Todos)
  - Status (Aberto/Fechado/Em Breve)
  - Área de Conhecimento (Exatas/Humanas/Biológicas)
- **Campo de Busca:** Pesquisa por palavra-chave no título/descrição
- **Ícone de filtro** (`filter_list`) com badge indicando filtros ativos

**B. Cards de Editais**
Layout em lista vertical, cada card contém:

1. **Cabeçalho:**
   - Título do Edital (**Montserrat SemiBold 18px**)
   - Badge de status colorido:
     - 🟢 Verde = Aberto
     - 🔴 Vermelho = Fechado
     - 🟡 Amarelo = Em Breve

2. **Corpo:**
   - 📅 Data de Abertura/Encerramento
   - 🏛️ Órgão Responsável (PROPESP/PROEXT)
   - 📝 Resumo da descrição (máximo 3 linhas)
   - 💰 Valor da bolsa (se aplicável)

3. **Rodapé:**
   - Botão "Ver Detalhes" (Verde)
   - Ícone de favorito (`star_outline` / `star`) para salvar edital

**C. Paginação**
- Navegação numérica na parte inferior
- "Anterior" e "Próximo" com setas (`chevron_left` / `chevron_right`)

#### Heurísticas Aplicadas
- **Visibilidade do Status:** Badges coloridos indicam urgência (vermelho = fechado)
- **Eficiência de Uso:** Filtros reduzem tempo de busca para usuários frequentes
- **Ajuda e Documentação:** Tooltip explicativo ao passar mouse sobre ícones

---

## 5. Modal de Acessibilidade

<div align="center">

<img width="512" height="554" alt="Modal de Configurações de Acessibilidade" src="https://github.com/user-attachments/assets/96e6424a-c613-4beb-91e2-b03fb639b672" />

</div>

### Descrição
Painel dedicado às configurações de acessibilidade, desenvolvido especificamente para a **Persona Prof. Carlos (Baixa Visão)**.

#### Funcionalidades

**A. Tamanho da Fonte**
- **Controles:** Botões [-] e [+] com ícone de texto (`text_fields`)
- **Opções:** Pequeno (14px) / Médio (16px - Padrão) / Grande (18px) / Extra Grande (20px)
- **Feedback Visual:** Tamanho atual destacado em verde

**B. Modo de Alto Contraste**
- **Toggle Switch:** Ativa/Desativa modo de alto contraste
- **Ícone:** Olho com brilho (`visibility`)
- **Efeito:** Inverte cores para fundo escuro (#000000) com texto branco (#FFFFFF)

**C. Espaçamento de Elementos**
- **Slider:** Ajusta padding entre componentes (Compacto/Normal/Espaçoso)
- **Ícone:** Régua (`straighten`)
- **Aplicação:** Aumenta área de toque em 25% quando configurado para "Espaçoso"

**D. Navegação por Teclado**
- **Checkbox:** Ativa indicadores visuais de foco (bordas destacadas)
- **Ícone:** Teclado (`keyboard`)
- **Benefício:** Facilita navegação sem mouse para usuários com mobilidade reduzida

**E. Leitor de Tela (Screen Reader)**
- **Status:** Detecta automaticamente se há leitor ativo (NVDA/JAWS)
- **Ícone:** Alto-falante (`volume_up`)
- **Configuração:** Adiciona `aria-labels` descritivos em todos os elementos

#### Botões de Ação
- **Salvar Preferências:** Verde UFAM
- **Redefinir Padrão:** Azul Profundo
- **Fechar:** Ícone X (`close`) no canto superior direito

#### Heurísticas Aplicadas
- **Flexibilidade:** 5 níveis de customização adaptam-se a diferentes necessidades
- **Reconhecimento:** Cada opção tem ícone + rótulo + descrição auxiliar
- **Consistência:** Configurações persistem entre sessões via `localStorage`

---

## 6. Princípios de Design Aplicados

### A. Acessibilidade (WCAG 2.1 Nível AA)
✅ **Contraste Mínimo 4.5:1** em todos os textos  
✅ **Área de Toque ≥ 48x48dp** em dispositivos móveis  
✅ **Navegação por Teclado** com indicadores visuais claros  
✅ **Rótulos Textuais** acompanham todos os ícones  
✅ **Feedback Sonoro** para ações críticas (via screen reader)

### B. Heurísticas de Nielsen
| Heurística | Implementação |
|:-----------|:--------------|
| **Visibilidade do Estado** | Menu lateral destaca seção ativa em verde |
| **Linguagem do Usuário** | Termos acadêmicos (PIBIC, PACE) conhecidos pela comunidade UFAM |
| **Controle e Liberdade** | Botão "Voltar" sempre presente, ações reversíveis |
| **Consistência** | Mesma estrutura de card em todos os módulos |
| **Prevenção de Erros** | Validação de formulários em tempo real |
| **Reconhecimento** | Ícones Material + rótulos eliminam memorização |
| **Flexibilidade** | Atalhos de teclado para usuários avançados |
| **Design Minimalista** | Máximo de 3 ações por card |
| **Recuperação de Erros** | Mensagens claras com soluções ("Senha incorreta. Clique aqui para redefinir") |
| **Ajuda** | Tooltips contextuais em elementos complexos |

### C. Psicologia das Cores
- **Verde (`#00663C`):** Institucionalidade, confiança, crescimento acadêmico
- **Azul (`#005875`):** Profissionalismo, clareza, navegação neutra
- **Amarelo (`#FFF700`):** Urgência, destaque, ações importantes (usado com moderação)
- **Cinza Gelo (`#F5F5F5`):** Reduz fadiga visual comparado ao branco puro

### D. Responsividade
- **Desktop (≥1024px):** Grid de 3 colunas para cards
- **Tablet (768-1023px):** Grid de 2 colunas
- **Mobile (<768px):** Layout em coluna única com menu hamburger

---

## 7. Diferenciais do E-Project

### Comparação com Soluções Genéricas

| Aspecto | Trello/Notion (Genérico) | E-Project (Especializado) |
|:--------|:-------------------------|:--------------------------|
| **Terminologia** | "Board", "Task", "Workspace" | "Projeto PIBIC", "Relatório PACE", "Edital PROPESP" |
| **Fluxo de Trabalho** | Usuário configura do zero | Pré-configurado para processos UFAM |
| **Integração** | APIs externas complexas | Integração nativa com SIGAA/PROPESP |
| **Curva de Aprendizado** | 5-7 dias para dominar | ≤ 3 cliques por tarefa (imediato) |
| **Identidade Visual** | Paletas genéricas | Verde institucional UFAM |

---

## 8. Validação com Personas

### Persona 1: Prof. Victor (Eficiência)
✅ Dashboard mostra todos os projetos em uma única tela  
✅ Busca global encontra qualquer informação em < 2 segundos  
✅ Botão flutuante (+) permite criar projeto em 3 cliques  

### Persona 2: Ana Beatriz (Organização)
✅ Cards visuais com status coloridos facilitam priorização  
✅ Filtros de editais por área de conhecimento (Humanas)  
✅ Checklist de tarefas com barra de progresso motivacional  

### Persona 3: Prof. Carlos (Acessibilidade)
✅ Modo de alto contraste com 4.5:1 de contraste mínimo  
✅ Fonte ajustável até 20px sem quebra de layout  
✅ Todos os ícones possuem `aria-label` descritivo  

---

## 9. Próximos Passos

1. **Prototipação Interativa:** Desenvolver versão clicável no Figma para testes de usabilidade
2. **Testes com Usuários Reais:** 5 professores da UFAM (incluindo pessoa com baixa visão)
3. **Ajustes Iterativos:** Refinar com base no feedback (metodologia ágil)
4. **Implementação Front-end:** HTML/CSS/JavaScript seguindo este guia de estilos
5. **Integração Back-end:** Conectar com APIs do SIGAA e PROPESP

---

## 10. Conclusão

O design final do **E-Project** materializa os princípios estabelecidos nos documentos anteriores, criando uma interface que é simultaneamente:

- **Institucional:** Reflete a identidade visual da UFAM
- **Funcional:** Resolve os problemas mapeados nas personas
- **Acessível:** Atende rigorosamente às diretrizes WCAG 2.1
- **Familiar:** Inspira-se em padrões consolidados (Classroom/Teams)
- **Especializado:** Fala a "linguagem nativa" da comunidade acadêmica

Ao consolidar gestão de projetos, editais e documentos em uma única plataforma otimizada, o E-Project reduz a fragmentação de ferramentas e aumenta a produtividade dos pesquisadores da UFAM, cumprindo sua promessa de ser **"Electronic, Efficient, UFAM"**.

---

<div align="center">

**Desenvolvido com 💚 para a comunidade acadêmica da UFAM**

</div>
