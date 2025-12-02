<div align="center">

# Referências e Inspirações para o E-Project

</div>

Este documento evidencia a inspiração e em quais sistemas serviram de base para o E-Project, baseando-se em outros sites e sistemas de educação, tendo em vista as funcionalidades e a interface dos sistemas, pois em uma aprofundada pesquisa, foi pontuada as qualidades de cada interface e nos inspiramos em cada uma delas para implementar no sistema proposto no trabalho. O objetivo é ter a tela mais completa e fluida possível, levando em consideração as heurísticas de Nielsen, psicologia das cores, experiência do usuário, e outros aspectos que compõem a IHC.

---

## Google Classroom - Referência de interface e cores

<div align="center">

<img width="1199" height="812" alt="design de inspiração" src="https://github.com/user-attachments/assets/869fff8b-d058-4b7b-9a48-1862f2a4fa95" />

</div>

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


<div align="center">

---

# Portal PROPESP/UFAM - Referência de Design Institucional

</div>
<img width="1083" height="947" alt="design proesp" src="https://github.com/user-attachments/assets/363266f8-6c76-4438-b768-bca2e85958f3" />

##  Introdução

O **Portal PROPESP** (Pró-Reitoria de Pesquisa e Pós-Graduação da UFAM) é o site institucional oficial responsável pela divulgação de editais, normas e informações sobre projetos acadêmicos (PIBIC, PACE, mestrado, doutorado). Como plataforma governamental, segue as diretrizes do e-MAG (Modelo de Acessibilidade em Governo Eletrônico) e representa a **identidade visual oficial** que professores e alunos da UFAM já conhecem.

---

##  Funcionalidades Principais

- **Divulgação de Editais:** Publicação de oportunidades de bolsas e projetos (PIBIC, PACE, PIBITI)
- **Documentação Institucional:** Normas, resoluções e calendários acadêmicos
- **Informações sobre Programas:** Detalhes de mestrado, doutorado e especialização
- **Contatos:** Informações de pró-reitorias e coordenações
- **Calendário Acadêmico:** Datas de submissão, defesas e eventos
- **Acessibilidade:** Ferramentas de ajuste de contraste e tamanho de fonte (A+, A, A-)

---

##  Interface

### Layout
- **Barra superior governamental:** Links para portais federais (Gov.br, Simplifique, Comunica BR)
- **Cabeçalho institucional verde:** Logo PROPESP + UFAM em destaque (identidade oficial)
- **Menu lateral fixo:** Navegação por categorias administrativas (A PROPESP, EDITAIS)
- **Área de conteúdo:** Texto denso com informações institucionais detalhadas

### Organização
- **Estrutura administrativa:** Organização por departamentos e hierarquia institucional
- **Breadcrumb:** Indicação de caminho de navegação (PÁGINA INICIAL > ACESSIBILIDADE)
- **Ferramentas de acessibilidade:** Botões A+/A-/A (ajuste de fonte), Alto Contraste, Atalhos de teclado (Alt+1/2/3/4)
- **VLibras:** Tradutor de Libras integrado (acessibilidade para surdos)

---

##  Análise Crítica

###  Pontos Fortes

