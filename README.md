# 🚀 Quest

[![React](https://img.shields.io/badge/React-20232A?style=for-the-badge&logo=react&logoColor=61DAFB)](https://reactjs.org/)
[![Node.js](https://img.shields.io/badge/Node.js-339933?style=for-the-badge&logo=nodedotjs&logoColor=white)](https://nodejs.org/)
[![Express](https://img.shields.io/badge/Express.js-000000?style=for-the-badge&logo=express&logoColor=white)](https://expressjs.com/)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)](https://www.postgresql.org/)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/pt-BR/docs/Web/CSS)

O **Quest** é uma plataforma EdTech inovadora voltada para **avaliação formativa contínua** e **diagnóstico pedagógico em tempo real** em sala de aula. O objetivo principal do projeto é aumentar a participação ativa dos estudantes, combatendo a inibição e a exposição por meio de um ambiente seguro, interativo e dinâmico.

---

## 📌 Principais Funcionalidades (Features)

*   **🔄 Sincronização de Conteúdo:** Compartilhamento instantâneo de slides e conteúdos diretamente nas telas dos dispositivos dos alunos em tempo real.
*   **🕵️ Dúvidas Anônimas:** Canal direto e seguro para que os alunos possam enviar perguntas e feedbacks ao professor sem receio de exposição perante a turma.
*   **📊 Avaliação Formativa Dinâmica:** Verificações rápidas e interativas de aprendizagem ao final das explicações para validar a absorção do conteúdo.
*   **📈 Painel Analítico ("Foto Diagnóstica"):** Geração instantânea de relatórios e métricas de desempenho para o professor mapear os pontos de atenção da turma de forma imediata.
*   **🔑 Acesso Facilitado:** Sem necessidade de cadastros complexos para os alunos. O acesso à sala é feito de forma simples e rápida através de um código PIN nos navegadores.

---

## 🛠️ Tecnologias Utilizadas

*   **Frontend:** React, HTML5, CSS3, JavaScript.
*   **Backend:** Node.js com Express.
*   **Banco de Dados:** PostgreSQL.
*   **Acesso:** Web App responsivo.

---

## 🚀 Como Executar o Projeto Localmente

Siga as instruções abaixo para configurar e rodar o projeto em sua máquina local.

### 📋 Pré-requisitos

Antes de começar, você precisará ter instalado em sua máquina:
*   [Node.js](https://nodejs.org/) (versão LTS recomendada)
*   [PostgreSQL](https://www.postgresql.org/) (com um banco de dados criado para o projeto)
*   Gerenciador de pacotes `npm` (instalado automaticamente com o Node.js) ou `yarn`.

---

### 🔧 Instalação e Configuração

#### 1. Clonar o repositório
```bash
git clone https://github.com/vinium12/Quest.git
cd Quest
```

#### 2. Configurar o Banco de Dados (Backend)
Crie um arquivo `.env` na pasta do backend (ex: `server/.env` ou `backend/.env` dependendo da sua estrutura de diretórios) com as credenciais do seu PostgreSQL:
```env
DB_USER=seu_usuario
DB_HOST=localhost
DB_NAME=quest_db
DB_PASSWORD=sua_senha
DB_PORT=5432
PORT=5000
```

---

### 🖥️ Executando a Aplicação

A aplicação é dividida em duas partes principais: **Backend (servidor)** e **Frontend (cliente)**.

#### ▶️ Iniciando o Backend
Abra um terminal, acesse o diretório correspondente e instale as dependências:
```bash
cd backend
npm install
npm start
```
*O servidor Express iniciará na porta configurada (ex: `http://localhost:5000`).*

#### ▶️ Iniciando o Frontend
Em um novo terminal, acesse a pasta do frontend, instale as dependências e inicie o app React:
```bash
cd frontend
npm install
npm start
```
*O React abrirá automaticamente em seu navegador padrão no endereço `http://localhost:3000`.*

---

## 👥 Equipe (Autores)

Este projeto foi desenvolvido para fins acadêmicos por:

*   **Vinicius Fernandes de Lima**
*   **Jônatas Frinhani de Souza Palmeira**
*   **Gustavo**
