📌 Projeto: API de Usuários com Node.js & Express<br>
📖 Descrição<br>
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

⚙️ Tecnologias<br>
Node.js<br>
Express.js<br>
MySQL (mysql2)<br>
bcrypt<br>
jsonwebtoken (JWT)<br>
express-rate-limit<br>
express-validator<br>
dotenv
<br>

🔒 Funcionalidades<br>
Cadastro de usuários com criptografia de senha<br>
Login com geração de token JWT<br>
Listagem de usuários<br>
Busca de usuário por ID<br>
Atualização de dados de usuário<br>
Remoção de usuário
<br>

🔒Middleware de segurança:<br>
Rate Limiting global<br>
Rate Limiting específico para login<br>
Sanitização e validação de inputs
<br>

📂 Estrutura
Código<br>
├── app.js<br>
├── routes/<br>
│ └── userRoutes.js<br>
├── controllers/<br>
│ └── userController.js<br>
├── models/<br>
│ └── db.js<br>
├── middlewares/<br>
│ ├── limiters.js<br>
│ └── validator.js<br>
└── package.json
<br>

🚀 Execução
Clone o repositório:<br>
bash<br>
git clone https://github.com/seu-usuario/API-de-Usuarios-com-ExpressJS.git
<br>

🟢Instale as dependências:<br>
bash<br>
npm install<br>
🟢Crie e Configure um arquivo .env:
<br>
Configure suas variáveis<br>
DB_HOST=localhost<br>
DB_USER=root<br>
DB_PASSWORD=sua_senha<br>
DB_NAME=seu_banco<br>
SECRET_KEY=sua_chave_secreta<br>

Inicie o servidor:
<br>
bash<br>
npm start<br>
Acesse:http://localhost:3000/users
<br>

📌 Endpoints<br>
Método Rota Descrição<br>
🟢POST /users/register Cadastro de usuário<br>
🟢POST /users/login Login e geração de token JWT<br>
🟢GET /users Listar todos os usuários<br>
🟢GET /users/:id Buscar usuário por ID<br>
🟢PUT /users/:id Atualizar usuário<br>
🟢DELETE /users/:id Remover usuário
<br>

🌟 Destaques Técnicos<br>
🟢Estrutura modular e organizada<br>
🟢Implementação de boas práticas de segurança (XSS, SQL Injection, brute force)<br>
🟢Middleware customizado para validação e limitação de requisições<br>
🟢Código limpo e de fácil manutenção<br>
