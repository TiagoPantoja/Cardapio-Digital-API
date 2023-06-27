# Cardápio Digital API
 
Este é um projeto Java desenvolvido com o framework Spring Boot para gerenciar um cardápio de alimentos. O projeto consiste em uma API REST que permite salvar e recuperar informações sobre alimentos.

## Tecnologias utilizadas

- Java 17
- Spring Boot 3.1
- Spring Data JPA 3.1.1
- HATEOAS
- PostgreSQL

## Pré-requisitos

- JDK 8 ou superior
- Maven

## Configuração

1. Clone o repositório do projeto: `git clone https://github.com/seu-usuario/cardapio.git`
2. Navegue até o diretório raiz do projeto: `cd cardapio`
3. Compile o projeto com o Maven: `mvn compile`
4. Execute o projeto: `mvn spring-boot:run`

A API estará disponível em `http://localhost:8080/food`.

## Endpoints

### POST /food

Salva as informações de um alimento no cardápio.

**Requisição**

- Corpo (JSON):
{
  "title": "Nome do Alimento",
  "image": "URL da Imagem",
  "price": 10
}

### Resposta

Código de status: 200 (OK)
### GET /food
Recupera todos os alimentos do cardápio.

### Resposta

Código de status: 200 (OK)
Corpo (JSON):
{
  "title": "Nome do Alimento",
  "image": "URL da Imagem",
  "price": 10
}

### Resposta

Código de status: 200 (OK)
### GET /food
Recupera todos os alimentos do cardápio.

### Resposta

Código de status: 200 (OK)
Corpo (JSON):
[
  {
    "id": 1,
    "title": "Nome do Alimento",
    "image": "URL da Imagem",
    "price": 10
  },
  {
    "id": 2,
    "title": "Outro Alimento",
    "image": "URL da Imagem",
    "price": 15
  },
  ...
]

## Contribuição
Contribuições são bem-vindas! Se você encontrar algum problema ou tiver alguma sugestão, sinta-se à vontade para abrir uma issue ou enviar um pull request.
