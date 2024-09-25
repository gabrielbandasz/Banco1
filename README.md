# Banco1
```
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