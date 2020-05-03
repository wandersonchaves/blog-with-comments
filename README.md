# BLOG WITH COMMENTS

[Build your first Rails app - blog with comments (tutorial)](https://www.youtube.com/watch?v=wbZ6yrVxScM)

### Installation

- Criar nova aplicação rails

```sh
rails new blog-with-comments --database=postgresql --skip-test --skip-action-cable --skip-turbo-links
```

- Copiar arquivos de configuração
  - docker-compose
  - database.yml
  - Procfile.dev
  - .env

```sh
cp ../rails-react-learning/docker-compose.yml .

cp ../rails-react-learning/config/database.yml config/database.yml

cp ../rails-react-learning/Procfile.dev .

cp ../rails-react-learning/.env .
```

configure o `database.yml` para o nome do banco correto

### Boot

- Inicie o docker-compose

`docker-compose up --build`

- Instale e configure o DB Rails

```sh
rails db:create

rails db:migrate
```

- Inicialize o server com _overmind_

```sh
overmind start
```
