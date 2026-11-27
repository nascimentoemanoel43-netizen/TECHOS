# User Stories — TechOS

## US01 — Autenticação no Sistema
- **Como** técnico de suporte,
- **Quero** realizar login com e-mail e senha,
- **Para que** eu possa acessar o painel restrito de Ordens de Serviço de forma segura.

### Critérios de Aceitação (BDD)
- **Cenário 1:** Login bem-sucedido
  - **Dado** que o usuário está na tela de login,
  - **Quando** insere credenciais válidas e clica em "Entrar",
  - **Então** o sistema autentica o usuário e redireciona para o Dashboard principal.

- **Cenário 2:** Credenciais inválidas
  - **Dado** que o usuário está na tela de login,
  - **Quando** insere uma senha incorreta,
  - **Então** o sistema exibe uma mensagem de erro informando "Credenciais inválidas".

---

## US02 — Abertura de Ordem de Serviço (OS)
- **Como** atendente da TechServices,
- **Quero** registrar uma nova Ordem de Serviço informando o cliente, o equipamento e o defeito relatado,
- **Para que** o problema possa ser encaminhado para a equipe técnica.

### Critérios de Aceitação (BDD)
- **Cenário 1:** Cadastro de OS com sucesso
  - **Dado** que o atendente acessa o formulário de nova OS,
  - **Quando** preenche todos os campos obrigatórios e clica em "Salvar",
  - **Então** a OS é gerada com status "Aberta" e um número de identificação único.
  ---

## US03 — Listagem e Filtro de Ordens de Serviço
- **Como** técnico de suporte ou atendente,
- **Quero** visualizar a lista de todas as Ordens de Serviço com opções de filtro por status,
- **Para que** eu possa localizar rapidamente os chamados pendentes ou concluídos.

### Critérios de Aceitação (BDD)
- **Cenário 1:** Filtrar OS por status "Aberta"
  - **Dado** que o usuário está na tela de gerenciamento de OS,
  - **Quando** seleciona o filtro "Abertas",
  - **Então** o sistema exibe apenas as ordens de serviço correspondentes a esse status.

---

## US04 — Atualização de Status da Ordem de Serviço
- **Como** técnico responsável,
- **Quero** atualizar o status de uma Ordem de Serviço (ex: de "Aberta" para "Em Andamento" ou "Concluída"),
- **Para que** o andamento do atendimento seja transparente para toda a equipe.

### Critérios de Aceitação (BDD)
- **Cenário 1:** Alteração de status bem-sucedida
  - **Dado** que o técnico visualiza os detalhes de uma OS aberta,
  - **Quando** altera o status para "Em Andamento" e clica em salvar,
  - **Então** o sistema atualiza o registro no banco de dados e exibe a mensagem de sucesso.