#### **1. Familiaridade Institucional**
O portal utiliza a **paleta verde oficial da UFAM** (#00663C), criando reconhecimento imediato para professores e alunos. O Prof. Victor (Persona 1) já acessa este site regularmente para buscar editais, portanto qualquer sistema acadêmico da UFAM deve **manter elementos visuais familiares** (logo, cores institucionais) para evitar estranhamento.

#### **2. Conformidade Legal**
Segue as normas de acessibilidade do Governo Federal (e-MAG, Decreto 5.296/2004), garantindo que o sistema atenda requisitos legais — aspecto crítico para uma solução institucional como o E-Project.

#### **3. Recursos de Acessibilidade**
- **Alto contraste:** Alternância entre fundo claro/escuro (essencial para Prof. Carlos - Persona 3 com baixa visão)
- **Ajuste de fonte:** Botões A+/A-/A permitem personalização (embora com feedback visual limitado)
- **VLibras:** Inclusão para comunidade surda

---

###  Pontos Fracos (Oportunidades para o E-Project)

#### **1. Navegação Confusa**
- Menu lateral com **hierarquia administrativa** (Apresentação, Organograma, Atribuições) em vez de **hierarquia por tarefas** do usuário (Buscar Editais, Submeter Projeto)
- Breadcrumb não clicável (apenas informativo)
- Falta de busca com filtros (usuário precisa ler lista completa de editais)

#### **2. Densidade Visual**
- **Três barras de navegação** (Gov.br, Verde PROPESP, Menu Lateral) ocupam 200px+ de altura
- Texto pequeno e denso (< 14px em várias seções)
- Espaçamento apertado entre elementos (8-12px vs. recomendado 16-24px)

#### **3. Poluição de Interface**
- Links de atalho ("Ir para o conteúdo 1", "Ir para o menu 2") tecnicamente corretos para acessibilidade, mas **visualmente confusos** para usuários comuns
- Múltiplos tons de cinza sem hierarquia clara
- Falta de elementos visuais (ícones, cards) — tudo é baseado em texto

#### **4. Contraste de Cores (Problema Crítico)**
Apesar de ter ferramenta de "Alto Contraste", o **modo padrão apresenta problemas**:

| Elemento | Cor Fundo | Cor Texto | Problema |
|:---------|:----------|:----------|:---------|
| Cabeçalho | Verde escuro | Amarelo (#FFD700) | Contraste aceitável, mas texto pequeno dificulta leitura |
| Menu lateral (hover) | Preto | Amarelo | Adequado (modo Alto Contraste ativado) |
| Corpo do texto | Branco | Cinza médio (#616161) | Contraste insuficiente para Prof. Carlos |
| Datas/metadados | Branco | Cinza claro (#9E9E9E) | **Falha WCAG** — contraste < 4.5:1 |

**Problema Identificado:** No modo normal, textos secundários (datas, metadados) têm contraste baixo. Na página inicial com Alto Contraste, a interface melhora significativamente (fundo verde + texto branco), mas deveria ser o **padrão**, não uma opção escondida.

---

##  Conclusão

O Portal PROPESP representa a **realidade atual** que o E-Project precisa transformar: uma plataforma **funcionalmente completa**, mas com **experiência de usuário limitada**. Sua principal contribuição ao projeto é validar dois aspectos críticos:

### **1. Identidade Visual Institucional**
A paleta verde (#00663C) e o logo PROPESP/UFAM são **âncoras visuais** que o E-Project deve preservar. O Prof. Victor citou no briefing que precisa acessar "3+ sites de pró-reitorias" — ao manter elementos visuais familiares do PROPESP, reduzimos a percepção de "mais uma ferramenta nova" e criamos **continuidade institucional**.

### **2. Requisitos de Acessibilidade Real**
O portal demonstra que **conformidade técnica ≠ usabilidade acessível**. Ter botões A+/A-/A não resolve o problema se:
- O contraste padrão já é insuficiente (Prof. Carlos não deveria precisar "ativar" acessibilidade)
- Os botões não têm feedback visual claro (usuário clica e não sabe se funcionou)
- A fonte aumenta, mas o layout quebra (texto sobrepõe elementos)

### **Lições para o E-Project:**
-  **Adotar:** Paleta verde institucional, logo PROPESP, VLibras
-  **Melhorar:** Contraste alto como padrão (não opcional), fontes >= 16px, espaçamento generoso (16-24px)
-  **Simplificar:** Navegação por tarefas (não departamentos), busca com filtros visuais, cards em vez de listas textuais
-  **Evitar:** Múltiplas barras de navegação, menu apenas textual, linguagem burocrática

O E-Project não deve **replicar** o PROPESP, mas sim **evoluir** dele: manter a familiaridade institucional (cores, logo) enquanto resolve as frustrações de usabilidade identificadas no briefing (retrabalho, navegação confusa, falta de gestão integrada).

---

## 🔍 Referências nas Heurísticas de Nielsen

Esta análise baseia-se nas **10 Heurísticas de Usabilidade de Nielsen (1994)**, utilizadas para avaliar a qualidade da interface:

| Heurística | Avaliação no PROPESP |
|:-----------|:--------------------|
| **1. Visibilidade do estado do sistema** | ⭐⭐⭐☆☆ Breadcrumb presente, mas falta indicador de seção ativa no menu |
| **4. Consistência e padrões** | ⭐⭐⭐☆☆ Menu lateral sem padrão visual claro (alguns itens colapsam, outros não) |
| **6. Reconhecimento vs. memorização** | ⭐⭐☆☆☆ Menu apenas textual, sem ícones ou elementos visuais de apoio |
| **7. Flexibilidade e eficiência** | ⭐⭐☆☆☆ Busca genérica sem filtros, usuário precisa ler lista completa de editais |
| **8. Estética e design minimalista** | ⭐⭐☆☆☆ Poluição visual (3 barras navegação, texto denso, espaçamento apertado) |
| **Acessibilidade (WCAG 2.1)** | ⭐⭐⭐☆☆ Ferramentas presentes (A+/A-, Alto Contraste, VLibras), mas contraste padrão insuficiente |

**Justificativa da escolha:** O PROPESP serve como **referência de contexto institucional** e **análise de gap** — identifica exatamente o que precisa ser melhorado. Ao documentar suas limitações (confirmadas pelas frustrações do Prof. Victor no briefing), validamos a necessidade do E-Project e estabelecemos critérios claros de evolução.

---

**Aplicação no E-Project:**
- ✅ **Paleta institucional:** Verde #00663C (cabeçalho) + Cinza #F5F5F5 (fundo) = Familiaridade + Legibilidade
- ✅ **Contraste WCAG AAA:** Texto preto #212121 sobre fundo claro (ratio 16:1) — legível para Prof. Carlos SEM ativar modo especial
- ✅ **Navegação simplificada:** 1 barra superior (logo + busca + perfil) + 1 menu lateral (ícones + texto)
- ✅ **Feed visual de editais:** Cards com badges de status (🟢 Aberto, 🔴 Encerrado) substituem lista textual

---

**Fonte:** Nielsen, J. (1994). *10 Usability Heuristics for User Interface Design*. Nielsen Norman Group | W3C (2018). *Web Content Accessibility Guidelines (WCAG) 2.1*

