## TP3-IHC - Benchmarking

O objetivo desta etapa é realizar uma análise comparativa (benchmarking) de soluções existentes – tanto genéricas (utilizadas pelo cliente) quanto oficiais – para mapear as lacunas de funcionalidade e confirmar a viabilidade da proposta de valor.

Com base no briefing com o Professor Victor Celso, o problema central é a falta de uma ferramenta específica para a gestão de projetos acadêmicos da UFAM, o que o força a usar ferramentas genéricas que exigem muito retrabalho de adaptação.


**a) Avaliação dos Critérios de Comparação**

Com base na demanda, os itens definidos para comparação foram:

- **Gestão de Projetos:** Capacidade de organizar visualmente e acompanhar a evolução de tarefas.
- **Especificidade Acadêmica (UFAM):** Se a ferramenta possui modelos prontos e terminologia nativa para projetos da UFAM (PIBIC, PACE, Pibex, etc.).
- **Retrabalho de Adaptação:** O esforço necessário para o usuário configurar a ferramenta para a "linguagem UFAM" (criação de tags, planilhas, cabeçalhos, etc.).
- **Centralização de Editais:** Capacidade de agregar informações e links externos (como os sites das Pró-Reitorias) em um feed unificado.
- **Integração (E-campus):** Potencial de integração ou sincronização com outros sistemas de banco de dados oficiais.
- **Portabilidade:** Qualidade da experiência de uso em múltiplos dispositivos (Desktop e Mobile).


**b) Definição dos Similares-alvo**

Os produtos, organizações ou serviços selecionados como referência foram:

- **Sistema 1:** Trello - Ferramenta de gestão visual de projetos baseada em quadros Kanban.
- **Sistema 2:** Notion - Ferramenta flexível "tudo-em-um" que combina anotações, bancos de dados e gestão de projetos.
- **Sistema 3:** Google Sheets / Excel - Ferramentas de planilhas. Representam a alternativa manual de organização de dados.
- **Sistema 4:** E-campus / SEI - Sistemas oficiais da UFAM. Analisados para confirmar a lacuna de funcionalidade de "acompanhamento".


**c) Obtenção e Análise de Dados**

Abaixo está a análise detalhada de cada similar-alvo em relação à sua capacidade de resolver o problema do cliente:

<div align="center">
  
### Sistema 1 - Trello

| Critério | Descrição da Solução | Análise de Destaque |
|:--:|:--:|:--:|
| **Problemas Resolvidos** | Organização visual de tarefas e fluxo de trabalho simples, permitindo acompanhamento de status e colaboração. | Funciona bem para fluxos genéricos. |
| **Como é Resolvido** | Sistema de Quadros (Boards), Listas (Lists) e Cartões (Cards), seguindo o princípio do Kanban. | Utiliza metodologia visual (Kanban) de baixo atrito. |
| **Pontos Fortes** | Excelente Portabilidade (desktop e mobile), interface intuitiva, e curva de aprendizado baixa. | Design focado na simplicidade e uso rápido. |
| **Pontos Fracos** | Totalmente Genérico (Exige 100% de adaptação manual); não possui modelos acadêmicos nativos; não centraliza editais; nenhuma integração com E-campus. | Representa a dificuldade do "Retrabalho de Adaptação" citada pelo cliente. |

