## TP3-IHC - Parte 1: Imersão e Definição

 
### 1. Matriz CSD - Sistema de Gerenciamento de Projetos Acadêmicos UFAM

  Após o briefing, a equipe se reuniu para organizar as informações coletadas em uma Matriz CSD. O objetivo desta etapa, conforme o documento do trabalho, é categorizar os principais tópicos do projeto para guiar a investigação futura.

A matriz construída pela equipe foi a seguinte:

| CERTEZAS (C) | SUPOSIÇÕES (S) | DÚVIDAS (D) |
| :---: | :---: | :---: |
| **C1.** O usuário principal é o **professor/orientador** (Interface prioritária). | **S1.** Outros professores da UFAM têm dificuldade de "adaptar" ferramentas genéricas similares ao do cliente. | **D1.** Para o MVP, qual a prioridade máxima? (Projetos de Pesquisa vs. Extensão? Acompanhamento de projetos existentes vs. feed de novos editais?). |
| **C2.** O **acompanhamento pós-aprovação** (gestão, lembretes), já que os sistemas atuais (E-campus, SEI) não servem para isso. | **S2.** Orientandos se beneficiariam de um acesso, mas essa interface **não** é prioritária para o MVP. | **D2.** Como funciona o fluxo técnico de submissão/aprovação no e-Campus? A integração de *envio* (escrita) é tecnicamente viável? Quais as restrições de segurança/LGPD? |
| **C3.** A interface deve ser **prática, dinâmica e simples (clean)**, pois ferramentas genéricas (Trello, Notion) causam retrabalho de adaptação. | **S3.** O acesso **mobile** será usado para consultas rápidas, e o **desktop** para gerenciamento e cadastros. | **D3.** Quais são os campos/colunas exatas das planilhas Excel atuais? Quais são exatamente os campos/etapas "pré-setados" que diferenciam um PIBIC de um PACE? (Solicitar exemplos). |
| **C4.** O sistema deve cobrir **múltiplos tipos de projetos** acadêmicos (PIBIC, PACE, PIBEX, PIBID, PIBIT, mestrado). | **S4.** Uma aplicação Web (PWA) é preferível a um aplicativo nativo (iOS/Android) pela facilidade de acesso multiplataforma. | **D4.** Quais são *exatamente* os sites de pró-reitorias consultados para editais (ProPESP, ProEST, etc.)? |
| **C5.** O acesso deve ser **multiplataforma (desktop e mobile)**, garantindo portabilidade. | **S5.** A integração automática (API de leitura) com o e-Campus é tecnicamente viável. | **D5.** Como funciona o "compêndio de normas"? Quais são as 5 leis/normas mais cruciais que o professor precisa ter à mão? |
| **C6.** Necessidade de **templates pré-formatados específicos da UFAM** ("linguagem nativa"). | **S6.** É tecnicamente viável fazer *scraping* nos sites das 3+ Pró-Reitorias para alimentar o feed de editais. | **D6.** Qual o volume médio de projetos simultâneos gerenciados por um professor? |
| **C7.** Necessidade de um **feed de atualizações de editais** das pró-reitorias. | **S7.** O controle de presença de orientandos é essencial (Must-Have) e pode ser um "check-in" semanal, mais simples que um controle diário. |**D7.** Como o cliente é notificado sobre a aprovação de um projeto atualmente (Email? Portal?)? |
| **C8.** A integração (leitura) com o banco de dados do **e-Campus** é desejável. | | **D8.** Uma funcionalidade de "contatos úteis" (pró-reitorias) pré-cadastrados no app seria útil? |
| **C9.** Projetos frequentemente se relacionam entre si (ex: "PIBICs que conversam com PIBIT"). | 
---
### 2. Evidência Matriz CSD

**Data da Reunião:** 07/11/2025

**Cliente:** Prof. Dr. Victor Celso

<div align="center">
  <img src="https://drive.google.com/uc?export=view&id=1a7NX6mCmLLov9DRWuJgqq2WNF3Ct4Zhb" width="70%">
  <p><i>Registro da reunião de equipe durante a construção da Matriz CSD (Certezas, Suposições e Dúvidas). O grupo discutiu coletivamente as percepções sobre o projeto, identificando pontos consolidados, hipóteses a validar e aspectos que ainda requerem esclarecimento. Essa etapa foi fundamental para alinhar o entendimento entre os participantes e direcionar as próximas fases do desenvolvimento da solução.</i></p>
</div>
