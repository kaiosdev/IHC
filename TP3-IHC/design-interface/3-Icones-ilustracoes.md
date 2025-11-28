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

| Ícone (Nome Google) | Significado no E-Project |
| :--- | :--- |
| **`home`** | **Dashboard/Início:** Visão geral do sistema. |
| **`folder_open`** | **Meus Projetos:** Acesso aos projetos de PIBIC/PACE cadastrados. |
| **`feed`** | **Editais:** Feed unificado de oportunidades (Propesp/Proext). |
| **`description`** | **Documentos:** Área de geração de relatórios e cartas. |
| **`person`** | **Perfil:** Dados do usuário e configurações de conta. |
| **`visibility`** | **Acessibilidade:** Menu de alto contraste e tamanho de fonte. |

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