<i> Teste visual do Trello, mostrando como o sistema organiza tarefas em quadros e cartões, ilustrando sua abordagem de gestão visual e simplicidade de uso.<br>
[Teste 1 - Trello](https://drive.google.com/file/d/1HtChSaSEovoB4zJeHdFwBWghB0K8SwFR/view)
</i>

---

### Sistema 2 - Notion

| Critério | Descrição da Solução | Análise de Destaque |
|:--:|:--:|:--:|
| **Problemas Resolvidos** | Necessidade de um espaço de trabalho unificado, combinando documentos, bancos de dados e gestão de tarefas. | Alta flexibilidade para documentação e estruturação de dados. |
| **Como é Resolvido** | Páginas flexíveis, bases de dados relacionais e templates altamente personalizáveis. | Permite a construção de estruturas complexas, como os modelos que o cliente precisa, mas de forma manual. |
| **Pontos Fortes** | Extremamente poderoso, flexível e permite excelente resultado estético e funcional se dedicado tempo à configuração. | Potencial para criar modelos personalizados. |
| **Pontos Fracos** | Curva de Aprendizado Alta e o "Retrabalho de Adaptação" é ainda maior que o do Trello; não fala a "linguagem UFAM" nativamente; não integra com E-campus. | A flexibilidade exige um investimento de tempo inicial elevado. |

<i> Exploração no Notion, destacando sua estrutura flexível baseada em páginas e bancos de dados, destacando sua flexibilidade e poder de personalização, mas com curva de aprendizado elevada.<br>
[Teste 2 - Notion](https://drive.google.com/file/d/1Abf5II5S3ccQUV5DuTh9HmDlD8XNGDHH/view)
</i>

--- 
  
### Sistema 3 - Google Sheets / Excel

| Critério | Descrição da Solução | Análise de Destaque |
|:--:|:--:|:--:|
| **Problemas Resolvidos** | Organização de dados estruturados em formato de tabela, possibilitando cálculos, cruzamento e registro de informações detalhadas. | Excelente para dados brutos e cálculos. |
| **Como é Resolvido** | Células, fórmulas e formatação condicional, criando planilhas para monitoramento manual. | Ferramenta universalmente acessível. |
| **Pontos Fortes** | Amplamente conhecido e acessível. | Baixo custo e alta disponibilidade. |
| **Pontos Fracos** | Representação literal do "retrabalho manual"; não é uma ferramenta de gestão, mas de registro; Interface péssima para acompanhamento visual de projetos; Portabilidade mobile ruim para gestão. | Fracasso total nos critérios de gestão e acompanhamento. |

<i> Captura de exemplo do uso de planilhas como ferramenta de organização, evidenciando sua funcionalidade tabular e limitações em termos de acompanhamento visual.<br>
[Teste 3 - Google Sheets / Excel](https://drive.google.com/file/d/1vaJGYmzOp-kHph4Q4XFrOts3XRcfMTNj/view)
</i>

---
  
### Sistema 4 - E-campus / SEI

| Critério | Descrição da Solução | Análise de Destaque |
|:--:|:--:|:--:|
| **Problemas Resolvidos** | Registro, protocolo e tramitação oficial de processos e documentos dentro da universidade. | Garante a conformidade legal e institucional. |
| **Como é Resolvido** | Formulários de cadastro e sistemas de protocolo eletrônico. | Fluxo oficial de submissão. |
| **Pontos Fortes** | É o sistema oficial de registro, garantindo a conformidade legal e a Integração com o banco de dados institucional. | Único com alta Especificidade Acadêmica. |
| **Pontos Fracos** | Não oferece nenhuma funcionalidade de acompanhamento ou gestão da evolução do projeto. Não tem boa portabilidade ou interface visual de gestão. | Não cumpre o requisito central de acompanhamento. |

<i>Registro da interface do sistema institucional E-campus/SEI, ilustrando sua função de protocolo e gestão documental dentro do ambiente acadêmico da UFAM.<br>
[Teste 4 - E-campus / SEI](https://drive.google.com/file/d/1z9lZNQDUpmRZssG66xTVjfOHfCrcGR1u/view?usp=drive_open)
</i>
</div>

---


**d) Matriz de Comparação Consolidada**

A matriz a seguir consolida a avaliação dos similares-alvo, focada nos requisitos levantados no briefing:

| Similar | Gestão de Projetos (Visual) | Especificidade Acadêmica (Nativa) | Evita Retrabalho de Adaptação | Centralização de Editais | Integração (E-campus) | Portabilidade (Mobile/Desktop) |
|:--:|:--:|:--:|:--:|:--:|:--:|:--:|
| **Sistema 1 (Trello)** | ✅ | ❌ | ❌ | ❌ | ❌ | ✅ |
| **Sistema 2 (Notion)** | ✅ | ❌ | ❌ | ❌ | ❌ | ✅ |
| **Sistema 3 (Planilhas)** | ❌ | ❌ | ❌ | ❌ | ❌ | ✅ |
| **Sistema 4 (E-campus/SEI)** | ❌ | ✅ | ✅ | ❌ | ✅ | ❌ |

---

<div align="center">

  ### Análise visual comparativa (benchmarking) dos principais sistemas<br> utilizados como referência durante o projeto.
  
  <img src="https://drive.google.com/uc?export=view&id=1rjRHymP0w5uybTaa4EiMRJ_tyyDIpnJm" width="70%">
  <p><i>Análise visual do Trello, evidenciando sua eficiência em fluxos genéricos,<br>
    porém com alta necessidade de adaptação à realidade acadêmica.</i></p>

  <img src="https://drive.google.com/uc?export=view&id=1FNnAuR_0tQ8IsMefED8h5WVBS8BuxSDf" width="70%">
  <p><i>Benchmarking do Notion, destacando sua flexibilidade e poder de personalização, <br>mas com curva de aprendizado elevada e ausência de integração institucional.</i></p>

  <img src="https://drive.google.com/uc?export=view&id=1Fhn3PM8mIVUNgMglbVfgidrsM-H-t-pP" width="70%">
  <p><i>Visualização da análise do Google Sheets/Excel, ressaltando sua força em manipulação de dados <br>e fraqueza em gestão visual e acompanhamento de projetos.</i></p>

  <img src="https://drive.google.com/uc?export=view&id=1dQuX-ehzg9A8GhShMTJ2fORP1NQCstfv" width="70%">
  <p><i>Imagem ilustrando a avaliação do E-campus/SEI, demonstrando sua adequação legal e acadêmica,<br> mas limitações em portabilidade e acompanhamento visual de processos.</i></p>

  <img src="https://drive.google.com/uc?export=view&id=1byIr0xLhxjp9faYe0jzmP2_FD9aXPPUU" width="70%">
  <p><i>Tabela consolidada do benchmarking, comparando de forma direta os sistemas analisados com base <br>nos critérios definidos no briefing. A matriz evidencia as lacunas de integração e especificidade acadêmica,<br> reforçando a necessidade de uma solução personalizada para o contexto da UFAM.</i></p>

</div>

---

<div align="center">

### Conclusão do Benchmarking
</div>

A análise comparativa confirma de forma robusta a lacuna identificada pelo cliente. Existe uma dissociação crítica no mercado de ferramentas:

**Ferramentas Genéricas (Trello, Notion):** Excelentes em Gestão de Projetos e Portabilidade, mas falham na Especificidade Acadêmica e Evitar Retrabalho (exigem 100% de configuração manual).

**Sistemas Oficiais (E-campus):** Excelentes em Especificidade e Integração, mas falham miseravelmente em Gestão de Projetos e Portabilidade (não oferecem acompanhamento).

O resultado valida plenamente a oportunidade de mercado para o produto proposto, que deve combinar a **Gestão de Projetos de baixo atrito** com a **Especificidade Acadêmica nativa da UFAM**, resolvendo o problema central de retrabalho e melhorando a experiência móvel para o client. Esta conclusão será a base para a definição da solução (Etapa 4).
