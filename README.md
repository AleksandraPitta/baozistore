# 🥟 Baozi Store

Uma API REST para organizar clientes, produtos e pedidos de uma pequena loja de pão chinês, unindo a tradição do baozi com a modernidade do matcha.

Projeto desenvolvido para a disciplina de **Desenvolvimento Web Back-End** (ADS, UNINTER).

## Tecnologias

- Java 21
- Spring Boot
- Spring Data JPA
- Banco de dados H2 (em memória)
- Maven
- Testes feitos no Postman

  ## Diagrama de caso de uso

  <img width="600" alt="diagrama-caso-de-uso" src="https://github.com/user-attachments/assets/08ea3c36-8f54-4bbc-aeb4-f4f1bb305554" />


## 🚀 Como rodar

Com o projeto aberto na pasta, rode:

```bash
./mvnw spring-boot:run
```

A API sobe em `http://localhost:8080`.

O console do banco fica em `http://localhost:8080/h2-console`
(JDBC URL: `jdbc:h2:mem:baozistore`, usuário `sa`, senha vazia).

## Endpoints

| Método | URL | O que faz |
|---|---|---|
| POST | `/produtos` | cadastra um produto |
| GET | `/produtos` | lista os produtos |
| GET | `/produtos/{id}` | busca um produto pelo id |
| DELETE | `/produtos/{id}` | apaga um produto |

O mesmo vale para `/clientes` e `/pedidos`.

## Exemplo

`POST /produtos`

```json
{
  "nome": "Baozi de Matcha",
  "preco": 9.99,
  "estoque": true
}
```

## Autora

Aleksandra Fernandes Pitta — Análise e Desenvolvimento de Sistemas, UNINTER.
