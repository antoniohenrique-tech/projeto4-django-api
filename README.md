Projeto 4 — API REST de Filmes

Projeto desenvolvido para a disciplina de Desenvolvimento de Software, utilizando Python, Django e Django REST Framework.

Objetivo

Implementar uma API REST para gerenciamento de filmes e gêneros cinematográficos.

Tecnologias utilizadas

- Python
- Django
- Django REST Framework
- django-filter
- SQLite

Funcionalidades

- Listagem e consulta de filmes e gêneros
- Cadastro de novos registros
- Atualização e exclusão de registros
- Filtragem de filmes
- Autenticação por token
- Painel administrativo Django
- Importação de dados a partir de arquivo CSV

Como executar

1. Criar um ambiente virtual:

python -m venv venv

2. Ativar o ambiente virtual no Windows:

.\venv\Scripts\Activate.ps1

3. Instalar as dependências:

python -m pip install -r requirements.txt

4. Preparar o banco de dados:

python manage.py migrate

5. Importar os filmes:

python importarDados.py

6. Criar um superusuário:

python manage.py createsuperuser

7. Iniciar o servidor:

python manage.py runserver

Endpoints

Método| Endpoint| Descrição
GET| "/api/filmes/"| Listar filmes
POST| "/api/filmes/"| Cadastrar filme
GET| "/api/filmes/{id}/"| Consultar filme
PUT/PATCH| "/api/filmes/{id}/"| Atualizar filme
DELETE| "/api/filmes/{id}/"| Excluir filme
GET/POST| "/api/generos/"| Consultar e cadastrar gêneros
POST| "/api/token/"| Obter token de autenticação
—| "/admin/"| Painel administrativo

As operações de escrita exigem autenticação.

Testes realizados

Foram testadas as operações de consulta, cadastro, atualização e exclusão de filmes, além da obtenção de token de autenticação.

O projeto utiliza o servidor local do Django para demonstração acadêmica.