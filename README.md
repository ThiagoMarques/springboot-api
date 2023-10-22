# API de Usuários

Esta é uma API de exemplo para gerenciamento de usuários feita com Maven para uma API REST usando Spring Boot 3.1.5 e Java 17. 
Além das dependências principais, inclui o Swagger para documentação da API. 
Ela permite a realização de operações CRUD (Create, Read, Update, Delete) em registros de usuários. 

## Utilização

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

