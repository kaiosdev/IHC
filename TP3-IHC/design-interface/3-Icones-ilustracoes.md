# Biblioteca de Ícones e Ilustrações - E-Project

## 1. Biblioteca Escolhida
Optamos pela biblioteca **Material Symbols**, no estilo **Rounded** (Arredondado).

* **Fonte:** [Google Fonts Icons](https://fonts.google.com/icons)
* **Estilo:** Preenchido (Filled) para estados ativos e Contorno (Outlined) para estados inativos.

### Justificativa de Escolha
1.  **Coerência Visual:** A geometria dos ícones Material Symbols "Rounded" harmoniza perfeitamente com a tipografia **Roboto** e **Montserrat** escolhida para o projeto.
2.  **Familiaridade (Heurística de Nielsen):** Sendo a biblioteca padrão do Android e produtos Google, os ícones (como a Lupa para busca ou a Casa para Home) são universalmente reconhecidos pelos usuários, reduzindo a curva de aprendizado.
3.  **Legibilidade:** Os ícones são desenhados em grids de pixels, garantindo clareza mesmo em tamanhos pequenos (telas mobile).

---

## 2. Ícones Principais do Sistema
Abaixo, listamos os ícones semânticos que representarão as principais funcionalidades do E-Project:

| Visualização | Nome (Google Fonts) | Significado no E-Project |
| :---: | :--- | :--- |
|  Home <img width="24" height="24" alt="home_24dp_FFFFFF_FILL0_wght400_GRAD0_opsz24" src="https://github.com/user-attachments/assets/5dc2e4d4-7a41-41e8-a83c-d134bfd7c4ac" /> | **`home`** | **Dashboard/Início:** Visão geral do sistema. |
| Projetos <img width="24" height="24" alt="folder_24dp_FFFFFF_FILL0_wght400_GRAD0_opsz24" src="https://github.com/user-attachments/assets/cf4ec748-6e78-41b1-a2b4-533bd8e7dbc4" /> | **`folder_open`** | **Meus Projetos:** Acesso aos projetos de PIBIC/PACE cadastrados. |
| Editais <img width="24" height="24" alt="source_notes_24dp_FFFFFF_FILL0_wght400_GRAD0_opsz24" src="https://github.com/user-attachments/assets/294acd6b-da9e-466c-958f-5028ecdef299" /> | **`Source Notes`** | **Editais:** Feed unificado de oportunidades (Propesp/Proext). |
| Docs <img width="24" height="24" alt="docs_24dp_FFFFFF_FILL0_wght400_GRAD0_opsz24" src="https://github.com/user-attachments/assets/960035f0-9559-46f1-a418-ae0b9a0eac94" /> | **`description`** | **Documentos:** Área de geração de relatórios e cartas. |
| Perfil <img width="24" height="24" alt="person_24dp_FFFFFF_FILL0_wght400_GRAD0_opsz24" src="https://github.com/user-attachments/assets/13cee9d3-6fd6-45a9-b822-91d048ef7f72" /> | **`person`** | **Perfil:** Dados do usuário e configurações de conta. |
| Acessibilidade <img width="24" height="24" alt="visibility_24dp_FFFFFF_FILL0_wght400_GRAD0_opsz24" src="https://github.com/user-attachments/assets/d7737943-2077-4801-b509-a0c4734b2925" /> | **`visibility`** | **Acessibilidade:** Menu de alto contraste e tamanho de fonte. |

> *Nota: As imagens acima são exemplos no estilo Rounded.*

---

## 3. Diretrizes de Uso e Acessibilidade

Para garantir que a interface seja inclusiva para a persona **Prof. Carlos (Baixa Visão)**, estabelecemos as seguintes regras estritas para o uso de ícones:

### A. Regra do Rótulo Obrigatório
**Nenhum ícone deve aparecer sozinho.** Todo ícone deve ser acompanhado de um rótulo textual visível.
* *Incorreto:* Apenas um ícone de "Lixeira".
* *Correto:* Ícone de "Lixeira" com o texto "Excluir" ao lado ou abaixo.
* *Motivo:* Garante a comunicabilidade inequívoca da função e auxilia leitores de tela.

### B. Tamanho do Alvo (Lei de Fitts)
Em dispositivos móveis, os ícones que funcionam como botões devem ter uma área de toque mínima de **48x48dp**, mesmo que o desenho do ícone seja menor (ex: 24px).

### C. Contraste
Os ícones devem seguir a paleta de cores definida:
* **Ícones de Ação/Navegação:** Verde UFAM (`#00663C`) ou Azul Profundo (`#005875`).
* **Ícones de Alerta:** Amarelo (`#FFF700`) - sempre com contorno escuro ou fundo escuro para contraste.
