# 📦 Projeto Exemplo Arquitetura Hexagonal

Projeto Java com Spring Boot utilizando **Arquitetura Hexagonal (Ports and Adapters)** para promover uma separação clara de responsabilidades, facilitar testes e garantir maior manutenibilidade do código.

---

## 📚 Sobre o Projeto

Este projeto é uma aplicação básica desenvolvida com o framework **Spring Boot**, estruturada segundo os princípios da **arquitetura hexagonal**, também conhecida como **Ports & Adapters**. Essa abordagem permite desacoplar as regras de negócio dos detalhes de infraestrutura, como banco de dados, APIs externas e interfaces web.

---

## 🧱 Estrutura do Projeto

```bash
src/
└── main/
    ├── java/
    │   └── com/seuempresa/projeto/
    │       ├── application/         # Casos de uso
    │       ├── domain/              # Entidades e lógica de negócio
    │       ├── adapters/            # Implementações de entrada/saída (ex: REST, DB, etc.)
    │       │   ├── in/              # Adaptadores de entrada (controllers, schedulers, etc.)
    │       │   └── out/             # Adaptadores de saída (repositories, clientes, etc.)
    │       ├── ports/               # Interfaces (driven/driver ports)
    │       └── config/              # Configurações Spring Boot
    └── resources/
        └── application.yml         # Configurações da aplicação

🚀 Como Executar
Pré-requisitos
Java 17+

Maven 3.8+

IDE: IntelliJ

# Build do projeto
mvn clean install

# Executar a aplicação
mvn spring-boot:run

🧪 Testes
Para rodar os testes:

mvn test

📌 Principais Tecnologias
Java 17

Spring Boot

Spring Web

Spring Data JPA

H2 Database (ou outro)

Maven

JUnit 5

🧠 Conceitos Utilizados
Arquitetura Hexagonal (Ports and Adapters)

SOLID Principles

Separação de responsabilidades

Testabilidade elevada

Inversão de dependência

👤 Autor
Willian Massuki Maeda

📝 Licença
Este projeto está licenciado sob a Licença MIT - veja o arquivo LICENSE para detalhes.

