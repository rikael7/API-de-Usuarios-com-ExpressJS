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

🔐 User Authentication API
API REST desenvolvida em Node.js para gerenciamento de usuários, com foco em segurança, boas práticas e autenticação JWT.
Este projeto implementa um CRUD completo de usuários com proteção contra ataques comuns como SQL Injection, XSS, Brute Force e DoS, além de criptografia de senhas.

🚀 Tecnologias Utilizadas
Node.js
Express
MySQL
bcrypt
JSON Web Token (JWT)
express-validator
express-rate-limit
dotenv

📌 Funcionalidades
Cadastro de usuários
Login com autenticação JWT
Listagem de usuários
Busca por ID
Atualização de dados
Remoção de usuários
Criptografia de senha
Validação de dados

Proteção contra:
SQL Injection
XSS
Brute Force
DoS
Emails duplicados

🔒 Segurança Implementada

Hash de senha com bcrypt
Queries parametrizadas (SQL Injection)
Sanitização de inputs (XSS)
Rate Limit global (DoS)
Rate Limit específico para login (Brute Force)
Validação de dados com express-validator
Variáveis de ambiente para dados sensíveis

⚙️ Configuração do Ambiente

Crie um arquivo .env na raiz do projeto:
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=12345
DB_NAME=sistema_cadastro
SECRET_KEY=sua_chave_secreta

📦 Instalação
npm install

▶️ Executar o projeto
node app.js

Servidor rodando em:
http://localhost:3000

📚 Rotas da API
🔹 Cadastro de usuário
POST /users/register
{
  "nome": "João",
  "email": "joao@email.com",
  "senha": "123456"
}

🔹 Login
POST /users/login
{
  "email": "joao@email.com",
  "senha": "123456"
}

🔹 Listar usuários
GET /users
🔹 Buscar usuário por ID
GET /users/:id
🔹 Atualizar usuário
PUT /users/:id
{
  "nome": "Novo Nome",
  "email": "novo@email.com"
}
🔹 Remover usuário
DELETE /users/:id

🗄️ Estrutura do Projeto
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


📈 Objetivo do Projeto
Este projeto foi desenvolvido para:
Praticar APIs REST
Aplicar conceitos de segurança
Demonstrar boas práticas de backend
Servir como portfólio para vagas de Desenvolvedor Júnior

👨‍💻 Autor

Rikael Ribeiro
Desenvolvedor em formação focado em backend, segurança e boas práticas.

⭐ Considerações Finais
Este projeto demonstra:
✔ Organização de código
✔ Segurança
✔ Boas práticas
✔ Conhecimento real de backend

Ideal para portfólio e entrevistas técnicas.
