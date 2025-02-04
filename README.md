# ToDo List - Backend

Este é o backend do projeto **ToDo List**, desenvolvido com **Django** e **Django REST Framework (DRF)**. O backend é responsável por gerenciar as operações CRUD (Create, Read, Update, Delete) para as tarefas.

## Tecnologias Utilizadas

- **Django**: Framework web para Python.
- **Django REST Framework (DRF)**: Extensão do Django para construir APIs RESTful.
- **Python 3.x**: Linguagem de programação principal.
- **SQLite** (por padrão): Banco de dados relacional para armazenar os dados.

## Pré-requisitos

Antes de rodar o projeto, você precisará ter o seguinte instalado:

- **Python 3.x**: Para rodar o backend.
  - [Baixe e instale o Python aqui](https://www.python.org/downloads/)

- **pip**: Gerenciador de pacotes do Python (geralmente já vem com a instalação do Python).

## Instalação

1. Clone o repositório do projeto:
    ```bash
    git clone https://github.com/Rafael-Guerreiro/TODOlist_Backend
    ```

2. Navegue até a pasta do projeto:
    ```bash
    cd todolist-backend
    ```

3. Crie e ative um ambiente virtual:
    ```bash
    python -m venv venv
    source venv/bin/activate  # Para Linux/macOS
    venv\Scripts\activate     # Para Windows
    ```

4. Instale as dependências do projeto:
    ```bash
    pip install -r requirements.txt
    ```

## Como Executar

1. Aplique as migrações para configurar o banco de dados:
    ```bash
    python manage.py migrate
    ```

2. Crie um superusuário para acessar a interface de administração (opcional):
    ```bash
    python manage.py createsuperuser
    ```

3. Inicie o servidor de desenvolvimento:
    ```bash
    python manage.py runserver
    ```

4. Acesse o backend no seguinte endereço:
    ```
    http://localhost:8000
    ```

## Endpoints da API

- **GET /api/todos/**: Retorna todas as tarefas.
- **POST /api/todos/**: Cria uma nova tarefa.
- **PUT /api/todos/{id}/**: Atualiza uma tarefa existente.
- **DELETE /api/todos/{id}/**: Deleta uma tarefa.
