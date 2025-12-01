<div align="center">

<h1>UI Kit e Guia de Estilos - E-Project</h1>

<img src="https://img.shields.io/badge/Instituição-UFAM-00663C?style=for-the-badge&logo=googlescholar&logoColor=white">

<img src="https://img.shields.io/badge/Artefato-UI_Kit_&_Design-00663C?style=for-the-badge&logo=figma&logoColor=white">

<img src="https://img.shields.io/badge/Foco-Acessibilidade-00663C?style=for-the-badge&logo=accessibility&logoColor=white">

<br><br>

> Este documento estabelece as diretrizes visuais para o **E-Project**, o Sistema de Gestão de Projetos Acadêmicos.
> Design focado na institucionalidade e acessibilidade (Personas: Prof. Carlos e Prof. Vitor).

<br>

<a href="LINK-DO-SEU-PROJETO-AQUI">
  <img src="https://img.shields.io/badge/🔗_ACESSAR_GUIA_DE_ESTILOS-00663C?style=for-the-badge">
</a>

</div>

# UI Kit e Guia de Estilos - E-Project

Este documento estabelece as diretrizes visuais para o **E-Project**, o Sistema de Gestão de Projetos Acadêmicos. O design foi concebido para transmitir a institucionalidade da UFAM, priorizando rigorosamente a acessibilidade para usuários com baixa visão (Persona: Prof. Carlos) e a clareza de informações.

---

## 1. Identidade e Naming
* **Nome do Produto:** E-Project
* **Conceito:** Uma ferramenta de gestão centralizada, prática e integrada ao ecossistema acadêmico. O "E" reforça a natureza digital e a eficiência (Electronic/Efficient), enquanto "Project" define o objeto central de trabalho.

---

## 2. Paleta de Cores
A paleta utiliza as cores institucionais modernizadas. A escolha do preto puro para textos e do branco para superfícies garante a máxima taxa de contraste possível.

### Cores Institucionais e de Marca
| Função | Cor | Código HEX | Aplicação Recomendada |
| :--- | :--- | :--- | :--- |
| **Primária (Brand)** | **Verde UFAM** | `#00663C` | Cabeçalho, Botões Principais, Links ativos. |
| **Secundária (Apoio)** | **Azul Profundo** | `#005875` | Títulos de seções, Ícones de navegação, Elementos de suporte. |
| **Destaque (Accent)** | **Amarelo Solar** | `#FFF700` | Ícones de Favorito, Alertas, Badges de Status. **Atenção:** Usar sempre com texto Preto (`#000000`). |

### Cores Neutras (Superfície e Texto)
| Função | Cor | Código HEX | Aplicação Recomendada |
| :--- | :--- | :--- | :--- |
| **Texto Principal** | **Preto Absoluto** | `#000000` | Todo o corpo de texto, títulos e rótulos para contraste máximo (AAA). |
| **Surface (Cartões)** | **Branco Puro** | `#FFFFFF` | Fundo de cartões (Cards), áreas de conteúdo e campos de formulário. |
| **Background (Fundo)**| **Cinza Gelo** | `#F5F5F5` | Fundo geral da página (atrás dos cartões) para criar profundidade e descanso visual. |

### Justificativa de Acessibilidade (Contraste WCAG)
Para atender à Persona de Acessibilidade (Prof. Carlos), as cores foram validadas:

<img width="1013" height="622" alt="image" src="https://github.com/user-attachments/assets/35652974-256a-4f34-a77e-ca1bfc20e2c0" />

1.  **Verde (#00663C) sobre Branco:** Contraste suficiente para botões e cabeçalhos legíveis.
2.  **Azul (#005875) sobre Branco:** Excelente contraste para leitura.
3.  **Preto (#000000) sobre Branco:** Contraste máximo (21:1), ideal para leitura de textos longos e dados críticos.
4.  **Amarelo (#FFF700):** Utilizado exclusivamente como fundo para texto preto ou como ícone gráfico, garantindo visibilidade sem comprometer a leitura.

> **Evidência de Teste (WebAIM):**
>
> ## 1
> <img width="611" height="762" alt="Paleta Fundo e Cabeçalho" src="https://github.com/user-attachments/assets/132080e3-af1c-4eaf-ba27-dc8f76c257bb" />
>
> ## 2 
> <img width="618" height="755" alt="Captura de tela 2025-11-27 174947" src="https://github.com/user-attachments/assets/918c544e-2fc1-44c4-a8f2-045678f2fc8f" />


---

## 3. Tipografia
A escolha tipográfica equilibra a seriedade acadêmica com a funcionalidade de um software de gestão.

### Famílias Escolhidas (Google Fonts)
* **Títulos (Display):** **Montserrat**
    * *Motivo:* Geométrica, moderna e robusta. Passa a sensação de estabilidade institucional da UFAM sem parecer antiquada.
* **Corpo de Texto (Body):** **Roboto**
    * *Motivo:* Alta legibilidade em telas, excelente distinção entre caracteres (evita confusão entre "I", "l", "1") e otimizada para interfaces densas.

### Escala Tipográfica (Mobile & Desktop)
| Elemento | Fonte | Peso | Tamanho |
| :--- | :--- | :--- | :--- |
| **H1 (Título Página)** | Montserrat | Bold (700) | 24px (Mobile) / 32px (Desk) |
| **H2 (Seções)** | Montserrat | SemiBold (600) | 20px (Mobile) / 24px (Desk) |
| **Body (Padrão)** | Roboto | Regular (400) | **16px** (Mínimo para Acessibilidade) |
| **Legendas/Auxiliar**| Roboto | Medium (500) | 14px |
| **Botões** | Roboto | Bold (700) | 16px |

---

## 4. Ícones e Elementos
* **Biblioteca:** Material Symbols (Google) - Estilo *Rounded*.
* **Consistência:** Ícones sólidos para estados ativos, ícones de linha (outline) para inativos.
* **Regra de Acessibilidade:** Nenhum ícone deve ser utilizado sem um rótulo de texto ou `aria-label` descritivo, garantindo que leitores de tela interpretem a função corretamente.
