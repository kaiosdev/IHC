<div align="center">

<h1>MURAL DE INSPIRAÇÃO (MOODBOARD)</h1>

<img src="https://img.shields.io/badge/Disciplina-IHC-003f52?style=for-the-badge&logo=googlescholar&logoColor=white" alt="Disciplina IHC">
<img src="https://img.shields.io/badge/Artefato-Moodboard-008f54?style=for-the-badge&logo=pinterest&logoColor=white" alt="Mural de Inspiração">

<br><br>

> **Conceito Visual e Estético**
> <br>Referências visuais que orientam o estilo, o clima e a estética desejada para a interface, refletindo os sentimentos e experiências que o aplicativo deve transmitir.

</div>

---
<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1CXAGMnd4XSkg1B3wSyyWtP_NaTs2Ol5O" width="100%">
</div>

## 1. Introdução

Este documento evidencia a inspiração e os sistemas que serviram de base para o **E-Project**. A pesquisa baseou-se em plataformas de educação consolidadas e portais institucionais, pontuando as qualidades de cada interface para implementação no sistema proposto.

O objetivo é alcançar uma tela completa e fluida, alinhada às **Heurísticas de Nielsen**, **Psicologia das Cores** e **Experiência do Usuário (UX)**.

---

## 2. Google Classroom
![Referência](https://img.shields.io/badge/REFERÊNCIA-INTERFACE_&_FLUIDEZ-003f52?style=flat-square)

O Google Classroom é referência global por permitir que professores e alunos realizem tarefas essenciais em **3 cliques ou menos**.

<div align="center">
  <img width="90%" alt="Interface Google Classroom" src="https://github.com/user-attachments/assets/869fff8b-d058-4b7b-9a48-1862f2a4fa95" />
  <br>
  <sub><b>Figura 1:</b> Interface de gestão de turmas do Google Classroom. (Fonte: Google for Education, 2024)</sub>
</div>

### 🧩 Por que escolhemos como inspiração?

* **Gestão Visual:** Uso de Cards visuais para representar cada turma/disciplina.
* **Navegação:** Menu lateral fixo com hierarquia clara (Título → Professor → Datas).
* **Minimalismo:** Interface prioriza o conteúdo, dispensando manuais ou treinamentos complexos.
* **Paleta Neutra:** Fundo branco/cinza que destaca apenas o conteúdo pedagógico.

### 🏆 Avaliação Heurística (Nielsen)

| Heurística | Avaliação no Classroom | Aplicação no E-Project |
| :--- | :--- | :--- |
| **1. Visibilidade do estado** | ⭐⭐⭐⭐⭐ Menu lateral destaca seção ativa. | Menu lateral persistente indicando onde o usuário está. |
| **2. Correspondência** | ⭐⭐⭐⭐⭐ Metáfora de "sala de aula" e "mural". | Uso de termos acadêmicos (Turma, Edital, Projeto). |
| **4. Consistência** | ⭐⭐⭐⭐⭐ Todos os cards seguem o mesmo padrão. | Padronização dos cards de editais e projetos. |
| **6. Reconhecimento** | ⭐⭐⭐⭐⭐ Ícones + texto para reduzir carga cognitiva. | Uso de ícones universais (download, upload, calendário). |
| **8. Estética Minimalista** | ⭐⭐⭐⭐⭐ Foco no essencial, sem poluição. | Layout limpo para evitar distrações (Foco na tarefa). |

---

## 3. Portal PROPESP/UFAM
![Referência](https://img.shields.io/badge/REFERÊNCIA-INSTITUCIONAL_&_IDENTIDADE-008f54?style=flat-square)

O Portal oficial da Pró-Reitoria de Pesquisa e Pós-Graduação representa a **identidade visual oficial** que professores e alunos já conhecem.

<div align="center">
  <img width="90%" alt="Portal PROPESP" src="https://github.com/user-attachments/assets/363266f8-6c76-4438-b768-bca2e85958f3" />
  <br>
  <sub><b>Figura 2:</b> Página inicial do Portal PROPESP. (Fonte: Portal da UFAM, 2024)</sub>
</div>

### ⚖️ Análise Crítica: O que manter e o que melhorar?

#### ✅ Pontos Fortes (Manter)
1.  **Familiaridade Institucional:** A paleta verde oficial (`#00663C`) cria reconhecimento imediato.
2.  **Conformidade Legal:** Segue diretrizes do e-MAG e Governo Federal.
3.  **Ferramentas de Acessibilidade:** Botões de contraste e VLibras integrados.

#### ⚠️ Pontos Fracos (Melhorar no E-Project)
1.  **Navegação Confusa:** Menu baseado em organograma burocrático, não em tarefas do usuário.
2.  **Densidade Visual:** Texto muito pequeno e espaçamento apertado.
3.  **Contraste Padrão:** O modo "normal" do site possui falhas de contraste em textos secundários.

### 🔍 Diagnóstico de Contraste (Problema vs. Solução)

| Elemento | Problema no Portal Atual | Solução no E-Project |
| :--- | :--- | :--- |
| **Corpo do texto** | Cinza médio sobre branco (Difícil leitura) | **Preto (#212121)** sobre branco (Alto contraste). |
| **Metadados** | Cinza claro (Falha WCAG < 4.5:1) | **Cinza Escuro** com ratio 4.5:1 garantido. |
| **Acessibilidade** | Opcional (usuário precisa ativar) | **Nativa** (o design padrão já é acessível). |

---

## 4. Notion - Referência de Design
<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1Y9KjPjjpsLcg4ZHAuFIPKX2bqRQ4LyT_" width="50%">
</div>

## Introdução

O Notion é uma plataforma de produtividade "all-in-one" lançada em 2016, que integra notas, bases de dados, gerenciamento de projetos, wikis e colaboração em um único espaço de trabalho modular. Tornou-se referência em flexibilidade de interface e personalização, sendo amplamente adotado por equipes acadêmicas, startups e empresas para organização de conhecimento e projetos.

## Funcionalidades Principais

- Páginas Aninhadas: Estrutura hierárquica infinita (páginas dentro de páginas)
- Blocos Modulares: Texto, tabelas, kanban, calendários, galerias, embeds
- Bases de Dados: Visualizações múltiplas (tabela, quadro, linha do tempo, calendário)
- Templates: Bibliotecas prontas para casos de uso (gestão de projetos, notas de aula)
- Colaboração: Edição em tempo real, comentários, menções, histórico de versões
- Integração: API aberta para conectar com outras ferramentas

## Interface

Layout:
- Barra lateral expansível com navegação por páginas/workspaces
- Área de conteúdo "canvas" infinitamente personalizável
- Paleta minimalista: Fundo branco/bege, textos em cinza escuro, acentos em azul
- Tipografia legível: Inter/System UI em 16px base, hierarquia clara de títulos

Organização:
- Estrutura de blocos: Cada elemento (texto, imagem, tabela) é um bloco arrastável
- Menu "/" (slash): Comando rápido para inserir qualquer tipo de conteúdo
- Breadcrumb clicável: Navegação por caminho de páginas aninhadas
- Visualizações dinâmicas: Mesma base de dados pode ser vista como lista, kanban, calendário

## Conclusão

O Notion representa design baseado em composição: em vez de oferecer uma interface rígida, permite que usuários construam sua própria experiência combinando blocos modulares. Sua força está na flexibilidade sem sacrificar simplicidade — iniciantes criam páginas de notas básicas em segundos, enquanto avançados constroem sistemas complexos de CRM ou gestão de projetos.

Para o E-Project, o Notion valida três conceitos críticos:

1. Visualizações múltiplas: Mesmos dados (projetos PIBIC) podem ser vistos como cards, lista ou timeline — adaptando-se a diferentes perfis de usuário (Prof. Victor prefere cards, Prof. Carlos prefere lista com texto grande)

2. Hierarquia flexível: Páginas aninhadas inspiram a estrutura "Dashboard → Projeto → Tarefas → Subtarefas" modelada nos HTAs do E-Project

3. Templates contextuais: Em vez de "tela em branco", oferecer modelos prontos ("Novo Projeto PIBIC", "Relatório Mensal") reduz fricção — especialmente para Ana Beatriz (Persona 2) que tem medo de "fazer errado"

Limitação identificada: A flexibilidade excessiva pode confundir usuários não técnicos (Prof. Carlos poderia se perder em menus de configuração). O E-Project adota o meio-termo: estrutura pré-definida (como Classroom) com personalização controlada (filtros, visualizações) — não requer que usuários "construam" o sistema do zero.

## Referências nas Heurísticas de Nielsen

Esta análise baseia-se nas 10 Heurísticas de Usabilidade de Nielsen (1994), utilizadas para avaliar a qualidade da interface:

Heurística 1 - Visibilidade do estado do sistema: Breadcrumb mostra localização, mas pode confundir em hierarquias profundas

Heurística 2 - Correspondência sistema-mundo real: Metáfora de "página/caderno", menu "/" intuitivo

Heurística 3 - Controle e liberdade do usuário: Desfazer ilimitado, blocos arrastáveis, histórico completo

Heurística 4 - Consistência e padrões: Todos os blocos seguem mesma lógica de interação

Heurística 6 - Reconhecimento vs. memorização: Menu "/" ajuda, mas usuários precisam aprender comandos

Heurística 7 - Flexibilidade e eficiência: Atalhos de teclado extensivos, templates aceleram criação

Heurística 8 - Estética e design minimalista: Interface limpa, foco no conteúdo, zero elementos decorativos

Justificativa da escolha: O Notion demonstra que flexibilidade controlada não compromete usabilidade quando bem implementada. Com mais de 30 milhões de usuários (Notion, 2024), prova que interfaces modulares podem escalar de uso pessoal a empresarial. Sua arquitetura de "blocos + visualizações" inspira o sistema de filtros e múltiplas views do E-Project.

Aplicação no E-Project:
- Visualizações alternativas: Dashboard com toggle "Cards / Lista / Timeline"
- Templates pré-configurados: "Novo Projeto PIBIC" já vem com campos obrigatórios
- Breadcrumb navegável: "Início > Meus Projetos > PIBIC Física > Relatório Mensal"
- Limite de personalização: Usuários NÃO podem "destruir" estrutura base (diferente do Notion) — garantindo que Prof. Carlos não se perca

Fonte: Nielsen, J. (1994). 10 Usability Heuristics for User Interface Design. Nielsen Norman Group.

## 5. Identidade Visual (Logotipo)
![Referência](https://img.shields.io/badge/INSPIRAÇÃO-SEMÂNTICA_&_MARCA-003f52?style=flat-square)

A marca do E-Project busca a **continuidade semântica** com a UFAM, garantindo que o sistema seja percebido como uma ferramenta oficial e confiável.

<div align="center">
  <img width="100%" alt="Inspiração Logo UFAM" src="https://github.com/user-attachments/assets/14fd4ebc-39fb-47af-b8c0-d80d1d9d875f" />
  <br>
  <sub><b>Figura 3:</b> Estudo de identidade visual baseado no brasão da UFAM. (Fonte: Elaboração própria baseada na marca da UFAM)</sub>
</div>

### 🎨 Construção da Identidade

* **Símbolos Mantidos:** Formato circular e os louros (símbolos de excelência acadêmica e tradição).
* **Evolução:** Substituição da pomba clássica por um **livro aberto com engrenagem e checkmark**, simbolizando a gestão prática de projetos.
* **Cores:** Uso do **Verde (#00663C)** para preservar a coerência institucional.
* **Objetivo:** Eliminar a barreira de adoção. Ao ver o logo, o professor deve pensar: *"Este sistema pertence à UFAM, é oficial, posso confiar"*.

---
<div align="center">
<sub>Documentação de Design de Interface • Atualizado em 2025</sub>
</div>
