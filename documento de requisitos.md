# Documento de Requisitos

## Sistema de Gerenciamento para Escola de Línguas (Acadêmico e Comercial)

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

- **RF-01** - O sistema deve permitir o cadastro de alunos, contendo nome, documentos, idade, contato e, quando aplicável, dados do responsável legal.
- **RF-02** - O sistema deve permitir o cadastro de professores, incluindo idiomas que podem lecionar, dados pessoais e dados contratuais.
- **RF-03** - O sistema deve permitir o cadastro de funcionários administrativos e financeiros.
- **RF-04** - O sistema deve exigir o cadastro de um responsável legal para alunos menores de idade.
- **RF-05** - O sistema deve permitir o cadastro de idiomas e seus respectivos níveis (A1, A2, I1, I2, B1, B2).
- **RF-06** - O sistema deve permitir o registro de resultado de teste de nivelamento para alunos que desejam ingressar em nível diferente do inicial.
- **RF-07** - O sistema deve permitir a criação de turmas por período/semestre, definindo idioma, nível e modalidade (presencial, online ou híbrido).
- **RF-08** - O sistema deve permitir a alocação de sala a uma turma, verificando a capacidade máxima de alunos.
- **RF-09** - O sistema deve verificar conflitos de horário de sala e de professor antes de confirmar a alocação de uma turma.
- **RF-10** - O sistema deve inserir automaticamente o aluno em lista de espera quando a turma desejada atingir capacidade máxima.
- **RF-11** - O sistema deve notificar o próximo aluno da lista de espera quando surgir uma vaga.
- **RF-12** - O sistema deve permitir ao professor registrar frequência diária dos alunos.
- **RF-13** - O sistema deve permitir ao professor registrar notas e avaliações pedagógicas.
- **RF-14** - O sistema deve permitir ao professor disponibilizar atividades, avaliações e conteúdos pedagógicos.
- **RF-15** - O sistema deve permitir ao professor informar e atualizar sua disponibilidade de dias e horários.
- **RF-16** - O sistema deve manter o histórico acadêmico do aluno, incluindo turmas cursadas, notas, faltas e documentos emitidos.
- **RF-17** - O sistema deve aplicar critérios de aprovação (nota mínima e frequência mínima) definidos para cada turma/curso.
- **RF-18** - O sistema deve permitir a emissão de certificado de conclusão para alunos aprovados.
- **RF-19** - O sistema deve permitir o registro de matrícula de um aluno em uma turma, validando existência de vaga, idade mínima e resultado de nivelamento (quando aplicável).
- **RF-20** - O sistema deve permitir rematrícula do aluno para o período/semestre seguinte.
- **RF-21** - O sistema deve permitir a transferência de um aluno entre turmas, respeitando as mesmas validações da matrícula.
- **RF-22** - O sistema deve impedir nova matrícula de aluno inadimplente.
- **RF-23** - O sistema deve permitir ao Financeiro definir planos de pagamento, valores de mensalidade e taxas de matrícula.
- **RF-24** - O sistema deve permitir o controle de recebimentos, cobranças e identificação de inadimplência.
- **RF-25** - O sistema deve permitir a aplicação de descontos (pontualidade, convênios, parentesco entre alunos).
- **RF-26** - O sistema deve permitir a gestão da folha de pagamento/repasse a professores, por hora/aula ou valor fixo.
- **RF-27** - O sistema deve permitir o registro de venda de materiais didáticos e controle básico de estoque.
- **RF-28** - O sistema deve gerar relatórios de receita, despesas, conversão e evasão de alunos.
- **RF-29** - O sistema deve permitir consulta, por parte do professor, ao próprio extrato de horas/aulas e valores a receber.
- **RF-30** - O sistema deve permitir ao aluno consultar seu plano de ensino e calendário de aulas.
- **RF-31** - O sistema deve permitir ao aluno consultar suas faltas, presenças e notas.
- **RF-32** - O sistema deve permitir ao aluno consultar sua situação de pagamento.
- **RF-33** - O sistema deve permitir ao aluno visualizar informações de semestres futuros (quando disponíveis).
- **RF-34** - O sistema deve permitir ao aluno acessar atividades disponibilizadas pelo professor.
- **RF-35** - O sistema deve disponibilizar ao aluno uma área de links (sala virtual, grupo da turma, materiais, provas).

### 3.2 Requisitos Não Funcionais

- **RNF-01 (Usabilidade)** - A interface deve ser utilizável por usuários sem conhecimento técnico avançado, especialmente nos perfis Administrador, Professor e Aluno.
- **RNF-02 (Desempenho)** - Operações de consulta (ex.: verificação de conflito de horário) devem ser processadas em tempo aceitável, evitando bloqueios perceptíveis ao usuário.
- **RNF-03 (Confiabilidade)** - O Sistema não deve permitir inconsistências como duplo agendamento do mesmo professor ou sala no mesmo horário.
- **RNF-04 (Manutenibilidade)** - O Sistema deve ser estruturado de forma modular, permitindo evolução independente dos módulos acadêmicos e financeiro.
- **RNF-05 (Compatibilidade)** - O Sistema deve ser acessível para computadores que possuam JAVA XX.

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
