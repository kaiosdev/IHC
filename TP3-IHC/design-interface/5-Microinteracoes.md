<div align="center">

<h1>🎬 MICROINTERAÇÕES – E-PROJECT UFAM</h1>

<img src="https://img.shields.io/badge/Disciplina-Interação_Humano--Computador-003f52?style=for-the-badge&logo=googlescholar&logoColor=white" alt="Disciplina: IHC">
<img src="https://img.shields.io/badge/Projeto-E--Project_UFAM-008f54?style=for-the-badge&logo=figma&logoColor=white" alt="Projeto: E-Project UFAM">
<img src="https://img.shields.io/badge/Ferramenta-Figma-003f52?style=for-the-badge&logo=figma&logoColor=white" alt="Figma">

<br><br>

> **Feedback e Fluidez**
> <br>Protótipo de alta fidelidade com foco em **microinterações**, **feedback imediato** e **fluidez de navegação** para o sistema acadêmico **E-Project UFAM**. As animações foram concebidas utilizando **Smart Animate** e **Prototype Interactions** no Figma.

<br>

<a href="https://www.figma.com/design/lLDopNGZcEgvP0ihCUu2W0/E-Project?node-id=0-1&p=f&t=5IBWSzOBG1SzTdvN-0">
  <img src="https://img.shields.io/badge/🔗_ABRIR_PROTÓTIPO_NO_FIGMA-008f54?style=for-the-badge&logo=figma&logoColor=white">
</a>

</div>

---

