# Backend de Registro e Login com Token

Este projeto implementa um backend para autenticação de usuários utilizando SQLite e tokens JWT para segurança.

## Tecnologias Utilizadas
- Node.js
- Express
- SQLite
- JWT (JSON Web Token)
- bcrypt para hash de senhas

## Funcionalidades
- Registro de novos usuários
- Login de usuários registrados
- Geração de token JWT para autenticação
- Proteção de rotas utilizando middleware

## Instalação e Execução
1. Clone o repositório:
   ```sh
   git clone https://github.com/Jusenx/backend-Registro-e-Login-com-Token.git
   ```
2. Acesse o diretório do projeto:
   ```sh
   cd backend-Registro-e-Login-com-Token
   ```
3. Instale as dependências:
   ```sh
   npm install
   ```
4. Execute o servidor:
   ```sh
   node index.js
   ```

## Uso da API

### Registro de Usuário
**Endpoint:** `POST /register`
**Payload:**
```json
{
  "username": "exemplo",
  "password": "senha123"
}
```

### Login de Usuário
**Endpoint:** `POST /login`
**Payload:**
```json
{
  "username": "exemplo",
  "password": "senha123"
}
```
**Resposta:**
```json
{
  "token": "seu_token_aqui"
}
```

### Rota Protegida (Exemplo)
**Endpoint:** `GET /profile`
**Cabeçalho:** `Authorization: Bearer seu_token_aqui`

## Contribuição
Sinta-se à vontade para contribuir com melhorias e correções. Para isso, faça um fork do repositório, crie uma branch e envie um pull request.

## Licença
Este projeto está sob a licença MIT.

