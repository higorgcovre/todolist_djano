# Criar o arquivo README.md
New-Item -Path README.md -ItemType File

# Adicionar conteúdo ao README.md
@"
# To-Do List

Este é um projeto simples de lista de tarefas criado com Django e PostgreSQL.

## Requisitos

- Python
- Django
- PostgreSQL

## Configuração

1. Clone o repositório:
    ```bash
    git clone <URL_DO_REPOSITORIO>
    ```

2. Instale as dependências:
    ```bash
    pip install -r requirements.txt
    ```

3. Configure o banco de dados no `settings.py`.

4. Crie e aplique as migrações:
    ```bash
    python manage.py makemigrations
    python manage.py migrate
    ```

5. Execute o servidor:
    ```bash
    python manage.py runserver
    ```

## Uso

Acesse `http://127.0.0.1:8000/` no seu navegador para ver a lista de tarefas.

## Contribuição

Sinta-se à vontade para abrir issues e pull requests.
"@ | Set-Content -Path README.md
