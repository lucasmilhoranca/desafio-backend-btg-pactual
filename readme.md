<p align="center" width="100%">
    <img width="50%" src="./image/btg-logo.jpg"> 
</p>


<h3 align="center">
  Desafio Backend do BTG Pactual
</h3>

<p align="center">

  <img alt="License: MIT" src="https://img.shields.io/badge/license-MIT-%2304D361">
  <img alt="Language: Java" src="https://img.shields.io/badge/language-java-green">
  <img alt="Version: 1.0" src="https://img.shields.io/badge/version-1.0-yellowgreen">

</p>

## Desafio
- Confira o enunciado completo, [clicando aqui](problem.md).

## Como interagir com o banco de dados?
- Utilizamos o [MongoDB Compass](https://www.mongodb.com/products/tools/compass)

## Como interagir com a API?
- Utilizei o [Httpie](https://github.com/httpie)

:mag: Baixe o projeto e teste você mesmo na prática.

## :rocket: Tecnologias utilizadas

* Java 21
* Spring Boot
* Spring Data MongoDB
* RabbitMQ
* Docker

### Integração de Spring Boot com RabbitMQ e MongoDB:

- Criar um microserviço com Spring Boot
- Consumir uma fila do RabbitMQ
- Comunicar com o banco de dados MongoDB via Docker
- Mapear uma collection do MongoDB dentro do Spring
- Fazer aggregations no MongoDB com Spring
- Efetuar logs com o SLF4J

### Lista de tarefas:

**Introdução**:

- [x]  Qual é o desafio que vamos resolver?

---

**Comunicação com o banco e dados**:

- [x]  Iniciando o projeto Java (Web, Data MongoDB, RabbitMQ)
- [x]  Configurando o RabbitMQ e MongoDB no Docker
- [x]  Configurando a comunicacao do Spring Boot com o MongoDB
- [x]  Configurando a criacao da fila no RabbitMQ

---

**Funcionalidade de Consumo de Pedidos**:

- [x]  Mapear as entidades (Order, OrderItem)
- [x]  Criar o listener da fila do RabbitMQ
- [x]  Criar a implementação para salvar o pedido no MongoDB
- [x]  Testar o fluxo (rabbitmq → spring → mongodb)

---

**Funcionalidade de disponibilizar as informações via API**:

- [x]  Lembre-se, a API deverá informar:
    - Lista de pedidos realizados por cliente
    - Valor total de um pedido
    - Quantidade de pedidos por cliente
- [x]  Criar endpoint (estruturar DTO de retorno)
- [x]  Criar serviço de listagem de pedidos do cliente
- [x]  Criar serviço que calcula o valor total de todos os pedidos do cliente
- [x]  Testar a API