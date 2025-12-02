<div align="center">

<h1>UI KIT E GUIA DE ESTILOS - E-PROJECT</h1>

<img src="https://img.shields.io/badge/Instituição-UFAM-003f52?style=for-the-badge&logo=googlescholar&logoColor=white">
<img src="https://img.shields.io/badge/Artefato-UI_Kit_&_Design-008f54?style=for-the-badge&logo=figma&logoColor=white">
<img src="https://img.shields.io/badge/Foco-Acessibilidade-003f52?style=for-the-badge&logo=accessibility&logoColor=white">

<br><br>

> **Diretrizes Visuais**
> <br>Este documento estabelece as diretrizes visuais para o **E-Project**, o Sistema de Gestão de Projetos Acadêmicos. Design focado na institucionalidade e acessibilidade (Personas: Prof. Carlos e Prof. Vitor).

<br>

<a href="LINK-DO-SEU-PROJETO-AQUI">
  <img src="https://img.shields.io/badge/🔗_ACESSAR_GUIA_DE_ESTILOS-008f54?style=for-the-badge">
</a>

</div>

---

## 1. Identidade e Naming
* **Nome do Produto:** E-Project
* **Conceito:** Uma ferramenta de gestão centralizada, prática e integrada ao ecossistema acadêmico. O "E" reforça a natureza digital e a eficiência (Electronic/Efficient), enquanto "Project" define o objeto central de trabalho.

---

## 2. Paleta de Cores
A paleta utiliza as cores institucionais modernizadas. A escolha do preto puro para textos e do branco para superfícies garante a máxima taxa de contraste possível.

### Cores Institucionais e de Marca
| Função | Cor | Código HEX | Aplicação Recomendada |
| :--- | :--- | :---: | :--- |
| **Primária (Brand)** | **Verde UFAM** | `#00663C` | Cabeçalho, Botões Principais, Links ativos. |
| **Secundária (Apoio)** | **Azul Profundo** | `#005875` | Títulos de seções, Ícones de navegação. |
| **Destaque (Accent)** | **Amarelo Solar** | `#FFF700` | Favoritos, Alertas e Badges de Status. |

> ⚠️ **Atenção:** O Amarelo Solar deve ser usado sempre com texto **Preto (`#000000`)** para garantir leitura.

### Cores Neutras (Superfície e Texto)
| Função | Cor | Código HEX | Aplicação Recomendada |
| :--- | :--- | :---: | :--- |
| **Texto Principal** | **Preto Absoluto** | `#000000` | Todo o corpo de texto, títulos e rótulos. |
| **Surface (Cartões)** | **Branco Puro** | `#FFFFFF` | Fundo de cartões (Cards) e formulários. |
| **Background**| **Cinza Gelo** | `#F5F5F5` | Fundo geral da página (atrás dos cartões). |

<br>

### Justificativa de Acessibilidade (Contraste WCAG)
Para atender à Persona de Acessibilidade (**Prof. Carlos**), as cores foram validadas para garantir contraste máximo:

<div align="center">
  <img width="800" alt="Resumo de Cores" src="https://github.com/user-attachments/assets/35652974-256a-4f34-a77e-ca1bfc20e2c0" />
</div>

1.  **Verde (#00663C) sobre Branco:** Contraste suficiente para botões e cabeçalhos.
2.  **Azul (#005875) sobre Branco:** Excelente contraste para leitura.
3.  **Preto (#000000) sobre Branco:** Contraste máximo (**21:1**), ideal para dados críticos.

#### Evidência de Teste (WebAIM)

<div align="center">
  <table>
    <tr>
      <td align="center"><strong>Teste 1: Fundo e Cabeçalho</strong></td>
      <td align="center"><strong>Teste 2: Botões e Destaques</strong></td>
    </tr>
    <tr>
      <td><img width="400" alt="Teste WebAIM 1" src="https://github.com/user-attachments/assets/132080e3-af1c-4eaf-ba27-dc8f76c257bb"></td>
      <td><img width="400" alt="Teste WebAIM 2" src="https://github.com/user-attachments/assets/918c544e-2fc1-44c4-a8f2-045678f2fc8f"></td>
    </tr>
  </table>
</div>

---

## 3. Tipografia
A escolha tipográfica equilibra a seriedade acadêmica com a funcionalidade de um software de gestão.

### Famílias Escolhidas (Google Fonts)
* **Títulos (Display): Montserrat**
    * *Motivo:* Geométrica, moderna e robusta. Passa a sensação de estabilidade institucional da UFAM.
* **Corpo de Texto (Body): Roboto**
    * *Motivo:* Alta legibilidade em telas, excelente distinção entre caracteres (evita confusão entre "I", "l", "1").

### Escala Tipográfica (Mobile & Desktop)
| Elemento | Fonte | Peso | Tamanho (px) |
| :--- | :--- | :---: | :--- |
| **H1 (Título Página)** | Montserrat | Bold (700) | 24px (Mob) / 32px (Desk) |
| **H2 (Seções)** | Montserrat | SemiBold (600) | 20px (Mob) / 24px (Desk) |
| **Body (Padrão)** | Roboto | Regular (400) | **16px** (Acessibilidade) |
| **Legendas**| Roboto | Medium (500) | 14px |
| **Botões** | Roboto | Bold (700) | 16px |

---

## 4. Ícones e Elementos
* **Biblioteca:** Material Symbols (Google) - Estilo *Rounded*.
* **Consistência:** Ícones sólidos (Filled) para ativos, linha (Outline) para inativos.
* **Regra de Acessibilidade:** Nenhum ícone deve ser utilizado sem um rótulo de texto ou `aria-label` descritivo.
