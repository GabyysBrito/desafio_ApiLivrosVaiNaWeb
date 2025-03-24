# 📚 API de Doação de Livros

## 📝 Sobre o projeto
Essa é uma API simples feita com Flask e SQLite3 para fins de estudo da escola Vai Na Web, ela permite cadastar e listar dados

## 🛠️ Tecnologias Utilizadas

- Flask 🚀 (Micro Framework para desenvolvimento da API)

- SQLite3 🗄️ (Banco de dados para armazenar os livros)

- Python 🐍 (Linguagem principal do projeto)

## Como rodar o projeto

1. Faça o clone do repositório 

```bash 
    git clone <URL_DO_REPOSITORIO>
    cd nome-do-projeto
```

2. Crie um ambiente virtual (obrigatório):
```
    python -m venv venv
    source venv/Scripts/activate
```

3. Instale as dependências 
```
    pip install -r requirements.txt
```

4. Inicie o servidor:
```bash
    python app.py
```

> A api está disponível em http: http://127.0.0.1:5000/

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

## 🎯 Funcionalidades da API

- 📌 Cadastrar um livro no banco de dados via POST na rota /doar.

- 📌 Listar todos os livros cadastrados via GET na rota /livros.

- 📌 Exibir uma página inicial via GET na rota (/) com uma mensagem personalizada.

# Endpoints

### 📌 POST /doar 
Endpoint para cadastrar um novo livro

**Formato de envio dos dados**
```json
    {
        "titulo":"O poder do hábito",
        "categoria":"Auto-ajuda",
        "autor":"Charles Duhigg"
        "image_url": "https://...."
    }
```

**Resposta 201 (Created)** 
```json
    "mensagem": "Livro cadastrado com sucesso"
```

## 📌 GET /livros
Retorna todos os livros cadastrados em nossa API.

**Resposta (200)**

```json
    {
        "id":"1"
        "titulo":"O poder do hábito",
        "categoria": "Auto-ajuda",
        "autor": "Charles Duhigg",
        "image_url": "https://...."
    }
```

## 📌 Página inicial

```python
    @app.route("/")

    def inicial():
        return "<h1> Sistemas de Livros da Vai na Web </h1>"
```