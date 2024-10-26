Banco de dados MY SQL

Usuários: para gerenciar o login e os dados do usuário.
Transações: para armazenar receitas e despesas, com detalhes de valor e data de vencimento.
Saldo: para controlar o saldo atual e o dinheiro guardado.

Estrutura das Tabelas

Tabela Usuarios
Esta tabela conterá as informações de login e dados básicos dos usuários que acessam a área administrativa.

Colunas:
UsuarioID: Identificador único do usuário.
Nome: Nome completo do usuário.
Email: Email para login, deve ser único.
Senha: Senha criptografada para segurança.
DataCriacao: Data e hora de criação do usuário.

-------------------------------------------------------------------------------------------
Tabela Transacoes
Essa tabela armazenará as receitas e despesas, incluindo valores e datas de vencimento.

Colunas:
TransacaoID: Identificador único da transação.
Tipo: Indica se a transação é uma receita (Credito) ou despesa (Debito).
Descricao: Descrição da transação (ex: "Moto").
Valor: Valor da transação.
DataVencimento: Data de vencimento da transação.
UsuarioID: Relacionamento com a tabela Usuarios para identificar o usuário a que a transação pertence.

-------------------------------------------------------------------------------------------
Tabela Saldo
A tabela Saldo pode ser usada para armazenar o saldo atual e o dinheiro guardado de cada usuário.

Colunas:
SaldoID: Identificador único do saldo.
SaldoAtual: Saldo atual do usuário.
DinheiroGuardado: Valor guardado pelo usuário.
UsuarioID: Relacionamento com a tabela Usuarios para associar o saldo ao usuário.