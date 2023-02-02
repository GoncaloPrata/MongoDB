# Notas

## Getting Started with MongoDB Atlas

### Lesson 1

Quando se usa o Atlas para guardar os nossos dados, os dados estão replicados em vários servers. Eles chamam
a isto "Replica Set". Isto significa que os dados estão guardados em vários servers, e que em caso de falha,
não ficamos sem assesso a eles.

Existem 2 tipos de bases de dados no Atlas:

1. Serverless -> é escalável consoante a procura e cobra consoante os recursos que são utilizados. Adequadas para
aplicações que têm workload espaçado
2. Cluster -> é composto por vários servidores a trabalharem em conjunto. existem 2 tipos de clusters:
   - Shared ->  são menores e incluem uma opção free e boa opção para quem está a começar
   - Dedicates -> melhor para aplicações de produção com mais features

Quando estamos a fazer deploy podemos usar AWS, Google Cloud ou Azure por exemplo.

### Lesson 2

Quando criamos uma conta fazemos parte de uma organização.
Uma organização é um grupoo que define os seus utilizadores e equipas, esta organização também concede acessos
aos projetos.

## Overview of MongoDB and the Document Model

### Lesson 1


MongoDb é uma General Purpose Document Database que estrutura dados em documenots em vez de tabelas relacionais.

Documento Model -> easier to plan how application data will corresponde to data in the database

Document -> unidade básica de MongoDB

Collection -> grupos de documentos, que não têm de ter exatamente a mesma estrutura

Database -> container de coleções


### Lesson 2

Enquanto que os dados visualmente são guardados em JSON, são guardados no formato BSON

Um JSON como na verdade é um BSON na verdade pode guardar vários tipos de objetos tais como:
1. string
2. boolean
3. object
4. array
5. null
6. dates
7. numbers
8. object id's -> tipo de objeto especial para criar identificadores de objetos unicos

Todos os documentos precisam de um campo "_id" que atua como chave primária, caso não exista, então,
a MongoDB automaticamente gera um campo "_id"

Documentos dentro duma mesma coleção podem conter campos diferentes entre si e os campos em comum podem ter
diferentes tipos de dados. Por isso, se for necessário, é possível inserir documentos com novos schemas diretamente
na coleção. É possível também adicionar validação de schema com regras quanto a estrutura do documento

**Estrutura de um Documento**:

Syntax:
``` json
{
   "key": value,
   "key": value,
   "key" : value
}
```
Example:

``` json

{
   "_id": 1,
   "name": "AC3 Phone",
   "colors" : ["black", "silver"],
   "price" : 200,
   "available" : true
}
```