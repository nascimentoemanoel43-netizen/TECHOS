# Estimativas de Esforço — TechOS (Planning Poker / Fibonacci)

Este documento registra a pontuação de esforço atribuída às User Stories do TechOS utilizando a escala modificada de Fibonacci (1, 2, 3, 5, 8, 13 pontos de história).

## Quadro de Pontuação das User Stories

| ID | User Story | Complexidade | Risco | Pontos (Fibonacci) | Justificativa |
| :--- | :--- | :--- | :--- | :---: | :--- |
| **US01** | Autenticação de Usuário (Login) | Média | Médio | **5** | Envolve criptografia de senha (hash) e controle de sessão por token JWT. |
| **US02** | Abertura de Ordem de Serviço | Baixa | Baixo | **3** | Formulário padrão com inserção direta em tabela relacional do MySQL. |
| **US03** | Listagem e Filtro de OS | Baixa | Baixo | **3** | Consultas SQL com parâmetros `WHERE` simples e renderização em tabela HTML. |
| **US04** | Atualização de Status da OS | Média | Baixo | **3** | Operação de edição (UPDATE) com validação de regras de transição de status. |
| **US05** | Cadastro de Clientes e Equipamentos| Baixa | Baixo | **2** | Telas e tabelas cadastrais simples com relacionamento básico de chave estrangeira. |
| **US06** | Relatório Básico de OS | Média | Médio | **5** | Requer agregações SQL (`COUNT`, `GROUP BY`) e exibição de métricas consolidadas. |

## Resumo do Planejamento
- **Total de Pontos do Bloco 1 (Backlog Inicial):** 21 pontos de história.
- **Média por História:** ~3.5 pontos, indicando um bom fracionamento das tarefas para o padrão técnico do curso do SENAI.