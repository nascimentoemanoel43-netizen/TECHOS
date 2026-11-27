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