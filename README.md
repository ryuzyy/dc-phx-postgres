# Docker環境でPhoenix & PostgreSQLの環境構築する用のテンプレート
いつでも破壊できるように

## Setup
```bash

$ docker-compose build
$ docker-compose run --rm app mix phx.new {.envのPROJECT_NAME}

# /config/dev.exs 5~8行目を..envで指定した値に修正

$ docker-compose up -d
$ docker-compose run --rm app bash -c "cd {PROJECT_NAME} && mix ecto.create"

$ docker-compose restart app


```
