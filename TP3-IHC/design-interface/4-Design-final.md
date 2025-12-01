# E-Project - Sistema de Gestão de Projetos Acadêmicos UFA
<div align="center">
---

## 📱 Interface Mobile - Fluxo do Aluno (Membro 4)

Este módulo foi desenhado especificamente para a **Persona Ana Beatriz** (Estudante de Engenharia e bolsista PIBIC), focando em resolver suas dores principais: sobrecarga de tarefas e incerteza sobre a comunicação com o orientador.

### 1. Tela de Tarefas (Dashboard Mobile)
Focada na organização rápida e redução de ansiedade.
* **Card de Destaque:** Exibe a entrega mais urgente ("Relatório Parcial") com alerta de prazo em destaque, ajudando a aluna a priorizar.
* **Lista de Demandas:** Cards com áreas de toque expandidas (acessibilidade) para facilitar o uso em movimento.
* **Integração:** Exibe tarefas reais do projeto "Biodiversidade Amazônica" e obrigações administrativas (Frequência, Estágio).
  
<img width="392" height="851" alt="Tela 1 - Lista de Tarefas" src="https://github.com/user-attachments/assets/b6fefac4-7730-46e5-84dc-3ff3aa0dd2f6" />

### 2. Submissão e Atualização
Combina duas funcionalidades em uma única tela para otimizar o tempo do aluno:
* **Upload Intuitivo:** Área de anexo clara com padrão de traçado.
* **Canal Direto:** Campo de mensagem integrado para enviar atualizações de status junto com o arquivo, centralizando a comunicação que antes ficava dispersa no WhatsApp.
* **Botão de Ação:** Botão "Enviar Atividade" com largura total para fácil alcance do polegar.
* 
<img width="392" height="851" alt="Tela 2 - Upload e Envio" src="https://github.com/user-attachments/assets/c0784aff-d239-4d6a-b9fc-7b135aefee21" />

### 3. Feedback do Sistema (Sucesso e Erro)
Telas essenciais para garantir a confirmação da ação e reduzir a insegurança da aluna.
* **Sucesso (Verde):** Confirmação visual clara e mensagem tranquilizadora ("O orientador recebeu sua notificação").
* **Erro (Alerta):** Instrução clara de correção ("Verifique sua conexão") para evitar frustração.

<img width="631" height="1358" alt="Tela 3 - Sucesso" src="https://github.com/user-attachments/assets/f3602ce5-2fec-45ba-92de-8121a8e3e812" />
<img width="392" height="851" alt="Tela 4 - Erro" src="https://github.com/user-attachments/assets/fa57e469-ada6-44d1-8fa6-08564fe11a94" />

