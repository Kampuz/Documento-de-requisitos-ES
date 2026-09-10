# Documento de Requisitos

## Sistema de Gerenciamento para Esccola de Línguas (Acadêmico e Comercial)

---

## 1. Introdução

### 1.1 Propósito do documento de requisitos

Este documento tem como propósito especificar os requisitos funcionais e não funcionais do Sistema de Gerenciamento para Escola de Línguas, referido durante o documento como "o Sistema". O documento serve como base de comunicação entre a equipe de desenvolvimento, gerentes e usuários finais, definindo de forma clara e objetiva o que o Sistema deve fazer, quais restrições deve respeitar e quais características de qualidade deve possuir.

O público-alvo deste documento inclui: equipe de desenvolvimento, potenciais usuários (professor da disciplina).

### 1.2 Escopo do produto

O Sistema tem como objetivo ser um gerenciador completo para escolas de línguas, contemplando tanto a **gestão acadêmica** (turmas, matrículas, frequuência, notas, professores) quanto a **gestão comercial** (contratos, mensalidades, cobranças, folha de pagamento, venda de materiais) do negócio.

**O Sistema visa**:

- Automatizar o processo de matrícula, rematrícula e transferência de alunos entre turmas;
- Controlar a alocação de turmas, salas e horários, evitando conflitos de agenda;
- Gerenciar o corpo docente, incluindo contratos, disponibilidade e remuneração;
- Acompanhar o desempenho acadêmico dos alunos (frequência, notas, histórico);
- Controlar o fluxo financeiro da escola (receitas, despesas, inadimplência, repasses);
- Fornecer portais de consulta para alunos e professores.

**Fora do escopo**: Disponibilização de tarefas e sistema de videoconferência próprio (a turma deve utilizar programas de terceiros), integração com gateways de pagamento externos e emissão fiscal.

### 1.3 Definições, acrônimos e abreviações

| Termo | Definição |
| --- | --- |
| RF | Requisito Funcional |
| RNF | Requisito Não Funcional |
| Aluno | Usuário matriculado em ao menos uma turma da escola |
| Turma | Agrupamento de alunos cursando um mesmo idioma/nível em um mesmo período/horário |

### 1.4 Refências

"IEEE Recommended Practice for Software Requirements Specifications," in IEEE Std 830-1998 , vol., no., pp.1-40, 20 Oct. 1998, doi: 10.1109/IEEESTD.1998.88286.
URL: <https://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=720574&isnumber=15571>

Documentação interna do projeto: "Ideias - Projeto ES II"
URL: <https://docs.google.com/document/d/1AZ7kweWREC_jZflhAPyJzU8V_zu19BsfQ1N4kGLYcsE/edit?tab=t.0>

### 1.5 Visão geral do restante do documento

A Seção 2 apresenta uma descrição geral do produto, contextualizando-o dentro do ambiente em que será utilizado, suas principais funcionalidades, os perfis de usuário esperados e as restrições e suposições consideradas.
A seção 3 detalha os requisitos funcionais e não funcionais específicos do sistema, organizados por módulo e por ator. As seções finais trazem apêndices e o índice do documento.

---

## 2. Descrição Geral

### 2.1 Perspectiva do Produto

### 2.2 Funcionalidade do Produto

### 2.3 Características do Usuário

| Ator | Perfil | Principais responsabilidades no sitema |
| --- | --- | --- |
| Administrador/ Secretário | Usuário administrativo, sem necessidade de conhecimento técnico avançado; familiaridade com rotinas de secretaria escolar | Gerenciar cursos, turmas, salas, horários, matrículas, cadastros e lista de espera |
| Professor | Conhecimento básico de informática; foco pedagógico | Consultar turmas/ horários, registrar frequência e notas, informar disponibilidade |
| Financeiro | Usuário administrativo com conhecimento de rotinas financeiras/ contábeis básicas | Definir preços e planos, controlar cobranças e inadimplência, gerenciar folha de pagamento, gerar relatórios |
| Aluno | Público geral | Consultar plano de ensino, calendário, notas, faltas, pagamentos |

### 2.4 Restrições Gerais

### 2.5 Suposições e Dependências

## 3. Requisitos Específicos

### 3.1 Requisitos Funcionais

- **RF-XX (NOME)** - O Sitema deve permitir algo acontecer.

### 3.2 Requisitos Não Funcionais

- **RNF-01 (Segurança)** - **[TODO]**
- **RNF-02 (Usabilidade)** - A interface deve ser utilizável por usuários sem conhecimento técnico avançado, especialmente nos perfis Administrador, Professor e Aluno.
- **RNF-03 (Desempenho)** - Operações de consulta (ex.: verificação de conflito de horário) devem ser processadas em tempo aceitável, evitando bloqueios perceptíveis ao usuário.
- **RNF-04 (Disponibilidade)** - **[TODO]**
- **RNF-05 (Confiabilidade)** - O Sistema não deve permitir inconsistências como duplo agendamento do mesmo professor ou sala no mesmo horário.
- **RNF-06 (Manutenibilidade)** - O Sistema deve ser estruturado de forma modular, permitindo evolução independente dos módulos acadêmicos e financeiro.
- **RNF-07 (Compatibilidade)** - O Sistema deve ser acessível para computadores que possuam JAVA XX.

## 4. Apêndices

*[Apêndices]*

## 5. Índice

[1 Introdução](#1-introdução)
[1.1 Propósito do documento de requisitos](#11-propósito-do-documento-de-requisitos)
[1.2 Escopo do produto](#12-escopo-do-produto)
[1.3 Definições, acrônimos e abreviações](#13-definições-acrônimos-e-abreviações)
[1.4 Referências](#14-refências)
[1.5 Visão geral do restante do documento](#15-visão-geral-do-restante-do-documento)
[2 Descrição Geral](#2-descrição-geral)
[2.1 Perspectiva do Produto](#21-perspectiva-do-produto)
[2.2 Funcionalidade do Produto](#22-funcionalidade-do-produto)
[2.3 Características do Usuário](#23-características-do-usuário)
[2.4 Restrições Gerais](#24-restrições-gerais)
[2.5 Suposições e Dependências](#25-suposições-e-dependências)
[3. Requisitos Específicos](#3-requisitos-específicos)
[4. Apêndices](#4-apêndices)
[5. Índice](#5-índice)
