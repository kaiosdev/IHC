<div align="center">

# 📱 Interface Mobile - Fluxo do Aluno (PIBIC)

<p align="center">
  <a href="#-visão-geral-do-fluxo">Visão Geral</a> •
  <a href="#-tarefas-acadêmicas">Tarefas Acadêmicas</a> •
  <a href="#-rotina-administrativa">Rotina Admin</a> •
  <a href="#-acessibilidade-e-feedback">Acessibilidade</a>
</p>

---

### 🎯 Persona em Foco

> **👩‍🎓 Ana Beatriz** | Estudante de Engenharia & Bolsista PIBIC
>
> **Dores Principais:** Sobrecarga cognitiva por múltiplas tarefas e ansiedade na comunicação com orientador.
> **Solução Mobile:** Foco em organização rápida, feedback imediato e submissões guiadas.

</div>

---

## 📸 Visão Geral do Fluxo

Este módulo centraliza a rotina da Ana, desde a priorização de tarefas até a submissão de arquivos complexos com comunicação integrada.

| 1. Dashboard e Priorização | 2. Submissão Integrada (Upload + Chat) |
| :---: | :---: |
| Foco na redução de ansiedade com card de destaque para prazos urgentes e lista com áreas de toque expandidas. | Centraliza o envio do arquivo e a mensagem de status ao orientador em uma única tela. |
| <img src="https://github.com/user-attachments/assets/b6fefac4-7730-46e5-84dc-3ff3aa0dd2f6" width="280" alt="Dashboard" /> | <img src="https://github.com/user-attachments/assets/c0784aff-d239-4d6a-b9fc-7b135aefee21" width="280" alt="Upload" /> |

<br>

### 🚦 Feedback do Sistema
Feedback visual claro é essencial para reduzir a insegurança da aluna.

| ✅ Sucesso (Tranquilizador) | ⚠️ Erro (Acionável) |
| :---: | :---: |
| Confirmação verde e mensagem positiva. | Instrução clara de correção para evitar frustração. |
| <img src="https://github.com/user-attachments/assets/f3602ce5-2fec-45ba-92de-8121a8e3e812" width="250" alt="Sucesso" /> | <img src="https://github.com/user-attachments/assets/fa57e469-ada6-44d1-8fa6-08564fe11a94" width="250" alt="Erro" /> |

---

## 📚 Tarefas Acadêmicas

Fluxos detalhados para revisão de conteúdo e submissão final de artigos, com travas de segurança (WCAG 3.3.4).

| 4. Revisão de Apresentação | 5. Envio de Artigo Definitivo |
| :---: | :---: |
| Acesso rápido aos materiais e feedback do professor com botões de alto contraste. | Checklist obrigatório que habilita o botão de envio apenas após cumprimento dos requisitos. |
| <img src="https://github.com/user-attachments/assets/ca4df9e8-e754-4fde-b2fb-d479b97e0875" width="280" alt="Revisão" /> | <img src="https://github.com/user-attachments/assets/b306d8fe-9fb6-473a-8299-1b44de608175" width="280" alt="Artigo" /> |

---

## 🏛️ Rotina Administrativa

Funcionalidades de dia a dia focadas em rapidez e conformidade.

| 6. Check-in de Presença | 7. Relatório de Estágio |
| :---: | :---: |
| Ação imediata com validação visual de geolocalização. | Fluxo segmentado com múltiplos uploads (Principal + Anexo) e checklist de requisitos. |
| <img src="https://github.com/user-attachments/assets/fe9ea190-e5de-4762-9e2b-1374761ef772" width="280" alt="Presença" /> | <img src="https://github.com/user-attachments/assets/d15c76ee-bbd8-4bf6-89c6-a1270ea408bb" width="280" alt="Estágio" /> |

---

## ♿ Acessibilidade e Feedback

Implementação rigorosa das diretrizes WCAG para tornar a interface inclusiva.

| 8. Painel de Configurações WCAG | Confirmação Pós-Ação |
| :---: | :---: |
| Controles para Visão (Contraste 7:1, Tamanho de Fonte), Motora (Área de toque 44px+) e Cognitiva. | Feedback universal de conclusão de tarefa. |
| <img src="https://github.com/user-attachments/assets/24d5a9cf-cf5d-4865-8288-413ca19708b7" width="280" alt="Acessibilidade" /> | <img src="https://github.com/user-attachments/assets/52e5ff4e-aa91-4d51-bfa7-c8d986b3857b" width="280" alt="Confirmação" /> |

