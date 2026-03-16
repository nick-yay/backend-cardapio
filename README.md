# Cardápio Digital — Back-end

API REST para gerenciamento de cardápio digital, desenvolvida com Java e Spring Boot.

## Tecnologias

- Java 17
- Spring Boot 3.5
- Spring Data JPA
- PostgreSQL
- Lombok
- Docker

## Endpoints

| Método | Endpoint | Descrição |
|--------|----------|-----------|
| GET | /food | Lista todos os produtos |
| POST | /food | Cadastra novo produto |

## Como rodar localmente

### Pré-requisitos
- Java 17
- PostgreSQL rodando na porta 5432

### Configuração

Edite o `src/main/resources/application.properties` com suas credenciais:

```properties
spring.datasource.url=jdbc:postgresql://localhost:5432/food
spring.datasource.username=seu_usuario
spring.datasource.password=sua_senha
```

### Executando

```bash
./mvnw spring-boot:run
```

A API estará disponível em `http://localhost:8080`.

## Como rodar com Docker

Consulte o repositório [cardapio-docker](https://github.com/nick-yay/cardapio-docker) para rodar o projeto completo com Docker Compose.

## Front-end

[cardapio-frontend](https://github.com/nick-yay/cardapio-frontend)
