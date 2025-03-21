# 📚 Desafio: API de Cadastro de Livros

## 📝 Sobre o Desafio

- O desafio consiste em desenvolver uma API utilizando Flask para cadastrar e listar livros. Durante o projeto aplicou conceitos de banco de dados e construção de APIs.

## 🎯 Funcionalidades da API

- 📌 Cadastrar um livro no banco de dados via POST na rota /doar.

- 📌 Listar todos os livros cadastrados via GET na rota /livros.

- 📌 Exibir uma página inicial via GET na rota (/) com uma mensagem personalizada.

## 🛠️ Tecnologias Utilizadas

- Flask 🚀 (Micro Framework para desenvolvimento da API)

- SQLite 🗄️ (Banco de dados para armazenar os livros)

- Python 🐍 (Linguagem principal do projeto)

## ⚙️ Requisitos Técnicos

1️⃣ Utilizar Flask para criar as rotas da API. <br>
2️⃣ Utilizar SQLite como banco de dados. <br>
3️⃣ Criar uma tabela chamada LIVROS com os seguintes campos: <br>

- id (Chave primária, autoincrementada)

- titulo (Texto, obrigatório)

- categoria (Texto, obrigatório)

- autor (Texto, obrigatório)

- image_url (Texto, obrigatório)

4️⃣ Ao cadastrar um novo livro, a API deve retornar uma resposta JSON com código 201 confirmando o cadastro. <br>
5️⃣ A rota GET /livros deve retornar todos os livros cadastrados organizados em JSON. <br> 
6️⃣ A rota inicial / deve exibir uma mensagem personalizada. <br>
