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