---

<div align="center">

### 🎨 Design System Mobile

Mantendo consistência estrita com a versão Desktop.

| Cor Primária (Verde UFAM) | Cor de Erro/Alerta |
| :---: | :---: |
| ![#1B5E20](https://via.placeholder.com/150x50/1B5E20/ffffff?text=HEX+%231B5E20) | ![#D32F2F](https://via.placeholder.com/150x50/D32F2F/ffffff?text=HEX+%23D32F2F) |
| Ações principais, sucesso e identidade. | Avisos urgentes, erros e exclusões. |

## Módulo de Acessibilidade (WCAG)
Este módulo demonstra o compromisso do projeto com a inclusão, permitindo que o usuário personalize a interface.

### ⚙️ Painel de Configurações
<div align="center">
  <img src="https://github.com/user-attachments/assets/b9a858b4-2e07-4c98-a4ea-504cf0ed1355" width="300" alt="Tela de Configurações de Acessibilidade" />
</div>

**Função:** Central de controle para adaptação da interface.
* **Visualização:** Slider para ajuste de tamanho de fonte e *toggles* para Alto Contraste e Modo Escuro (focando em baixa visão e fotofobia).
* **Motora:** Opção "Aumentar Área de Toque" expande os *hit targets* para >44px (WCAG 2.5.5).
* **Cognitiva:** "Simplificar Rótulos" e "Alertas de Tempo Estendido" reduzem a carga cognitiva e ansiedade (WCAG 2.2.1).

### ✅ Confirmação de Ajuste
<div align="center">
  <img src="https://github.com/user-attachments/assets/87a70d19-8a2c-4205-8980-6b471178d5a5" width="300" alt="Feedback de Alterações Salvas" />
</div>

**Função:** Feedback de sistema para encerramento de ciclo.
* **Feedback Visual:** Ícone de check em verde fornece validação instantânea de que as preferências foram aplicadas.
* **Navegação:** Botão único e claro "Voltar para o início" evita becos sem saída na navegação.

---

## 2. Dashboard e Navegação
O ponto de partida da aluna, focado em organização e redução de ansiedade.

### 📋 Lista de Tarefas (Home)
<div align="center">
  <img src="https://github.com/user-attachments/assets/018d97e9-a02f-4a3c-b534-7aab7e10ee38" width="300" alt="Dashboard Principal" />
</div>

**Função:** Priorização e acesso rápido.
* **Hierarquia:** O card "Próxima Entrega" no topo isola a urgência (Relatório Parcial em 2 dias), ajudando a aluna a focar no que importa agora.
* **Acessibilidade:** O ícone de acessibilidade é fixo no topo direito, garantindo acesso às configurações em qualquer momento.
* **Consistência:** Botões listados com ícones de seta indicam claramente que levam a uma nova tela.

---

## 3. Fluxo de Submissão e Feedback
Gerenciamento de envios com comunicação integrada e tratamento de erros.

### 📤 Upload e Envio
<div align="center">
  <img src="https://github.com/user-attachments/assets/4d90a93b-7556-4e71-9a4c-77e9dd99610f" width="300" alt="Tela de Upload" />
</div>

**Função:** Envio simplificado de tarefas.
* **Multitarefa:** Combina a ação de upload (ícone de nuvem grande) com um campo de mensagem opcional, permitindo contextualizar o envio para o orientador na mesma tela.
* **Affordance:** O botão "ENVIAR ATIVIDADE" ocupa toda a largura, facilitando o toque com o polegar.

### 🔔 Feedback do Sistema
O sistema comunica claramente o resultado da ação, reduzindo incertezas.

| Sucesso | Erro (Tratamento) |
| :---: | :---: |
| <img src="https://github.com/user-attachments/assets/4a64cd9f-0e70-4858-9d2d-a196c1cefa33" width="250" /> | <img src="https://github.com/user-attachments/assets/22012c9e-d247-486b-820f-094cef8a0824" width="250" /> |
| **Confirmação:** Uso da cor verde e mensagem direta "Enviado com Sucesso!" para tranquilizar o aluno. | **Recuperação:** Alerta amarelo com instrução acionável ("Verifique sua conexão") e botão "Tentar Novamente" para evitar frustração. |

---

## 4. Tarefas Acadêmicas Específicas
Telas desenhadas para fluxos de trabalho complexos.

### 👁️ Revisar Apresentação
<div align="center">
  <img src="https://github.com/user-attachments/assets/e57b959e-d84d-480d-bd64-7a764d6fb24f" width="300" alt="Tela de Revisão" />
</div>

**Função:** Acesso a materiais de estudo/correção.
* **Contexto:** Exibe status "Pendente" com ícone de alerta amarelo.
* **Recursos:** Lista clara de documentos necessários com botões distintos para "Baixar" e "Visualizar", facilitando o acesso ao feedback do professor.

### 📝 Enviar Artigo
<div align="center">
  <img src="https://github.com/user-attachments/assets/0b57e5a5-9924-4c77-a7c5-fabfd86bcfb8" width="300" alt="Tela de Envio de Artigo" />
</div>

**Função:** Submissão final com controle de qualidade.
* **Prevenção de Erros:** Implementa um **Checklist de Requisitos** (ABNT, Gramática, PDF). O design sugere que o envio só deve prosseguir se esses itens forem validados, prevenindo erros de submissão (WCAG 3.3.4).

### 📍 Registrar Presença
<div align="center">
  <img src="https://github.com/user-attachments/assets/db8d3e7a-a879-4413-b2c4-2b2cc1a168e1" width="300" alt="Tela de Presença" />
</div>

**Função:** Validação rápida de frequência.
* **Geolocalização:** Feedback visual imediato ("Localização Válida" com check verde) informa que o aluno está no local correto (Campus 2, Bloco A), permitindo o check-in.

### 📂 Relatório de Estágio
<div align="center">
  <img src="https://github.com/user-attachments/assets/0459f7fc-0deb-4d2c-8b2f-54c377f07b12" width="300" alt="Tela de Relatório de Estágio" />
</div>

**Função:** Submissão documental complexa.
* **Segmentação:** Separa o upload em "Arquivo Principal" e "Anexo Obrigatório", guiando o aluno para não esquecer partes do relatório.
* **Instruções:** Links para instruções completas e regras ABNT mantêm a tela limpa, mas oferecem suporte se necessário.

Acessibilidade
<img width="392" height="851" alt="Acessibilidade" src="https://github.com/user-attachments/assets/b9a858b4-2e07-4c98-a4ea-504cf0ed1355" />

Acessibilidade
<img width="392" height="851" alt="Acessibilidade-1" src="https://github.com/user-attachments/assets/87a70d19-8a2c-4205-8980-6b471178d5a5" />

tela 1 Lista de tarefas
<img width="392" height="851" alt="Tela 1 - Lista de Tarefas" src="https://github.com/user-attachments/assets/018d97e9-a02f-4a3c-b534-7aab7e10ee38" />

tela 2 Upload e envio
<img width="392" height="851" alt="Tela 2 - Upload e Envio" src="https://github.com/user-attachments/assets/4d90a93b-7556-4e71-9a4c-77e9dd99610f" />

tela 3 sucesso
<img width="392" height="851" alt="Tela 3 - Sucesso" src="https://github.com/user-attachments/assets/4a64cd9f-0e70-4858-9d2d-a196c1cefa33" />

tela 4 erro
<img width="392" height="851" alt="Tela 4 - Erro" src="https://github.com/user-attachments/assets/40871802-9dfc-46fc-93b4-6eb3c0cbc9cf" />

erro
<img width="392" height="851" alt="Tela 4 - Erro-1" src="https://github.com/user-attachments/assets/22012c9e-d247-486b-820f-094cef8a0824" />

<img width="392" height="851" alt="Tela 9" src="https://github.com/user-attachments/assets/e57b959e-d84d-480d-bd64-7a764d6fb24f" />

<img width="392" height="851" alt="Tela 10" src="https://github.com/user-attachments/assets/0b57e5a5-9924-4c77-a7c5-fabfd86bcfb8" />

<img width="392" height="851" alt="Tela 11" src="https://github.com/user-attachments/assets/db8d3e7a-a879-4413-b2c4-2b2cc1a168e1" />

<img width="392" height="851" alt="Tela 12" src="https://github.com/user-attachments/assets/0459f7fc-0deb-4d2c-8b2f-54c377f07b12" />



</div>