### 🎨 Consistência Visual 
O projeto mobile segue estritamente o Design System estabelecido para a versão Desktop (Membro 3):
* **Cores:** Uso do Verde UFAM (#1B5E20) como cor primária e Vermelho (#D32F2F) para estados de erro/alerta.
* **Tipografia:** Hierarquia de textos alinhada com o sistema web.



### 4. Confirmação de Funções 
(Revisar Apresentação)
Função:
Esta tela serve como o ponto de entrada para a tarefa "Revisar Apresentação", fornecendo à Ana Beatriz todo o contexto (status, prazo, instruções) e os documentos necessários para iniciar a revisão.

Decisões de Usabilidade e Acessibilidade:
Comunicação de Urgência: O bloco Status é proeminente, usando um ícone de alerta (⚠️) e a cor vermelha/laranja para o Prazo (14/12/2025), sinalizando que a tarefa é Pendente e requer ação imediata (WCAG 1.4.1 – Uso de cor).

Acesso a Documentos (CRUCIAL):

A seção "Documentos Necessários" lista de forma clara tanto o arquivo principal (Rascunho_Projeto1.pptx) quanto o anexo de apoio (Feedback_Prof.pdf).
As ações "Baixar" e "Visualizar" são botões de alto contraste, garantindo fácil acesso aos materiais.

Hierarquia de Ação:

- O botão "Abrir para Revisão" é o botão primário, com um ícone de olho (👁️) que reforça a natureza da tarefa. Ele guia o usuário para o próximo passo no fluxo de trabalho.
- O botão "Marcar como Não Aplicável" é o botão secundário, posicionado de forma discreta para não desviar a atenção da ação principal, mas acessível se necessário.
- O ícone de acessibilidade deve ser um elemento persistente no cabeçalho (header) de todos os viewports (telas de 1 a 8), mantendo-se como um recurso de sistema de alta prioridade. A navegação acionada deve levar diretamente ao frame 'Acessibilidade' (penúltima tela), que, por sua vez, deve ter um botão 'Salvar' que leva ao frame de confirmação 'Alterações Salvas com Sucesso!' (última tela).
Instruções Flexíveis: As instruções breves estão disponíveis, com o botão "Ver instruções completas" permitindo a expansão de detalhes sem sobrecarregar a tela.
<img width="237" height="523" alt="Captura de tela 2025-12-01 144148" src="https://github.com/user-attachments/assets/ca4df9e8-e754-4fde-b2fb-d479b97e0875" />



### 5. Enviar Artigo
Função:
Permitir que o usuário, Ana Beatriz, submeta seu artigo final, garantindo que todos os requisitos de formato e conteúdo sejam atendidos antes do envio.

Decisões de Usabilidade e Acessibilidade:
Prevenção de Erros (WCAG 3.3.4): A seção "Requisitos de Submissão" atua como um checklist obrigatório. O botão "Enviar Artigo Definitivo" é desabilitado (cinza) e só é habilitado em verde após o upload e a marcação dos requisitos, minimizando erros formais de submissão.

Upload Intuitivo: A área de upload com o ícone de nuvem e a borda tracejada oferece suporte a "arrastar e soltar" e é visualmente clara. O feedback de arquivo carregado ("Tese_Final_Ana.pdf") com a opção de "Remover" permite correção imediata.

Hierarquia Visual: O prazo está destacado, e as notas opcionais estão separadas, mantendo o foco do usuário no upload e no checklist.
<img width="392" height="851" alt="Tela 6" src="https://github.com/user-attachments/assets/b306d8fe-9fb6-473a-8299-1b44de608175" />


### 6. Registrar Presença
Função:
Oferecer um mecanismo de check-in simples e rápido para a presença da Ana Beatriz (conforme a necessidade da Persona P2), validando sua localização dentro de um raio permitido.

Decisões de Usabilidade e Acessibilidade:
Simplicidade e Rapidez (E1): O design é focado na ação de "CHECK-IN AGORA". O botão primário é grande, verde e imediatamente clicável, desde que a validação de localização seja positiva.

Clareza da Localização: A validação "✔ LOCALIZAÇÃO VÁLIDA" em verde fornece feedback visual imediato, essencial para tarefas sensíveis a localização. O ícone de localização reforça o contexto.

Contexto Temporal (E6): A data "Hoje é: Segunda-feira..." é exibida com destaque, informando imediatamente o usuário sobre o contexto da tarefa.

Organização: O link "Ver histórico de Presença" está convenientemente posicionado como um botão secundário para usuários organizados (como a Ana) que desejam conferir registros anteriores.
<img width="392" height="851" alt="Tela 7" src="https://github.com/user-attachments/assets/fe9ea190-e5de-4762-9e2b-1374761ef772" />


### 7. Relatório de Estágio
Função:
Gerenciar a submissão formal do Relatório de Estágio, que requer vários anexos e o cumprimento de requisitos específicos de formatação e conteúdo.
Decisões de Usabilidade e Acessibilidade:
Clareza de Fluxo: A tela é dividida em blocos lógicos (Instruções, Checklist, Upload), guiando o usuário passo a passo pela submissão.

Instruções Detalhadas: Os links "Ver Instruções Completas" e "Ver Regras de Formatação ABNT" permitem que a Ana acesse informações adicionais sem sobrecarregar a tela principal.

Múltiplos Uploads: A seção "Upload de Arquivo" distingue claramente entre o 1. Arquivo Principal e o 2. Anexo Obrigatório, resolvendo o desafio de submissão de múltiplos documentos. Cada botão de upload é rotulado para clareza.

Requisitos Formaiss: O "Checklist" garante que itens críticos (como a assinatura do supervisor) não sejam esquecidos, fundamental para relatórios de estágio.
<img width="392" height="851" alt="Tela 8" src="https://github.com/user-attachments/assets/d15c76ee-bbd8-4bf6-89c6-a1270ea408bb" />

### 8. Opções de Acessibilidade
Função:
Permitir que o usuário ajuste a interface do aplicativo para atender às suas necessidades visuais, cognitivas e de interação, tornando o aplicativo mais inclusivo e aderente às diretrizes WCAG.

Decisões de Usabilidade e Acessibilidade:
Organização por Categorias: A tela é claramente dividida em três categorias lógicas (Visualização e Contraste, Auxílio à Leitura, Interação e Tempo), facilitando a navegação e o entendimento rápido das opções.

- Visualização e Contraste:

Tamanho de Texto: Uso de slider (controle deslizante) para ajuste fino do tamanho da fonte, crucial para baixa visão.

Modo de Alto Contraste: Permite ativar o modo de contraste mais alto, garantindo legibilidade (idealmente contraste de 7:1 para texto grande e 4.5:1 para texto normal).

Modo Escuro (Dark Mode): Reduz o cansaço visual.

Desativar Animações: Evita confusão e desorientação para usuários com sensibilidade a movimentos (WCAG 2.3.3).

- Auxílio à Leitura:

Destaque de Foco para Teclado: Ativa um contorno visível (anel de foco) ao redor do elemento ativo, essencial para a navegação por teclado (WCAG 2.4.7).

Simplificar Rótulos de Botão: Melhora a experiência para usuários de leitores de tela ao reduzir a complexidade textual.

- Interação e Tempo:

Aumentar Área de Toque (Hit Area): Garante que a área de toque dos botões e links atinja o mínimo recomendado de 44×44px, auxiliando usuários com dificuldades motoras (WCAG 2.5.5).

Alertas de Tempo Estendido: Permite mais tempo para o usuário responder a mensagens ou janelas de sessão, evitando que a ação expire rapidamente (WCAG 2.2.1).

Componentes de Interface: O uso de Toggle Switches para as opções binárias (Ligado/Desligado) é intuitivo e padrão em interfaces móveis.

Ação Final: O botão "SALVAR ALTERAÇÕES" é o ponto focal da tela, e o link "Restaurar Configurações Padrão" permite o reset seguro das preferências.
<img width="392" height="851" alt="Acessibilidade" src="https://github.com/user-attachments/assets/24d5a9cf-cf5d-4865-8288-413ca19708b7" />


- Tela de Confirmação (Pós-Ação)
Função:
Essa tela é um feedback imediato, simples e inconfundível para o usuário, confirmando que uma ação importante (como salvar configurações, enviar um artigo, ou fazer um check-in) foi concluída com êxito.

Decisões de Usabilidade:
Clareza Imediata: O ícone de check em um círculo verde é um padrão universal de "Sucesso", garantindo que o usuário não tenha dúvidas sobre o resultado.

Foco na Ação: O texto "Alterações Salvas com Sucesso!" é breve e direto.

Ação de Saída: O único botão ativo é "Voltar para o Início", guiando o usuário de volta ao ponto principal de navegação para continuar seu trabalho.
<img width="392" height="851" alt="Acessibilidade-1" src="https://github.com/user-attachments/assets/52e5ff4e-aa91-4d51-bfa7-c8d986b3857b" />








