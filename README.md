📌 Projeto: API de Usuários com Node.js & Express
📖 Descrição
Este projeto consiste em uma API RESTful desenvolvida em Node.js utilizando o framework Express, integrada a um banco de dados MySQL.
O sistema implementa autenticação com JWT, criptografia de senhas com bcrypt, proteção contra ataques de força bruta com rate limiting e boas práticas de segurança como sanitização e validação de entradas.

## 📸 API Demonstration

### Server Running

![Server Running](assets/server-running.png)

### User Registration

![User Registration](assets/postman-register.png)

### User Login (JWT)

![User Login](assets/postman-login.png)

### User READ

![User READ](assets/postman-READ.png)

⚙️ Tecnologias
Node.js
Express.js
MySQL (mysql2)
bcrypt
jsonwebtoken (JWT)
express-rate-limit
express-validator
dotenv

🔒 Funcionalidades
Cadastro de usuários com criptografia de senha
Login com geração de token JWT
Listagem de usuários
Busca de usuário por ID
Atualização de dados de usuário
Remoção de usuário
Middleware de segurança:
Rate Limiting global
Rate Limiting específico para login
Sanitização e validação de inputs

📂 Estrutura
Código
├── app.js
├── routes/
│ └── userRoutes.js
├── controllers/
│ └── userController.js
├── models/
│ └── db.js
├── middlewares/
│ ├── limiters.js
│ └── validator.js
└── package.json

🚀 Execução
Clone o repositório:
bash
git clone https://github.com/seu-usuario/nome-do-projeto.git

Instale as dependências:
bash
npm install
Crie e Configure um arquivo .env:

Código
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=sua_senha
DB_NAME=seu_banco
SECRET_KEY=sua_chave_secreta
Inicie o servidor:

bash
npm start
Acesse:

Código
http://localhost:3000/users
📌 Endpoints
Método Rota Descrição
POST /users/register Cadastro de usuário
POST /users/login Login e geração de token JWT
GET /users Listar todos os usuários
GET /users/:id Buscar usuário por ID
PUT /users/:id Atualizar usuário
DELETE /users/:id Remover usuário

🌟 Destaques Técnicos
Estrutura modular e organizada
Implementação de boas práticas de segurança (XSS, SQL Injection, brute force)
Middleware customizado para validação e limitação de requisições
Código limpo e de fácil manutenção