## 📘 Sumário
➡️ [**Sobre as Microinterações**](#sobre-as-microinterações)  
🎓 [**Persona: Orientador**](#persona-orientador)  
👩‍🎓 [**Fluxo: Tela de Ana (Orientanda)**](#fluxo-tela-de-ana-orientanda)  
🧠 [**Conclusão Geral**](#conclusão-geral)

---

## 💡 Sobre as Microinterações

As microinterações do **E-Project UFAM** foram desenhadas para:

- **Guiar o usuário** em tarefas complexas (envio de relatórios, presença, estágio);
- Oferecer **feedback claro** para cada ação (sucesso, erro, estado pendente);
- Manter **consistência visual e comportamental** em todas as telas;
- Atender critérios de **acessibilidade** desde o início da jornada.

**Principais recursos utilizados:**

- 🎨 **Figma** – prototipação de alta fidelidade  
- ✨ **Smart Animate** – transições suaves entre estados de componentes  
- 🔗 **Prototype Interactions** – definição de fluxos, gatilhos e estados de feedback  

---

## 👨‍🏫 Persona: Orientador

🎥 **Demonstração em Vídeo**  
🔗 [Fluxo do Orientador no Google Drive](https://drive.google.com/file/d/1STtqxaqsTUFfcSwDYPMre3um3ZmEiURT/view?usp=sharing)

---

### 👀 Visão Geral

O orientador acessa o E-Project para:

- Consultar **editais**;
- Acompanhar **presença** dos orientandos;
- Ver **projetos e entregas** em andamento.

A interface foi pensada para um uso rápido, focado em monitoramento e tomada de decisão.

### ✨ Principais Microinterações

- **Tela de Login / Seleção de Perfil**
  - Destaque visual no perfil selecionado;
  - Transição suave entre opções de usuário (orientador / orientando).

- **Dashboard do Orientador**
  - Cartões carregam com *fade-in* e leve movimento vertical;
  - Elementos importantes (projetos, pendências) surgem em ordem hierárquica, facilitando o escaneamento visual.

- **Ver Editais**
  - Navegação horizontal entre listas de editais;
  - Cartões surgem em sequência com combinação de *slide-up* + *opacity fade*.

- **Controle de Presença**
  - Lista de projetos com animação de entrada;
  - Estado vazio inicial com mensagem “Selecione um projeto”, evitando tela “morta”.

### 🎯 Decisões de Design (Orientador)

- **Feedback visual imediato** em toda ação clicável;
- **Transições suaves**, preservando o contexto entre telas;
- Uso de **cores institucionais** com contraste adequado;
- **Padrões de animação reaproveitados**, reforçando previsibilidade e reduzindo curva de aprendizado.

---

## 👩‍🎓 Fluxo: Tela de Ana (Orientanda)

🎥 **Demonstração em Vídeo**  
🔗 [Fluxo completo da Ana no Google Drive](https://drive.google.com/file/d/1lphGqdTunDBiVrGzKMJqFwNTKdb1Tmaz/view?usp=sharing)

---

### 1. Dashboard da Ana e Acessibilidade

#### 🏠 Dashboard / Lista de Tarefas

- Saudação personalizada: **“Olá, Ana Beatriz”**;
- Cartão em destaque de **Próxima Entrega** (Relatório Parcial PIBIC, com prazo e urgência);
- Lista de tarefas em cartões:
  - **Enviar Relatório**
  - **Revisar Apresentação**
  - **Enviar Artigo**
  - **Registrar Presença**
  - **Relatório de Estágio**

**Microinterações:**

- Cartões entram com *fade-in* + movimento suave;
- Toque gera leve expansão e mudança de cor;
- Ícones de seta comunicam continuidade de fluxo.

#### ♿ Tela de Acessibilidade

Acessada pelo ícone de cadeira de rodas no topo.

- **Visualização e Contraste**
  - Slider de **tamanho de texto** com resposta visual imediata;
  - *Switches* para **Alto Contraste**, **Dark Mode** e **Animações/Transições**.

- **Auxílio à Leitura**
  - Destaque de foco para navegação por teclado;
  - Opção de **simplificar rótulos de botão**.

- **Interação e Tempo**
  - Aumento de **área de toque (Hit Area)**;
  - **Alertas de tempo estendido** para tarefas com prazos.

**Feedback de Sucesso:**

- Tela de confirmação com ícone ✔️ em destaque;
- Mensagem **“Alterações Salvas com Sucesso!”**;
- Botão **“Voltar para o início”**, mantendo a usuária sempre com opção clara de retorno.

---

### 2. Enviar Relatório – Relatório Parcial PIBIC

#### 🧾 Seleção da Tarefa

- Ana toca em **“Enviar Relatório – Biodiversidade Amazônica”**;
- Cartão reage com microanimação e leva à tela de upload.

#### ⬆️ Tela de Upload e Envio

- Cabeçalho com título **“Enviar Relatório”**, seta de **voltar** e ícone de acessibilidade;
- Área de upload com borda tracejada e texto:  
  > “Toque para buscar o arquivo PDF ou DOCX”
- Campo **“Mensagem para o orientador (opcional)”**;
- Botão primário **“ENVIAR ATIVIDADE”** com animação de clique.

#### ✅ Sucesso

- Ícone circular verde ✔️ com efeito de entrada;
- Mensagem **“Enviado com Sucesso!”** e aviso de que o orientador foi notificado;
- Botão **“Voltar para o início”** retorna ao dashboard com transição suave.

#### ⚠️ Erro

- Ícone triangular amarelo de alerta;
- Mensagem **“Falha no Envio”** com orientação para verificar a conexão;
- Botão **“TENTAR NOVAMENTE”** em destaque;
- Seta de **voltar** permanece disponível, evitando beco sem saída.

> 🔁 Em todo o fluxo, Ana **nunca fica presa em um estado de erro**: sempre há opção de voltar ou tentar novamente.

---

### 3. Revisar Apresentação

- Tela **“Revisar Apresentação”** com cabeça padrão (voltar + acessibilidade);
- Cartão de **Status**:
  - Nome da tarefa;
  - Estado “Pendente (requer sua ação)”;
  - Prazo em destaque.
- **Detalhes e Instruções**
  - Texto com foco na revisão da seção adequada;
  - Botão **“Ver instruções completas >”**.
- **Documentos Necessários**
  - Arquivos listados com ações **“Baixar”** e **“Visualizar”**.
- Ações principais:
  - **“Abrir para Revisão”** (botão primário);
  - **“Marcar como Não Aplicável”** (alternativa).

**Foco de design:**  
Permitir que Ana entenda rapidamente **o que precisa ser feito**, **com quais arquivos** e **qual o prazo**, sem sobrecarga visual.

---

### 4. Enviar Artigo

- Tela **“Enviar Artigo”** com voltar + acessibilidade;
- Cartão de **Prazo** (“Vence em 15 dias”, com data exata);
- **Requisitos de Submissão** (checkboxes):
  - Conformidade com ABNT;
  - Revisão de linguagem/gramática;
  - Versão definitiva em PDF.
- **Upload do Artigo Final**
  - Botão **“Selecionar Arquivo (.pdf)”**;
  - Indicação de limite de 10 MB;
  - Nome e tamanho do arquivo com opção de **remover**.
- Campo de **Notas para a Coordenação**;
- Botão **“Enviar Artigo Definitivo”** fechando o fluxo.

**Destaque:**  
Checklists guiando a usuária pelos **pré-requisitos obrigatórios**, reduzindo risco de submissões incompletas.

---

### 5. Registrar Presença

- Tela **“Registrar Presença”** com voltar + acessibilidade;
- Informação do **dia atual** e do **evento** (ex.: “PIBIC – Novembro”);
- Cartão de **Localização para Check-in**:
  - Campus, bloco e sala;
  - Estado **“LOCALIZAÇÃO VÁLIDA”** com ícone confirmando a posição.
- Botão principal **“CHECK-IN AGORA”** com hit area ampliada;
- Botão secundário **“Ver histórico de Presença”** para consulta de registros.

**Intenção de design:**  
Transformar o check-in em uma ação **rápida e inequívoca**, com confirmação visual forte de que a presença foi capturada no local correto.

---

### 6. Relatório de Estágio

- Tela **“Relatório de Estágio”** com voltar + acessibilidade;
- Cartão de **Prazo Final** com data e contagem de dias restantes;
- Seção **Instruções e Detalhes**:
  - Resumo da tarefa;
  - Botões **“Ver Instruções Completas >”** e **“Ver Regras de Formatação ABNT >”**.
- **Requisitos Finais (Checklist)**:
  - Assinatura do supervisor anexada;
  - Relatório final em PDF;
  - Carga horária total verificada.
- **Upload de Arquivos**:
  1. Arquivo Principal (Relatório) – **Selecionar Relatório (.pdf)**  
  2. Anexo Obrigatório (Plano de Atividade) – **Selecionar Anexo (.pdf)**
- Botão **“Enviar Relatório de Estágio”** finalizando a entrega.

**Ponto chave:**  
O uso combinado de **checklist + upload guiado** reduz erros comuns em relatórios finais e deixa claro o que ainda falta.

---

### 🎯 Decisões de Design (Ana)

- **Fluxo único e coeso**: todas as tarefas da Ana partem do mesmo dashboard, mantendo o contexto.
- **Acessibilidade em primeiro plano**: atalho fixo em todas as telas, sem ficar escondido em menus profundos.
- **Microinterações significativas**:
  - Cartões, botões, checkboxes e áreas de upload sempre respondem ao toque;
  - Estados de sucesso/erro são claros e consistentes (verde, vermelho/amarelo, ícones dedicados).
- **Controle nas mãos da usuária**:
  - Sempre existe um caminho para **voltar**, **cancelar** ou **tentar novamente**;
  - Nenhum fluxo deixa a Ana “presa” em uma tela.

---

## 🧠 Conclusão Geral

As microinterações do **E-Project UFAM** foram pensadas para:

- 🔄 Reforçar a **comunicação entre sistema e usuário**, reduzindo incertezas;
- 👁️‍🗨️ Garantir **feedbacks visuais e textuais claros** para cada ação;
- 🧩 Manter **consistência visual e comportamental** entre personas e telas;
- ♿ Incorporar **acessibilidade configurável** como parte central da experiência, e não como um elemento secundário;
- 😌 Proporcionar uma jornada **fluida, previsível e agradável**, especialmente em tarefas críticas como envio de relatórios, presença e relatórios finais.

---
