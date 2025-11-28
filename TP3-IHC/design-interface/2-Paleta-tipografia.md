# UI Kit e Guia de Estilos - E-Project

Este documento estabelece as diretrizes visuais para o **E-Project**, o Sistema de Gestão de Projetos Acadêmicos. O design foi concebido para transmitir a institucionalidade da UFAM, priorizando rigorosamente a acessibilidade para usuários com baixa visão (Persona: Prof. Carlos) e a clareza de informações (Persona: Prof. Vitor).

---

## 1. Identidade e Naming
* **Nome do Produto:** E-Project
* **Conceito:** Uma ferramenta de gestão centralizada, prática e integrada ao ecossistema acadêmico. O "E" reforça a natureza digital e a eficiência (Electronic/Efficient), enquanto "Project" define o objeto central de trabalho.

---

## 2. Paleta de Cores
A paleta utiliza as cores institucionais (Verde/Amarelo/Azul) modernizadas para garantir alto contraste conforme diretrizes WCAG.

### Cores Principais
| Função | Cor | Código HEX | Aplicação Recomendada |
| :--- | :--- | :--- | :--- |
| **Primária (Brand)** | **Verde UFAM** | `#00663C` | Cabeçalho, Botões Principais, Links ativos. |
| **Secundária (Apoio)** | **Azul Profundo** | `#005875` | Títulos, Elementos de Navegação, Ícones neutros. |
| **Destaque (Accent)** | **Amarelo Solar** | `#FFF700` | Ícones de Favorito, Alertas, Badges de Status. **Atenção:** Usar apenas com texto preto/escuro. |
| **Surface (Fundo)** | **Cinza Gelo** | `#F5F5F5` | Fundo geral das telas (Reduz o brilho visual comparado ao branco puro). |

### Justificativa de Acessibilidade (Contraste)
Para atender à Persona de Acessibilidade (Prof. Carlos), as cores foram testadas contra o fundo branco e cinza:

<img width="589" height="419" alt="image" src="https://github.com/user-attachments/assets/0f089564-a2f7-4fef-8edb-61206aacd787" />


1.  **Verde (#00663C) sobre Branco:** Garante leitura confortável para textos e componentes interativos.
2.  **Azul (#005875) sobre Branco:** Excelente contraste para títulos e leituras que precisam de atenção Maior.
3.  **Amarelo (#FFF700):** Uso para Alto Constrate e fundos com texto preto.

> **Evidência de Teste (WebAIM):**
> 
## 1
> <img width="611" height="762" alt="Paleta Fundo e Cabeçalho" src="https://github.com/user-attachments/assets/132080e3-af1c-4eaf-ba27-dc8f76c257bb" />

## 2
> <img width="618" height="755" alt="Captura de tela 2025-11-27 174947" src="https://github.com/user-attachments/assets/918c544e-2fc1-44c4-a8f2-045678f2fc8f" />


---

## 3. Tipografia
A escolha tipográfica equilibra a seriedade acadêmica com a funcionalidade de um software de gestão.

### Famílias Escolhidas (Google Fonts)
* **Títulos (Display):** **Montserrat**
    * *Motivo:* Geométrica, moderna e robusta. Passa a sensação de estabilidade institucional da UFAM sem parecer antiquada.
* **Corpo de Texto (Body):** **Roboto**
    * *Motivo:* Alta legibilidade em telas, excelente distinção entre caracteres (evita confusão entre "I", "l", "1") e otimizada para interfaces densas (tabelas e listas).

### Escala Tipográfica (Mobile & Desktop)
| Elemento | Fonte | Peso | Tamanho |
| :--- | :--- | :--- | :--- |
| **H1 (Título Página)** | Montserrat | Bold (700) | 24px (Mobile) / 32px (Desk) |
| **H2 (Seções)** | Montserrat | SemiBold (600) | 20px (Mobile) / 24px (Desk) |
| **Body (Padrão)** | Roboto | Regular (400) | **16px** (Mínimo para Acessibilidade) |
| **Legendas/Auxiliar**| Roboto | Medium (500) | 14px |
| **Botões** | Roboto | Bold (700) | 16px (Caixa Alta opcional) |

---

## 4. Ícones e Elementos
* **Biblioteca:** Material Symbols (Google) - Estilo *Rounded*.
* **Consistência:** Ícones sólidos para estados ativos, ícones de linha (outline) para inativos.
* **Regra de Acessibilidade:** Nenhum ícone deve ser utilizado sem um rótulo de texto ou `aria-label` descritivo, garantindo que leitores de tela interpretem a função corretamente.
