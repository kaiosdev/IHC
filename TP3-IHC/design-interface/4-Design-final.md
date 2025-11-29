# E-Project - Sistema de Gestão de Projetos Acadêmicos UFAM

[![Status](https://img.shields.io/badge/status-em%20desenvolvimento-yellow)]()
[![Licença](https://img.shields.io/badge/licen%C3%A7a-MIT-green)]()

##  Sobre o Projeto

O **E-Project** é um sistema de gestão acadêmica desenvolvido especificamente para a Universidade Federal do Amazonas (UFAM), focado no gerenciamento e acompanhamento de projetos de pesquisa, extensão e ensino.

("https://www.figma.com/design/lLDopNGZcEgvP0ihCUu2W0/E-Project?node-id=0-1&t=hEyeKuFrlvNCNUQj-1")


###  Objetivo

Criar uma solução **prática, dinâmica e simples** que elimine o retrabalho de adaptação exigido por ferramentas genéricas (como Trello ou Excel), oferecendo um sistema pré-configurado com as características específicas dos projetos da UFAM.

##  Interfaces do Sistema

### Tela de Login
<img width="874" height="1702" alt="Tela de Login do E-Project" src="https://github.com/user-attachments/assets/a7bd9d1f-174c-4f28-9653-b406f52c8498"/>

A tela inicial do E-Project apresenta:
- Logo institucional da UFAM
- Identificação do sistema "E-Project"
- Opções de acesso diferenciadas:
  - **Orientador**: Para professores e coordenadores
  - **Orientando**: Para alunos e bolsistas
- Sistema específico para projetos: PIBIC, PACE, Pibex, PIBID e Mestrado

### Dashboard do Orientador

<img width="958" height="810" alt="Dashboard do E-Project" src="https://github.com/user-attachments/assets/790f45c0-59a5-4693-84e3-b1edcd0dde3f" />
<img width="630" height="876" alt="Captura de tela 2025-11-28 200321" src="https://github.com/user-attachments/assets/6532bc62-b25e-43c3-8158-24b5ad076a5f" />

O painel do orientador oferece uma visão completa com:

**Métricas Principais:**
- Total de Projetos (6)
- Projetos em Andamento (4)
- Projetos Concluídos (0)
- Projetos Atrasados (1)

**Funcionalidades:**
-  **Ver Editais**: Acesso a 3 novos editais disponíveis
-  **Controle de Presença**: Registro específico de presença dos orientandos
-  **Novo Projeto**: Cadastro rápido de projetos

**Filtros por Tipo:**
- Todos
- PIBIC
- PACE
- Pibex
- PIBID
- Mestrado

**Lista de Projetos Ativos:**
Cada projeto exibe:
- Nome e descrição
- Status (tag colorida)
- Orientador responsável
- Datas de início e término
- Pró-reitoria vinculada
- Progresso visual (%)
- Número do edital

### Dashboard do Orientando

<img width="809" height="821" alt="Captura de tela 2025-11-28 200356" src="https://github.com/user-attachments/assets/eeb4d84d-4ff9-43d4-af55-e4982e5ea54f" />

<img width="512" height="554" alt="Captura de tela 2025-11-28 200409" src="https://github.com/user-attachments/assets/0728dfa5-3330-4067-8f35-a0ec83abc8c5" />

O painel do orientando apresenta:

**Informações Centralizadas:**
- Nome do projeto vinculado
- Orientador responsável
- Acesso aos editais das Pró-Reitorias

**Filtros de Visualização:**
- Todas
- Propesp (Pesquisa)
- Proext (Extensão)
- Proeg (Ensino)
- Proplan (Planejamento)

**Status das Atividades:**
- Total de Editais (8)
- Editais Abertos (5)
- Encerramento em Breve (3)
- Novos (últimos 7 dias) (0)

**Lista de Editais Disponíveis:**
Cada edital mostra:
- Tipo (PIBIC, PACE, Pibex, PIBID)
- Título do programa
- Descrição resumida
- Data de publicação
- Prazo final (destacado em vermelho quando próximo)
- Pró-reitoria responsável
- Número do edital
- Botão "Acessar Edital"

##  Funcionalidades Principais

### Para Orientadores
-  Gestão completa de projetos acadêmicos
-  Acompanhamento de progresso em tempo real
-  Controle de presença específico para bolsistas
-  Visualização integrada de projetos relacionados
-  Envio de demandas aos orientandos
-  Dashboard com métricas e indicadores
-  Filtros por tipo de projeto e pró-reitoria

### Para Orientandos
-  Visualização de tarefas e demandas
-  Acompanhamento do próprio progresso
-  Acesso centralizado aos editais abertos
-  Notificações de prazos importantes
-  Interface simplificada e intuitiva

### Centralização de Editais
-  Agregação automática de editais das pró-reitorias
-  Notificações de novos editais
-  Links diretos para documentação oficial
-  Alertas de prazos próximos ao vencimento

##  Tipos de Projetos Suportados

| Tipo | Descrição | Pró-Reitoria |
|------|-----------|--------------|
| **PIBIC** | Programa Institucional de Bolsas de Iniciação Científica | Propesp |
| **PACE** | Programa de Apoio à Cultura e Extensão | Proext |
| **Pibex** | Programa Institucional de Bolsas de Extensão | Proext |
| **PIBID** | Programa Institucional de Bolsas de Iniciação à Docência | Propesp |
| **Mestrado** | Programas de Pós-Graduação Stricto Sensu | Propesp |

##  Diferenciais

###  Especificidade UFAM
- Sistema pré-configurado com as características dos projetos da UFAM
- Elimina retrabalho de adaptação de ferramentas genéricas
- Nomenclaturas, fluxos e processos alinhados com as normativas institucionais

###  Integração Planejada
- **E-campus**: Sincronização de atualizações e relatórios
- **Sites das Pró-Reitorias**: Importação automática de editais
- Conformidade com SEI e sistemas oficiais

###  Controle de Acesso
- **Nível Orientador**: Acesso total e gestão completa
- **Nível Orientando**: Acesso restrito focado em tarefas e demandas

##  Problemas Resolvidos

| Problema | Solução E-Project |
|----------|-------------------|
| Ferramentas genéricas sem especificidade | Sistema customizado para UFAM |
| Retrabalho de adaptação | Pré-configuração inteligente |
| E-campus/SEI sem acompanhamento | Dashboard com métricas e progresso |
| Dispersão de informações | Centralização de editais |
| Múltiplos acessos diários | Portal único integrado |

##  Paleta de Cores

- **Verde Institucional**: `#1B5E20` (cor principal UFAM)
- **Verde Claro**: `#4CAF50` (destaques e ações positivas)
- **Azul Escuro**: `#1565C0` (informações e links)
- **Amarelo**: `#FDD835` (alertas e destaques)
- **Vermelho**: `#D32F2F` (prazos críticos)
- **Cinza**: `#424242` (textos secundários)


##  Público-Alvo

### Primário
- **Professores/Orientadores**: Gestão completa de projetos e equipes

### Secundário
- **Alunos/Orientandos**: Acompanhamento de tarefas e demandas
- **Coordenadores**: Visão estratégica dos programas

**E-Project** - Gestão Acadêmica Inteligente para a UFAM 

*Universidade Federal do Amazonas - Simplificando a gestão de projetos acadêmicos*# Design Final - E-Project

<div align="center">
