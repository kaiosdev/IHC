# 6. Análise de Heurísticas, UX, Acessibilidade e Comunicabilidade

Esta seção apresenta como o design do **E-Project UFAM** aplica os princípios de usabilidade (Heurísticas de Nielsen), acessibilidade (WCAG / Lei de Fitts), comunicação visual e experiência do usuário, considerando especialmente as personas **Prof. Carlos (baixa visão)** e **Ana Beatriz (orientanda)**.

---

## 🎯 6.1 Aplicação das Heurísticas de Nielsen

### **Heurística 1 — Visibilidade do estado do sistema**
O sistema fornece feedback imediato sobre ações realizadas.
- **Onde aparece:** Telas de Sucesso/Erro e Dashboard.
- **Evidências de design:**
  - Ícone verde de check e mensagem “Enviado com Sucesso”.
  - Barra de progresso visual nos cards de projeto (ex: 65%).
  - Tags de status coloridas (“Em andamento”, “Atrasado”).

---

### **Heurística 2 — Correspondência entre o sistema e o mundo real**
Uso de linguagem acadêmica real do contexto UFAM.
- Termos familiares: *PIBIC, PACE, Proext, Edital, Orientador, Bolsista*.
- Ícone de pasta (*folder*) representa “Meus Projetos” como organização documental.

---

### **Heurística 3 — Controle e liberdade**
Permite desfazer e corrigir ações facilmente.
- Botão **Voltar** em telas internas.
- Tela de erro oferece **Tentar Novamente** sem perder informações.

---

### **Heurística 4 — Consistência e padrões**
Interface mantém coerência estética e funcional.
- Verde UFAM (`#00663C`) como ação primária / Vermelho (`#D32F2F`) para erros.
- Iconografia: *Material Symbols Rounded* (filled = ativo / outline = inativo).
- Tipografia consistente: **Montserrat** para títulos e **Roboto** para corpo.

---

### **Heurística 5 — Prevenção de erros**
A interface evita falhas antes de acontecerem.
- Seleção inicial de perfil (Orientador / Orientando) previne acessos inadequados.
- Área de upload orienta formatos aceitos: *PDF / DOCX*.

---

### **Heurística 6 — Reconhecimento ao invés de memorização**
Informações visíveis reduzem carga cognitiva.
- Ícones sempre acompanhados de rótulos textuais.
- Dashboard exibe alerta de prazo: **“Próxima entrega em 2 dias”**.

---

### **Heurística 8 — Estética e Design Minimalista**
Interface limpa e objetiva, sem poluição visual.
- Uso de espaçamento amplo, ênfase em elementos essenciais.
- Dashboard prioriza leitura rápida e hierarquia visual clara.

---

### **Heurística 9 — Diagnóstico e recuperação de erros**
Mensagens claras e orientadas à ação.
- “Não foi possível enviar. Verifique sua conexão com a internet.”
- Ícone triangular amarelo comunica atenção universalmente.

---

## ♿ 6.2 Acessibilidade e Inclusão

| Critério | Implementação |
|---------|---------------|
| **Contraste de Cores (WCAG)** | Verde UFAM e Azul Profundo testados no WebAIM para legibilidade |
| **Lei de Fitts** | Botões full-width e área de toque ≥ **48dp** na versão mobile |
| **Rótulos Obrigatórios** | Nenhum ícone é apresentado sem texto complementar |
| **Persona de Baixa Visão** | Hierarquia tipográfica, cores fortes e foco em clareza visual |

---

## 🧠 6.3 Comunicabilidade e Signos Metalinguísticos

- **Código de cores semântico**
  - 🟢 Verde = sucesso / progresso
  - 🟡 Amarelo = atenção / prazo próximo
  - 🔴 Vermelho = erro / atraso crítico
- **Microinterações**
  - Animações curtas e variação de cor ao pressionar botões
  - Smart Animate reforça confirmações de ação e diminui ansiedade do usuário
- **Estados vazios instrucionais**
  - Ex: *“Toque para buscar o arquivo”* orientando próximo passo

---

## 💡 Síntese Final
O design do **E-Project UFAM** demonstra uma aplicação consistente das Heurísticas de Nielsen, garantindo:
- Experiência fluida e previsível
- Comunicação clara entre usuário e sistema
- Inclusão e acessibilidade real baseadas nas personas definidas
- Redução de erros e aumento de confiança durante as interações

Assim, o sistema proporciona **usabilidade elevada, comunicabilidade eficaz e alinhamento total com necessidades reais de orientadores e orientandos da UFAM**.

---
