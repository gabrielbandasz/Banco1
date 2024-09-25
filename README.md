# Banco1
```sql
-- Exercícios 25/09
-- Gabriel Prade Bandasz
```

```sql
-- criar tabela clientes
create table Clientes1(
id_cliente int primary key,
nome_cliente varchar (100),
email_cliente varchar (150),
data_nascimento date,
telefone_cliente varchar (15)
);
```

```sql
-- criar tabela produtos
create table produtos1(
id_produto int primary key,
nome_produto varchar (100),
preco_produto decimal (8,2)
);
```

```sql
-- criar tabela faturas
create table faturas(
id_fatura int primary key,
data_criacao date,
valor_fatura decimal (10,2)
);
```



```sql
-- criar tabela faturas
create table faturas(
id_fatura int primary key,
data_criacao date,
valor_fatura decimal (10,2)
);
```

```sql
-- criar tabela clientes
create table Clientes1(
id_cliente int primary key,
nome_cliente varchar (100),
email_cliente varchar (150),
data_nascimento date,
telefone_cliente varchar (15)
);
```

```sql
-- criar tabela produtos
create table produtos1(
id_produto int primary key,
nome_produto varchar (100),
preco_produto decimal (8,2)
);

-- renomear nome_produto para descricao_produto
alter table produtos1 rename column nome_produto to descricao_produto;
```

```sql
-- criar tabela Funcionarios
create table Funcionarios(
id_funcionarios int primary key,
nome_funcionario varchar (100),
sobrenome_funcionario varchar (150),
salario_funcionario decimal (10,2)
);

-- adicionar coluna data_nascimento
alter table Funcionarios add data_nascimento date;

-- adicionar a coluna IDDepartamento
alter table Funcionarios add id_departamento int;

-- renomear sobrenome para apelido
alter table Funcionarios rename column sobrenome_funcionario to apelido_funcionario;


-- adicionar a coluna id_enderecos
alter table Funcionarios add id_enderecos int;
```

```sql
-- criar tabela Departamentos
create table Departamentos(
id_departamentos int primary key,
nome_departamentos varchar (100)
);
```

```sql
-- criar tabela Projetos
create table Projetos(
id_projetos int primary key,
nome_projeto varchar (100)
);

-- adicionar coluna id_clientes
alter table Projetos add id_clientes int;
```

```sql
-- criar tabela alocacoes
create table Alocacoes(
id_alocacoes int primary key,
id_funcionario int,
id_projeto int
);
```

```sql
-- criar tabela Clientes2
create table Clientes2(
id_clientes int primary key,
nome_clientes varchar (100)
);

-- renomear nome_clientes para nome_empresa
alter table Clientes2 rename column nome_clientes to nome_empresa;
```

```sql
-- criar tabela Enderecos
create table Enderecos(
id_enderecos int primary key,
rua_enderecos varchar (150),
cep_enderecos int (8),
cidade_enderecos varchar (100)
);
```

```sql
-- criar tabela Pedidos
create table Pedidos(
id_pedidos int primary key,
data_pedidos int
);

-- adicionar coluna id_cliente
alter table Pedidos add id_cliente int;
```

```sql
-- criar tabela ItensPedidos
create table ItensPedidos(
id_itped int primary key,
id_pedido int,
id_produtos int
);
```

```sql
-- criar tabela estoque
create table estoques(
id_estoques int primary key,
quantidade_estoques int
);

alter table Estoques add id_produto int;
```

```sql
-- criar tabela vendas
create table vendas(
id_vendas int primary key,
dataVenda date
);

alter table vendas add id_cliente2 int;
```