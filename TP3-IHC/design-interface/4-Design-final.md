<h1>DESIGN FINAL DA INTERFACE</h1>

#  E-Project Mobile: Fluxo do Aluno e Professor

> *Persona:* Ana Beatriz (Estudante & Bolsista)
> *Foco:* Organização, Acessibilidade e Redução de Ansiedade.

Este documento detalha a implementação da interface mobile, destacando os fluxos de tarefas, tratamento de erros e conformidade com WCAG.

</div>

---

## 1.  Dashboard e Navegação Vertical
Visão geral da estrutura de navegação e como o aplicativo lida com listagens longas (Scroll Infinito).

| Dashboard (Topo) | Listagem de Projetos (Scroll) |
| :---: | :---: |
| *Foco na Urgência:* O topo da tela isola a "Próxima Entrega" (vence em 2 dias) para priorização imediata. Acesso rápido às configurações de acessibilidade no header. | *Visibilidade de Status:* Cards expansivos com barras de progresso visual. Uso de espaçamento generoso para evitar toques acidentais na rolagem. |
<img width="887" height="864" alt="Captura de tela 2025-12-01 212652" src="https://github.com/user-attachments/assets/8e39b138-34fd-4020-a6f6-2715702d4fc2" />
<img width="697" height="778" alt="Captura de tela 2025-12-01 215547" src="https://github.com/user-attachments/assets/d6898187-c1c3-4e0d-918e-4c054167f829" />

## Orientador
<img width="958" height="810" alt="Captura de tela 2025-11-28 200214" src="https://github.com/user-attachments/assets/bc320e11-2be6-4adf-abb0-8ce036f93396" />
<img width="1053" height="847" alt="Captura de tela 2025-12-01 215529" src="https://github.com/user-attachments/assets/530bc58b-4950-4b06-88d6-9d7541cdd7b7" />


---

## 2.  Descoberta de Editais (Feed)
Interface otimizada para busca e visualização de oportunidades em telas pequenas.

| Filtros e Busca | Visualização de Prazos |
| :---: | :---: |
| *Zona do Polegar:* Filtros (Chips) e barra de busca posicionados para fácil alcance. | *Alerta Visual:* Prazos próximos são destacados em *Vermelho* (14/12/2024) para chamar atenção imediata durante a rolagem rápida. |<img width="592" height="887" alt="Captura de tela 2025-12-01 212715" src="https://github.com/user-attachments/assets/eb29c62c-46be-414c-b610-2053be4523d9" />

| <img width="512" height="554" alt="Captura de tela 2025-11-28 200409" src="https://github.com/user-attachments/assets/0e769985-f435-41e9-a053-601605190a9b" /> |

---
<div align="center">

<h1>DESIGN FINAL DA INTERFACE</h1>

<img src="https://img.shields.io/badge/Disciplina-IHC-003f52?style=for-the-badge&logo=googlescholar&logoColor=white" alt="Disciplina IHC">
<img src="https://img.shields.io/badge/Artefato-UI_Design-008f54?style=for-the-badge&logo=figma&logoColor=white" alt="UI Design">

<br><br>

> **Interface de Alta Fidelidade**
> <br>Apresentação das telas principais e fluxos de navegação, evidenciando a aplicação das Heurísticas de Nielsen, signos metalinguísticos e requisitos de acessibilidade.

</div>

---

## 1. Interface Mobile — Fluxo do Aluno (PIBIC)

Esta seção detalha a experiência projetada para o uso em smartphones, priorizando notificações rápidas e consulta de pendências.

### 👤 Persona em Foco: Ana Beatriz
<img src="https://img.shields.io/badge/PERFIL-ESTUDANTE_DE_ENGENHARIA-003f52?style=flat-square">
<img src="https://img.shields.io/badge/VÍNCULO-BOLSISTA_PIBIC-008f54?style=flat-square">

> **Cenário:** Ana precisa conciliar aulas, estágio e pesquisa. O aplicativo deve ser seu "assistente pessoal", evitando que ela perca prazos.

| 😫 Dores e Necessidades | 💡 Solução de Design (Mobile) |
| :--- | :--- |
| **Sobrecarga Cognitiva:** Medo de esquecer prazos em meio a muitas tarefas. | **Dashboard Limpo:** Foco total na "Próxima Entrega" e cards de pendências com contagem regressiva. |
| **Ansiedade na Comunicação:** Insegurança se o orientador recebeu os arquivos. | **Feedback Imediato:** Uso de microinterações e mensagens de sucesso claras após cada envio. |
| **Uso em Trânsito:** Acesso rápido entre uma aula e outra. | **Navegação Simplificada:** Menus inferiores acessíveis com o polegar e textos curtos. |

<br>

<div align="center">

---

### Navegação
<a href="#-visão-geral-do-fluxo">Visão Geral</a> •
<a href="#-tarefas-acadêmicas">Tarefas Acadêmicas</a> •
<a href="#-rotina-administrativa">Rotina Administrativa</a> •
<a href="#-acessibilidade-e-feedback">Acessibilidade & Feedback</a>

</div>

---

## 📌 Visão Geral do Fluxo

Centraliza a rotina da aluna — priorização de tarefas, envio de arquivos complexos e comunicação em uma interface amigável.

