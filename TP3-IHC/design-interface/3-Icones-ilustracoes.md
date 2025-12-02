<div align="center">

<h1>BIBLIOTECA DE ÍCONES E ILUSTRAÇÕES - E-PROJECT</h1>

<img src="https://img.shields.io/badge/Biblioteca-Material_Symbols-003f52?style=for-the-badge&logo=googlefonts&logoColor=white">
<img src="https://img.shields.io/badge/Estilo-Rounded_(Arredondado)-008f54?style=for-the-badge&logo=materialdesign&logoColor=white">
<img src="https://img.shields.io/badge/Acessibilidade-WCAG_Compliance-003f52?style=for-the-badge&logo=accessibility&logoColor=white">

<br><br>

> **Padrões Iconográficos**
> <br>Definição dos padrões iconográficos para garantir consistência visual e acessibilidade para o E-Project.
> **Fonte Oficial:** [Google Fonts Icons](https://fonts.google.com/icons)

<br>
</div>

---

## 1. Biblioteca Escolhida
![Padronização](https://img.shields.io/badge/PADRÃO-GOOGLE_MATERIAL_SYMBOLS-003f52?style=flat-square)

Optamos pela biblioteca **Material Symbols**, no estilo **Rounded** (Arredondado).

* **Estilo Ativo:** Preenchido (Filled).
* **Estilo Inativo:** Contorno (Outlined).

<div align="center">
  <img width="80%" alt="Exemplo de Icones" src="https://github.com/user-attachments/assets/cb1e8c8e-167f-4fcb-b483-e8140bc8b6cd" />
  <br>
</div>

### Justificativa de Escolha
1.  **Coerência Visual:** A geometria dos ícones harmoniza com a tipografia **Roboto** e **Montserrat** utilizadas no projeto.
2.  **Familiaridade (Heurística de Nielsen):** Sendo o padrão do Google/Android, reduz a curva de aprendizado para os alunos.
3.  **Legibilidade:** Desenhados em grids de pixels, garantindo clareza mesmo em telas mobile de baixa resolução.

---

## 2. Ícones Principais do Sistema
![Semântica](https://img.shields.io/badge/SEMÂNTICA-NAVEGAÇÃO_E_AÇÃO-008f54?style=flat-square)

Abaixo, listamos os ícones semânticos que representarão as principais funcionalidades do E-Project.

| Visualização | Nome (Google Fonts) | Significado no E-Project |
| :---: | :--- | :--- |
| <img width="24" height="24" src="https://github.com/user-attachments/assets/5dc2e4d4-7a41-41e8-a83c-d134bfd7c4ac" /> | **`home`** | **Dashboard/Início:** Visão geral do sistema. |
| <img width="24" height="24" src="https://github.com/user-attachments/assets/cf4ec748-6e78-41b1-a2b4-533bd8e7dbc4" /> | **`folder_open`** | **Meus Projetos:** Acesso aos projetos PIBIC/PACE. |
| <img width="24" height="24" src="https://github.com/user-attachments/assets/294acd6b-da9e-466c-958f-5028ecdef299" /> | **`source_notes`** | **Editais:** Feed unificado de oportunidades. |
| <img width="24" height="24" src="https://github.com/user-attachments/assets/960035f0-9559-46f1-a418-ae0b9a0eac94" /> | **`description`** | **Documentos:** Geração de relatórios e cartas. |
| <img width="24" height="24" src="https://github.com/user-attachments/assets/13cee9d3-6fd6-45a9-b822-91d048ef7f72" /> | **`person`** | **Perfil:** Dados do usuário e configurações. |
| <img width="24" height="24" src="https://github.com/user-attachments/assets/0a4c9b82-c1d5-4e59-b26c-856a9024b255" /> | **`visibility`** | **Acessibilidade:** Menu de contraste e fonte. |

<div align="center">
  <sub><b>Figura 2:</b> Conjunto de ícones selecionados para a navegação global. (Fonte: Google Fonts / Elaboração própria) [cite_start][cite: 68]</sub>
</div>

---

## 3. Diretrizes de Uso e Acessibilidade
![Diretrizes](https://img.shields.io/badge/REGRAS-ACESSIBILIDADE_VISUAL-003f52?style=flat-square)

Para garantir a inclusão da persona **Prof. Carlos (Baixa Visão)**, estabelecemos regras estritas de aplicação:

### A. Regra do Rótulo Obrigatório
**Nenhum ícone deve aparecer sozinho.** Todo ícone deve ser acompanhado de um rótulo textual visível para garantir a comunicabilidade e reduzir a ambiguidade.
* ❌ *Incorreto:* Apenas um ícone de "Lixeira".
* ✅ *Correto:* Ícone de "Lixeira" com o texto "Excluir" ao lado ou abaixo.

### B. Tamanho do Alvo (Lei de Fitts)
Em dispositivos móveis, a área de toque mínima deve ser de **48x48dp**, mesmo que o ícone visualmente seja menor (ex: 24px), garantindo facilidade de clique para usuários com dificuldades motoras.

### C. Contraste Cromático
Os ícones devem seguir rigorosamente a paleta de cores para garantir contraste suficiente:
* **Ação/Navegação:** Verde UFAM (`#00663C`) ou Azul Profundo (`#005875`).
* **Alerta:** Amarelo (`#FFF700`) - sempre utilizado com contorno escuro ou fundo contrastante para legibilidade.
