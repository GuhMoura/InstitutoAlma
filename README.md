<p align="center">
  <a href="https://www.fecap.br/">
    <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/4/4a/Fecap-logo.png/320px-Fecap-logo.png" alt="FECAP - Fundação de Comércio Álvares Penteado" width="150">
  </a>
</p>

<h1 align="center">Site Institucional - Instituto Alma</h1>

<p align="center">
  <img src="https://placehold.co/800x400/111F44/C5FFEE?text=Projeto+Instituto+Alma" alt="Banner do Projeto Instituto Alma" width="100%">
</p>

<p align="center">
  <img src="http://img.shields.io/static/v1?label=STATUS&message=EM%20DESENVOLVIMENTO&color=GREEN&style=for-the-badge" alt="Status Development">
  <img src="https://img.shields.io/static/v1?label=License&message=CC%20BY%204.0&color=blue&style=for-the-badge" alt="License">
</p>

## 👥 Global SI - Integrantes

| Nome | LinkedIn |
|------|----------|
| **Gustavo Moura** | [<img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" />](https://www.linkedin.com/in/gustavomoura3112) |
| **Lucas Corsino** | [<img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" />](https://www.linkedin.com/in/lucas-soares-corsino-885306288/) |
| **Guilherme Gomes Salvadeo** | - |
| **Manoel Rondon** | [<img src="https://img.shields.io/badge/LinkedIn-0077B5?style=flat&logo=linkedin&logoColor=white" />](https://www.linkedin.com/in/manoel-rondon) |

### 👨‍🏫 Professores Orientadores
* **Eduardo Savino Gomes**
* **Francisco de Souza Escobar**
* **José Carlos Buesso Junior**
* **Ronaldo Araujo Pinto**
* **Victor Bruno Alexander Rosetti de Quiroz**

---

## 📖 Descrição

Este projeto é um site institucional completo para o **Instituto Alma**, uma organização sem fins lucrativos focada em *"promover o desenvolvimento humano e a inclusão social por meio de ações educativas e de solidariedade"*.

Desenvolvido como **Projeto Integrado (PI)** do curso de Análise e Desenvolvimento de Sistemas da **FECAP**, o objetivo é criar um portal digital funcional, moderno e impactante.

### ✨ Funcionalidades Principais
* 🏢 **Institucional:** Apresentação da história, missão e valores.
* 📅 **Eventos:** Divulgação de atividades e agenda.
* 💰 **Doações:** Captação de recursos transparente.
* 🔐 **Portal:** Login/Cadastro para doadores e administradores.
* 🗣️ **Ouvidoria:** Canal direto de comunicação.

---

## 🚀 Tecnologias Utilizadas

O projeto é uma aplicação **Full-Stack**, dividida em Frontend (React) e Backend (Node.js/API).

| Área | Tecnologias |
|------|-------------|
| **Frontend** | ![React](https://img.shields.io/badge/react-%2320232a.svg?style=flat&logo=react&logoColor=%2361DAFB) ![Vite](https://img.shields.io/badge/vite-%23646CFF.svg?style=flat&logo=vite&logoColor=white) ![CSS3](https://img.shields.io/badge/css3-%231572B6.svg?style=flat&logo=css3&logoColor=white) |
| **Backend** | ![NodeJS](https://img.shields.io/badge/node.js-6DA55F?style=flat&logo=node.js&logoColor=white) ![Express.js](https://img.shields.io/badge/express.js-%23404d59.svg?style=flat&logo=express&logoColor=%2361DAFB) ![JWT](https://img.shields.io/badge/JWT-black?style=flat&logo=JSON%20web%20tokens) |
| **Banco de Dados** | ![MySQL](https://img.shields.io/badge/mysql-4479A1.svg?style=flat&logo=mysql&logoColor=white) ![Azure](https://img.shields.io/badge/azure-%230072C6.svg?style=flat&logo=microsoftazure&logoColor=white) |

---

## 🛠 Estrutura de Pastas

```bash
📁 PI - Atualizado/
│
├── 📁 instituto-alma-api/       (Backend - Node.js)
│   ├── 📁 middleware/           # Autenticação (JWT)
│   ├── 📄 .env                  # Credenciais (Azure/JWT)
│   ├── 📄 db.js                 # Conexão MySQL + SSL
│   └── 📄 server.js             # Rotas principais
│
└── 📁 instituto-alma-react/     (Frontend - React)
    ├── 📁 public/               # Assets estáticos
    └── 📁 src/
        ├── 📁 components/       # Componentes reutilizáveis
        ├── 📁 layouts/          # Layouts (Admin, Auth, Public)
        ├── 📁 pages/            # Telas do sistema
        └── 📄 App.jsx           # Configuração de Rotas
------------------------------------------------------------------------

⚙️ Instalação e Configuração
Nota: Este projeto requer dois terminais rodando simultaneamente.

Pré-requisitos
Node.js v18+
Git
MySQL Workbench

1. Clonar o Repositório
git clone https://[URL-DO-SEU-REPOSITORIO].git
cd [NOME-DA-PASTA-DO-PROJETO]

2. Configurar o Backend (Terminal 1)
cd instituto-alma-api
npm install

Configuração do .env:Crie um arquivo .env na pasta instituto-alma-api e insira:
DB_HOST="institutoalmasql.mysql.database.azure.com"
DB_USER="seu_usuario_admin_do_azure"
DB_PASSWORD="sua_senha_do_azure"
DB_NAME="instituto_alma"
JWT_SECRET="sua-chave-secreta-muito-segura"

Em seguida, execute npm run dev para iniciar a A
PI.3. Configurar o Frontend (Terminal 2)
cd instituto-alma-react
npm install
npm run dev

4. AcessoO projeto estará disponível em: http://localhost:5173
🗺️ Rotas da API (Endpoints)
🔓 Rotas Públicas
Método,Rota,Descrição
POST,/api/auth/register,Cadastro de Doador
POST,/api/auth/login,Login (Retorna JWT)
GET,/api/atividades,Lista atividades
POST,/api/ouvidoria,Envia mensagem
🔒 Rotas Protegidas (Admin)
Método,Rota,Descrição
POST,/api/atividades,Cria nova atividade
GET,/api/admin/doacoes,Relatório de doações
GET,/api/ouvidoria,Lê mensagens recebidas
🔒 Rotas Protegidas (Doador)
Método,Rota,Descrição
GET,/api/perfil,Dados do usuário
GET,/api/doador/doacoes,Histórico de doações

📄 Licença
Este projeto é licenciado sob a Licença Creative Commons CC BY 4.0.

<p align="center"> Desenvolvido com 💙 por Global SI - FECAP </p>
