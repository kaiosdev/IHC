# Matriz CSD - Sistema de Gerenciamento de Projetos Acadêmicos UFAM

**Data da Reunião:** 07/11/2025
**Cliente:** Prof. Dr. Victor Celso (Farmacologia - UFAM)

---

## CERTEZAS

Informações confirmadas pelo briefing com Prof. Victor Celso:

* **C1. Interface deve ser prática, dinâmica e simples (clean):** O cliente espera algo "prático, dinâmico e simples [...] menos é mais".
* **C2. Foco principal no acompanhamento pós-aprovação de projetos:** A maior dor é a falta de ferramentas para gerenciar o projeto após aprovado ("Não tem um acompanhamento, não tem um lembrete").
* **C3. Sistema deve atender múltiplos tipos de projetos acadêmicos:** Deve cobrir PIBIC, PACE, PIBEX, PIBID, PIBIT e projetos de mestrado.
* **C4. Interface prioritária é para o professor orientador:** "No primeiro momento, pra mim [...] Só para eu conseguir fazer isso já estava maravilhoso".
* **C5. Acesso deve ser multiplataforma (desktop e mobile):** O cliente mencionou o uso "do seu computador de casa ou daqui" e "de qualquer lugar".
* **C6. Integração com e-Campus é desejável:** O cliente confirmou que a integração com o banco de dados do e-Campus "é muito melhor".
* **C7. Sistema deve ter templates pré-formatados específicos da UFAM:** O cliente vê grande valor em "Ter algo nativo, com essa linguagem nativa, que converse com o professor".
* **C8. Feed de atualizações de editais das pró-reitorias é necessário:** O cliente sugeriu ativamente "uma barra de atualizações dos mais novos editais [...] seria maravilhoso".
* **C9. Projetos frequentemente se relacionam entre si:** O cliente mencionou que tem "PIBICs que conversam com PIBIT".

---

## SUPOSIÇÕES

Hipóteses que precisam ser validadas:

* **S1.** Orientandos também se beneficiariam de um acesso (mesmo que secundário) ao sistema.
* **S2.** A maioria dos professores-orientadores da UFAM tem um nível de familiaridade tecnológica similar ao do Prof. Victor (uso de Trello, Notion, etc.).
* **S3.** O acesso mobile será usado para consultas rápidas, enquanto o desktop será usado para gerenciamento e cadastros.
* **S4.** O controle de presença de orientandos é uma funcionalidade essencial (Must-Have) e não apenas desejável (Should-Have).
* **S5.** Uma aplicação Web (PWA) é preferível a um aplicativo nativo (iOS/Android) devido à facilidade de acesso em múltiplos dispositivos (desktop/mobile).
* **S6.** A funcionalidade de "banco de dados de leis" deve ser gerenciável pelo próprio professor, permitindo que ele adicione as leis que mais utiliza.
* **S7.** A integração automática (leitura e escrita) com o sistema e-Campus é tecnicamente viável e existem APIs disponíveis para isso.

---

## DÚVIDAS

Questões que precisam ser esclarecidas:

* **D1.** Quais são exatamente os sites de pró-reitorias que o cliente consulta para editais (ele mencionou ProPESP, ProEST, mas parecia haver mais)?
* **D2.** Como funciona o fluxo técnico de submissão e aprovação no e-Campus? (Precisamos de um contato técnico).
* **D3.** Quais são os campos/colunas exatas que o professor utiliza hoje em suas "planilhas formatadas no Excel" para acompanhar os projetos? (Solicitar um exemplo).
* **D4.** Qual o volume médio de projetos simultâneos gerenciados por um professor?
* **D5.** Com que frequência exata o cliente busca por novos editais? (Ele disse "todos os dias", mas isso é literal?).
* **D6.** Para um MVP, quais pró-reitorias/tipos de projeto são a prioridade máxima? (Pesquisa? Extensão? Ensino?).
* **D7.** Quais são as restrições de segurança ou políticas de acesso (LGPD) para consultar dados do e-Campus?
* **D8.** O cliente mencionou a dificuldade em contatar as pró-reitorias "uma a uma". Uma funcionalidade de "contatos úteis" pré-cadastrados no app seria útil?
* **D9.** Como o cliente é notificado sobre a aprovação de um projeto atualmente? (Email? Portal?).
