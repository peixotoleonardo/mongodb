# Mongo

> O Mongo é um banco de dados NoSQL que armazena documentos.

## O que é um Documento

É uma estrutura de dados composta por pares de chave/valor.

Eles são similares a objetos JSON. Os valores dos campos podem
ser de qualquer tipo suportado pelo MongoDB incluindo outros documentos
e arrays.

### Vantagens do Uso

- Os documentos correspondem a tipos de dados nativos em muitas
  linguagens de programação.
- Documentos e arrays aninhados reduzem a necessidade de JOINs.
- O esquema dinâmico suporta polimorfismo fluente.

## Collections

É onde o Mongo guarda os documentos, elas são análogas as tabelas
nos bancos de dados relacionais.

Além de collections, o MongoDB suporta:

- Read-only Views (à partir da versão 3.4)
- On-Demand Materialized Views (à partir da versão 4.2)

## Features Importantes

### Alta Performance

MongoDB fornece persistência de dados de alto desempenho.
Em particular,

- O suporte para modelos de dados incorporados reduz a
  atividade I/O no sistema de banco de dados.
- Os índices suportam consultas mais rápidas e podem
  incluir chaves de documentos aninhados e arrays.


### API de Consulta

A API de consulta do MongoDB suporta operações de leitura
e escrita assim como:

- Agregação de dados
- Pesquisa de texto e consultas geoespaciais.
  
### Alta Disponibilidade

A funcionalidade de replicação do MongoDB, chamada de replica set,
provê:

- failover automático
- redundância de dados

Um replica set é um grupo de servidores MongoDB que mantém o mesmo
conjunto de dados, fornecendo redundância e aumentando a disponibilidade
de dados.

### Escalonamento Horizontal

MongoDB provê escalonamento horizontal como parte da funcionalidade
principal:

- O sharding distribui dados em um cluster de máquinas.
- À partir da versão 3.4, o MongoDB suporta a criação de zonas de dados
  com base na shard key. Em um cluster balanceado, o MongoDB redireciona
  leituras e gravações cobertas por uma zona apenas para os shards
  dentro da zona.

### Suporte a Vários Mecanismos de Armazenamento

- Mecanismo de armazenamento WiredTiger
- Mecanismo de armazenamento em memória

Além desses, o MongoDB fornece API de mecanismo de armazenamento conectável
que permite que terceiros desenvolvam mecanismos de armazenamento para o
MongoDB.
