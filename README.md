# API de Usuários

Esta é uma API de exemplo para gerenciamento de usuários feita com Maven para uma API REST usando Spring Boot 3.1.5 e Java 17. 
Além das dependências principais, inclui o Swagger para documentação da API. 
Ela permite a realização de operações CRUD (Create, Read, Update, Delete) em registros de usuários. 

## Endpoints

### Listar Usuários

- **Método:** GET
- **Rota:** /users
- **Descrição:** Retorna a lista de todos os usuários cadastrados.

### Obter um Usuário

- **Método:** GET
- **Rota:** /users/{username}
- **Descrição:** Retorna os detalhes de um usuário específico com base no nome de usuário.

### Deletar Usuário

- **Método:** DELETE
- **Rota:** /users/{id}
- **Descrição:** Exclui um usuário com base no ID fornecido.

### Criar Usuário

- **Método:** POST
- **Rota:** /users
- **Descrição:** Cria um novo usuário com base nos dados fornecidos no corpo da solicitação.

### Atualizar Usuário

- **Método:** PUT
- **Rota:** /users
- **Descrição:** Atualiza os detalhes de um usuário com base nos dados fornecidos no corpo da solicitação.

## Utilização

Aqui estão alguns exemplos de como utilizar os endpoints desta API:

- **Listar Usuários:**

  ```http
  GET /users

- **Obter um Usuário::**

  ```http
  GET /users/{username}

- **Deletar Usuário:**

  ```http
  DELETE /users/{id}

- **Criar Usuários:**

  ```http
  POST /users
Content-Type: application/json
{
    "login": "user",
    "password": "senha",
}
- **Atualizar Usuários:**

  ```http
  PUT /users
Content-Type: application/json
{
    "login": "user",
    "password": "senha",
}

