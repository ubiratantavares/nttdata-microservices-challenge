# 📦 Desafio Técnico NTT DATA - Microserviços com Spring Boot e Spring Cloud

Este projeto foi desenvolvido como parte do desafio técnico da NTT DATA em parceria com a DIO. O objetivo é construir uma aplicação baseada em microserviços utilizando Spring Boot e Spring 
Cloud, aplicando conceitos modernos de arquitetura como Service Discovery, API Gateway, comunicação entre serviços e autenticação simplificada.

## 🧩 Arquitetura do Sistema

O sistema é composto por:

- **Service Discovery**: Eureka Server para registro e descoberta de serviços.

- **API Gateway**: Spring Cloud Gateway para roteamento e autenticação.

- **Produtos Service**: Microserviço para gerenciamento de produtos.

- **Pedidos Service**: Microserviço para simulação de pedidos.


![Arquitetura](images/arquitetura.png)

## 🚀 Tecnologias Utilizadas

- Java 17

- Spring Boot

- Spring Cloud (Eureka, Gateway)

- Spring Web

- Spring Data JPA

- H2 Database

- Spring Security

- Maven

## 📁 Estrutura do Repositório

nttdata-microservices/ ├── api-gateway/ ├── service-discovery/ ├── produtos-service/ ├── pedidos-service/ ├── images/ └── README.md


## 🔐 Autenticação

Todas as requisições devem conter um token fixo no header:

Authorization: Bearer meu-token-secreto


O API Gateway valida esse token antes de redirecionar para os microserviços.

