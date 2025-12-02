<div align="center">

<h1>MURAL DE INSPIRAÇÃO (MOODBOARD)</h1>

<img src="https://img.shields.io/badge/Disciplina-IHC-003f52?style=for-the-badge&logo=googlescholar&logoColor=white" alt="Disciplina IHC">
<img src="https://img.shields.io/badge/Artefato-Moodboard-008f54?style=for-the-badge&logo=pinterest&logoColor=white" alt="Mural de Inspiração">

<br><br>

> **Conceito Visual e Estético**
> <br>Referências visuais que orientam o estilo, o clima e a estética desejada para a interface, refletindo os sentimentos e experiências que o aplicativo deve transmitir.

</div>

---

## 1. Introdução

Este documento evidencia a inspiração e os sistemas que serviram de base para o **E-Project**. A pesquisa baseou-se em plataformas de educação consolidadas e portais institucionais, pontuando as qualidades de cada interface para implementação no sistema proposto.

O objetivo é alcançar uma tela completa e fluida, alinhada às **Heurísticas de Nielsen**, **Psicologia das Cores** e **Experiência do Usuário (UX)**.

---

## 2. Google Classroom
![Referência](https://img.shields.io/badge/REFERÊNCIA-INTERFACE_&_FLUIDEZ-003f52?style=flat-square)

O Google Classroom é referência global por permitir que professores e alunos realizem tarefas essenciais em **3 cliques ou menos**.

<div align="center">
  <img width="100%" alt="Interface Google Classroom" src="https://github.com/user-attachments/assets/869fff8b-d058-4b7b-9a48-1862f2a4fa95" />
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
  <img width="100%" alt="Portal PROPESP" src="https://github.com/user-attachments/assets/363266f8-6c76-4438-b768-bca2e85958f3" />
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

## 4. Identidade Visual (Logotipo)
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
