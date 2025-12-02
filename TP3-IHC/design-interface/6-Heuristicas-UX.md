# 📱 Relatório de Design de Interface: Aplicação Acadêmica

Este documento apresenta a documentação das decisões de design para o aplicativo de gestão acadêmica, com foco nos critérios de Interação Humano-Computador (IHC). A análise detalha a aplicação das **Heurísticas de Nielsen**, **Comunicabilidade**, **UX** e **Acessibilidade**.

---

## 1. Visibilidade do Estado do Sistema (Heurística 1)

O sistema deve sempre manter os usuários informados sobre o que está acontecendo, por meio de feedback apropriado em tempo razoável.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1VeZC_8hexuH72w-ez9WPNTtah7HsvG1v" width="400px" alt="Heurística 1 - Visibilidade">
</div>

**Descrição e Análise:**
* **Feedback Visual de Progresso:** Utilização de barras de progresso (ex: "65%", "80%") nos cartões de projetos (PIBIC, PACE), permitindo que o aluno saiba exatamente quanto falta para a conclusão.
* **Status Tags:** Etiquetas claras como "Em andamento" informam o estado atual da atividade sem ambiguidade.
* **Fonte:** Interface do Aplicativo - Tela de Projetos.

---

## 2. Correspondência entre o Sistema e o Mundo Real (Heurística 2)

O sistema fala a linguagem do usuário, com palavras, frases e conceitos familiares, seguindo convenções do mundo real.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1eMIRZNfBYzc7NOTTudDdAlJb8lWLrWS9" width="400px" alt="Heurística 2 - Correspondência">
</div>

**Descrição e Análise:**
* **Mapeamento de Ícones:** Uso de ícones que representam metaforicamente objetos físicos conhecidos (ex: gráfico para projetos, relógio para andamento, check para concluídos).
* **Linguagem Natural:** Termos como "Atrasados", "Concluídos" e "Novo Projeto" são diretos e familiares ao contexto acadêmico, facilitando o fluxo e a eficiência da UX.
* **Fonte:** Interface do Aplicativo - Dashboard Principal.

---

## 3. Controle e Liberdade do Usuário (Heurística 3)

Os usuários frequentemente escolhem funções do sistema por engano e precisam de uma "saída de emergência" claramente marcada.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1X-Xi00a2BHhdUA-sii3Zm76vLiz-E_nZ" width="400px" alt="Heurística 3 e 9 - Controle e Erros">
</div>

**Descrição e Análise:**
* **Navegação Reversível:** Botões de ação secundária como "Voltar para o início" ou "Tentar Novamente" garantem que o usuário não fique preso em estados de erro ou sucesso.
* **Código Cromático Semântico:** Uso do verde para sucesso e amarelo/vermelho para falhas, reforçando a comunicabilidade do estado da ação.
* **Fonte:** Interface do Aplicativo - Telas de Feedback de Envio.

---

## 4. Prevenção de Erros (Heurística 5)

Melhor do que boas mensagens de erro é um design cuidadoso que evita, em primeiro lugar, que problemas ocorram.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1va7NKjGDjXpB3RxYS1o7NcO1C04inWj5" width="400px" alt="Heurística 5 - Prevenção de Erros">
</div>

**Descrição e Análise:**
* **Restrições de Upload:** O sistema informa explicitamente o formato aceito (.pdf) e o tamanho limite (10MB) antes do envio, prevenindo erros de compatibilidade.
* **Checklists de Validação:** A seção de "Requisitos de Submissão" atua como um *checklist* mental e sistêmico para garantir que o aluno não envie documentos incompletos.
* **Fonte:** Interface do Aplicativo - Tela de Envio de Artigo.

---

## 5. Reconhecimento em vez de Memorização (Heurística 6)

Minimizar a carga de memória do usuário tornando objetos, ações e opções visíveis.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1eMIRZNfBYzc7NOTTudDdAlJb8lWLrWS9" width="400px" alt="Heurística 6 - Reconhecimento">
</div>

**Descrição e Análise:**
* **Informação Contextual:** O card de "Próxima Entrega" exibe proativamente o que é urgente, evitando que o usuário tenha que navegar pelo calendário para lembrar prazos.
* **Instruções Visuais:** O ícone de upload com a instrução "Toque para buscar o arquivo" deixa a affordance (possibilidade de ação) explícita.
* **Fonte:** Interface do Aplicativo - Home e Upload.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1eMIRZNfBYzc7NOTTudDdAlJb8lWLrWS9" width="400px" alt="Heurística 6 - Cores e Prazos">
</div>

* **Uso de Cores para Prazos:** A data em vermelho e a tag amarela "Encerrando em breve" comunicam urgência visualmente, facilitando o reconhecimento rápido sem necessidade de leitura profunda.

---

## 6. Ajuda e Documentação (Heurística 10)

Mesmo que o sistema possa ser usado sem documentação, pode ser necessário fornecer ajuda e documentação.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1_Sc85OOv6z32bSwfW0Y-iAbejO45A7gi" width="400px" alt="Heurística 10 - Ajuda">
</div>

**Descrição e Análise:**
* **Acesso Rápido a Regras:** Botões dedicados para "Ver Instruções Completas" e "Ver Regras de Formatação ABNT" fornecem suporte no momento exato da tarefa (context-sensitive help).
* **Clareza nas Instruções:** Texto explicativo curto e direto acima dos botões de ação.
* **Fonte:** Interface do Aplicativo - Tela de Relatório de Estágio.

---

## 7. Acessibilidade e Inclusão

O design considera a diversidade de necessidades dos usuários, permitindo personalização da interface.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1VhyPXNB0ScBo-GWe3mOHIYag620hcA35" width="400px" alt="Acessibilidade">
</div>

**Descrição e Análise:**
* **Controle Visual:** Opções para ajuste de tamanho de texto e alto contraste atendem usuários com baixa visão.
* **Modo Escuro:** Inclusão de Dark Mode para conforto visual e economia de bateria.
* **Auxílio Cognitivo e Motor:** Opções para "Simplificar Rótulos" e "Aumentar Área de Toque" (Lei de Fitts), facilitando a interação para usuários com dificuldades motoras finas.
* **Fonte:** Interface do Aplicativo - Configurações de Acessibilidade.

---

## 8. Comunicabilidade e Ciclo de Feedback

O design estabelece uma conversa eficiente com o usuário através de metalinguagem e feedback contínuo.

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1LweSTGCf5h9nTANPuW9Jc5fee7PeuSl-" width="400px" alt="Comunicabilidade - Feedback">
</div>

**Descrição e Análise:**
* **Feedback Acadêmico:** O sistema fecha o ciclo de comunicação disponibilizando o arquivo de "Feedback_Prof.pdf" diretamente na tela de tarefa, permitindo que o aluno veja a resposta do sistema/professor para sua ação anterior.
* **Status de Ação:** O alerta amarelo com "Requer sua Ação" direciona a atenção do usuário para pendências críticas.
* **Fonte:** Interface do Aplicativo - Tela de Revisão.

---

<div align="center">
  <sub>Trabalho desenvolvido para a disciplina de Interação Humano-Computador | UFAM</sub>
</div>
