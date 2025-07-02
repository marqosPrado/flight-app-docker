# ✈️ Flight Application - Fullstack

Repositório responsável por orquestrar o **backend**, **frontend** e o **banco de dados** do sistema Flight Application, utilizando **Docker**.

A aplicação permite gerenciar e visualizar informações de voos, integrando uma API backend com um frontend moderno e um banco de dados PostgreSQL.

---

## 📦 Tecnologias Utilizadas

- **Backend:** Node.js, TypeScript, Express
- **Frontend:** Next.js, React, TypeScript
- **Banco de Dados:** PostgreSQL
- **Containerização:** Docker & Docker Compose

---
## ⚙️ Configuração Inicial

### 1️⃣ Pré-requisitos

- [Docker](https://www.docker.com/) instalado
- [Docker Compose](https://docs.docker.com/compose/) instalado

---

### 2️⃣ Configuração de Variáveis de Ambiente

Crie ou edite o arquivo `.env` na raiz do projeto com as seguintes variáveis:

```ini
# Ambiente
NODE_ENV=development

# Configuração do Banco de Dados
DATABASE_HOST=db
DATABASE_PORT=5432
POSTGRES_USER=postgres
POSTGRES_PASSWORD=admin
POSTGRES_DB=flight-database
````

🚀 Como Subir o Projeto

Na raiz do repositório, execute:
```ini
docker compose up --build
```

Este comando irá:

✅ Criar um container para o banco de dados PostgreSQL
✅ Construir e subir o backend em http://localhost:3001
✅ Construir e subir o frontend em http://localhost:3000
🛠️ Serviços Disponíveis
* Serviço	Descrição	Endereço
* Frontend	Interface do usuário	http://localhost:3000
* Backend	API REST	http://localhost:3001
* Banco de Dados	PostgreSQL	Host interno: db
