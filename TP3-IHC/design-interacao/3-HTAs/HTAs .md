# Análise Hierárquica de Tarefas (HTA)

https://drive.google.com/file/d/1Exq5bAjpqa5Gl6QWJfWXguX_ZQ-GbgAi/view?usp=sharing

## HTA 1: Gestão de Tarefas do Orientador

**Persona:** Victor Antunes (Orientador)  
**Objetivo Raiz (0):** Gerenciar Tarefas do Orientando

### 1. Visualização "Lado a Lado" (Mapa vs. HTA)

#### Trecho do Mapa de Objetivos (Origem)
<img width="480" height="519" alt="Captura de tela 2025-11-21 200703" src="https://github.com/user-attachments/assets/a0c60f34-e286-4c9c-b33b-b6e59b684f88" />

```
O
GERENCIAR TAREFAS DO ORIENTANDO
  ├─ Criar nova tarefa para o orientando
  ├─ Definir prazo da tarefa criada
  ├─ Enviar a tarefa ao aluno
  ├─ Analisar tarefas concluídas
  ├─ Revisar relatório anexado
  └─ Registrar aprovação ou solicitação de correção
```

### 2. Sintaxe e Planos

- **Plano 0:** Fazer 1, depois 2. Quando o aluno entregar, fazer 3. Se 3 estiver ok, fazer 4.1, caso contrário, fazer 4.2.
- **Plano 1:** Fazer 1.1 e depois 1.2.
- **Plano 3:** Fazer 3.1 e depois 3.2 .

### 3. Descrição Detalhada

Este HTA foca na persona Victor Antunes. O objetivo principal é a gestão eficiente das atividades dos bolsistas. A análise decompõe o processo em três fases temporais: a criação da demanda (subtarefa 1), a atribuição (subtarefa 2) e a correção (subtarefa 3 e 4).

A hierarquia mostra que "Criar tarefa" e "Definir prazo" são ações atômicas que compõem o planejamento. O ciclo só se encerra (subtarefa 4) quando o professor toma uma decisão binária: aprovar ou pedir revisão, resolvendo a "dor" do usuário de ter comunicação descentralizada.

---

## HTA 2: Execução de Tarefas pelo Aluno

**Persona:** Ana Beatriz (Aluno Orientado - AO/AAC)  
**Objetivo Raiz (0):** Realizar Entregas das Tarefas

### 1. Visualização "Lado a Lado" (Mapa vs. HTA)

#### Trecho do Mapa de Objetivos (Origem)
<img width="1228" height="371" alt="Captura de tela 2025-11-21 200901" src="https://github.com/user-attachments/assets/7544d9af-b20f-49e5-867d-bb564b33d4c7" />

```
AO AAC
REALIZAR ENTREGAS DAS TAREFAS
  ├─ Abrir a lista de tarefas pendentes
  ├─ Ler instruções da tarefa enviada
  ├─ Ver o prazo da tarefa
  ├─ Fazer upload do arquivo solicitado
  ├─ Confirmar o envio da entrega
  ├─ Marcar a tarefa como concluída
  └─ Ver histórico das tarefas concluídas
```

### 2. Sintaxe e Planos

- **Plano 0:** Fazer 1 para selecionar a tarefa. Fazer 2. Se 2 for sucesso, fazer 3. Fazer 4 periodicamente (opcional).
- **Plano 1:** 1.1 depois 1.2.
- **Plano 2:** 2.1 depois 2.2.

### 3. Descrição Detalhada

Focado na persona Ana Beatriz, este HTA mapeia o fluxo linear de entrega de um trabalho acadêmico. A separação entre "Fazer upload" (2.1) e "Confirmar envio" (2.2) é crítica para dar o feedback de segurança que a persona exige ("medo de perder prazos").

O passo 3 (Marcar como concluída) é separado para garantir que o sistema registre o status visualmente (verde), conforme mencionado nos requisitos de acessibilidade cognitiva, dando à aluna a sensação de dever cumprido.

---

## HTA 3: Acessar Opções de Acessibilidade Visual

**Persona:** Prof. Carlos Mendonça (PAV)  
**Objetivo Raiz (0):** Utilizar Interface sem Dificuldade Visual

### 1. Visualização "Lado a Lado" (Mapa vs. HTA)

#### Trecho do Mapa de Objetivos (Origem)
<img width="1030" height="761" alt="Captura de tela 2025-11-21 201507" src="https://github.com/user-attachments/assets/9db8ffa4-dbfa-44f5-8856-77417e9e240b" />

```
PAV
UTILIZAR A INTERFACE SEM DIFICULDADE VISUAL
  ├─ Aumentar o tamanho das fontes
  ├─ Ativar modo de alto contraste
  ├─ Exibir botões com texto ampliado
  ├─ Navegar por fluxos lineares
  └─ Operar o sistema via desktop com zoom
```

### 2. Sintaxe e Planos

- **Plano 0:** Fazer 1 (configuração inicial) e então realizar 2 (uso contínuo).
- **Plano 1:** Fazer 1.1, 1.2 ou 1.3 conforme necessidade (não sequencial, configurável).
- **Plano 2:** Realizar 2.1 enquanto executa 2.2.

### 3. Descrição Detalhada

Este HTA aborda as necessidades do Prof. Carlos Mendonça. Diferente dos fluxos de tarefas (início-meio-fim), este HTA representa um estado de configuração e interação contínua.

O subgrupo 1 agrupa as configurações que o sistema deve persistir (contraste, fonte), enquanto o subgrupo 2 descreve a forma como a tarefa é executada (uso de zoom e fluxos lineares). Isso garante que o objetivo de "evitar fadiga visual" e "confusão" seja atingido antes mesmo da execução da tarefa acadêmica em si.

---

## HTA 4: Acessar Opções de Acessibilidade Cognitiva

**Persona:** João Paulo (AAC)  
**Objetivo Raiz (0):** Manter Foco nas Atividades

### 1. Visualização "Lado a Lado" (Mapa vs. HTA)


#### Trecho do Mapa de Objetivos (Origem)
<img width="1805" height="384" alt="Captura de tela 2025-11-21 201559" src="https://github.com/user-attachments/assets/02a0bc23-f718-4337-ad6a-2ef145a35fb4" />

```
AAC
MANTER FOCO NAS ATIVIDADES DO PROJETO
  ├─ Ver checklist da tarefa atual
  ├─ Identificar a próxima ação ("o que fazer agora")
  ├─ Usar ícones acompanhados de texto
  ├─ Ver cores semânticas
  └─ Ativar modo sem distrações
```

### 2. Sintaxe e Planos

- **Plano 0:** Fazer 1 (preparação). Fazer 2 para compreensão. Fazer 3 para execução.
- **Plano 2:** 2.1 guiado por 2.2 e 2.3 simultaneamente.

### 3. Descrição Detalhada

Focado na persona João Paulo (TDAH/Dislexia), este HTA prioriza a organização mental antes da ação. O plano inicia com a remoção de estímulos externos (1.1).

O passo 2 é crucial: ele decompõe o objetivo de "não se perder" em verificações visuais rápidas (ícones e cores). O HTA demonstra que, para esse usuário, entender o status da tarefa (vermelho/verde) e a próxima ação imediata é um pré-requisito hierárquico para conseguir acessar o checklist (passo 3) e efetivamente trabalhar.

---

## Sobre este Documento

Este documento apresenta a Análise Hierárquica de Tarefas (HTA) para um sistema de gestão acadêmica, focando em diferentes personas e suas necessidades específicas de acessibilidade e usabilidade.