| **Dashboard e Priorização** | **Submissão Integrada (Upload + Chat)** |
| :---: | :---: |
| Foco em redução da ansiedade com destaque de prazos e áreas de toque ampliadas. | Envio de arquivo e mensagem contextual para o orientador na mesma tela. |
| <img src="https://github.com/user-attachments/assets/b6fefac4-7730-46e5-84dc-3ff3aa0dd2f6" width="280" /> | <img src="https://github.com/user-attachments/assets/c0784aff-d239-4d6a-b9fc-7b135aefee21" width="280" /> |

---

### 🎯 Feedback do Sistema

| **Sucesso (Tranquilizador)** | **Erro (Acionável)** |
| :---: | :---: |
| Confirmação verde e mensagem positiva. | Instruções claras para resolução, reduzindo frustração. |
| <img src="https://github.com/user-attachments/assets/f3602ce5-2fec-45ba-92de-8121a8e3e812" width="250" /> | <img src="https://github.com/user-attachments/assets/fa57e469-ada6-44d1-8fa6-08564fe11a94" width="250" /> |

---

## 📚 Tarefas Acadêmicas

| **Revisão de Apresentação** | **Envio de Artigo Final** |
| :---: | :---: |
| Acesso rápido aos materiais e feedback do professor com botões de contraste alto. | Checklist habilita o botão de envio apenas após cumprir requisitos — evita erros. |
| <img src="https://github.com/user-attachments/assets/ca4df9e8-e754-4fde-b2fb-d479b97e0875" width="280" /> | <img src="https://github.com/user-attachments/assets/b306d8fe-9fb6-473a-8299-1b44de608175" width="280" /> |

---

## 🗂 Rotina Administrativa

| **Check-in de Presença** | **Relatório de Estágio** |
| :---: | :---: |
| Ação imediata com validação visual de geolocalização. | Fluxo segmentado com uploads múltiplos e instruções de normas ABNT. |
| <img src="https://github.com/user-attachments/assets/fe9ea190-e5de-4762-9e2b-1374761ef772" width="280" /> | <img src="https://github.com/user-attachments/assets/d15c76ee-bbd8-4bf6-89c6-a1270ea408bb" width="280" /> |

---

## 🔎 Acessibilidade e Feedback
Implementação rigorosa das diretrizes **WCAG**, garantindo a inclusão.

| **Painel de Configurações (WCAG)** | **Confirmação Pós-Ajuste** |
| :---: | :---: |
| Controle de contraste, tamanho da fonte, área de toque e simplificação cognitiva. | Mensagem clara e botão único para retorno. |
| <img src="https://github.com/user-attachments/assets/24d5a9cf-cf5d-4865-8288-413ca19708b7" width="280" /> | <img src="https://github.com/user-attachments/assets/52e5ff4e-aa91-4d51-bfa7-c8d986b3857b" width="280" /> |

---

<div align="center">

## 🎨 Design System Mobile

| Cor Primária (Verde UFAM) | Cor de Erro/Alerta |
| :---: | :---: |
| ![#1B5E20](https://via.placeholder.com/150x50/1B5E20/ffffff?text=HEX+%231B5E20) | ![#D32F2F](https://via.placeholder.com/150x50/D32F2F/ffffff?text=HEX+%23D32F2F) |
| Ações principais e identidade visual. | Falhas críticas e alertas. |

</div>

---

## 🧠 Fluxo Completo — Telas Individuais (Prints)

> 🔻 *A seguir, todas as telas organizadas em sequência funcional do usuário*

### Acessibilidade
<img width="392" height="851" src="https://github.com/user-attachments/assets/b9a858b4-2e07-4c98-a4ea-504cf0ed1355" />
<img width="392" height="851" src="https://github.com/user-attachments/assets/87a70d19-8a2c-4205-8980-6b471178d5a5" />

### Tela 1 — Lista de Tarefas
<img width="392" height="851" src="https://github.com/user-attachments/assets/018d97e9-a02f-4a3c-b534-7aab7e10ee38" />

### Tela 2 — Upload e Envio
<img width="392" height="851" src="https://github.com/user-attachments/assets/4d90a93b-7556-4e71-9a4c-77e9dd99610f" />

### Tela 3 — Sucesso
<img width="392" height="851" src="https://github.com/user-attachments/assets/4a64cd9f-0e70-4858-9d2d-a196c1cefa33" />

### Tela 4 — Erro
<img width="392" height="851" src="https://github.com/user-attachments/assets/40871802-9dfc-46fc-93b4-6eb3c0cbc9cf" />
<img width="392" height="851" src="https://github.com/user-attachments/assets/22012c9e-d247-486b-820f-094cef8a0824" />

### Tela 5 — Revisar Apresentação
<img width="392" height="851" src="https://github.com/user-attachments/assets/e57b959e-d84d-480d-bd64-7a764d6fb24f" />

### Tela 6 — Enviar Artigo
<img width="392" height="851" src="https://github.com/user-attachments/assets/0b57e5a5-9924-4c77-a7c5-fabfd86bcfb8" />

### Tela 7 — Registrar Presença
<img width="392" height="851" src="https://github.com/user-attachments/assets/db8d3e7a-a879-4413-b2c4-2b2cc1a168e1" />

### Tela 8 — Relatório de Estágio
<img width="392" height="851" src="https://github.com/user-attachments/assets/0459f7fc-0deb-4d2c-8b2f-54c377f07b12" />

---
<div align="center">

✨ **Design orientado à redução da ansiedade, acessibilidade real e fluxo sem barreiras.**  

</div>
