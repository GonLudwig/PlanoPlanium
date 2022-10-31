## TESTE TÉCNICO - PLANIUM


### Subindo o projeto

Voce deve adicionar ao seu hosts `/etc/hosts`

```
127.0.0.1       backend.com.br
127.0.0.1       frontend.com.br
```

Construa o projeto com os sequintes comandos.

Crie as variaveis de ambiente.

```sh
cp .env.example .env
```
```sh
cp ./app/.env.example ./app/.env
```

```sh
docker-compose up
```
Instalacao do composer.
```sh
docker-compose run --rm composer install
```
Criacao do banco de dados.
```sh
docker-compose run --rm artisan migrate --seed
```
### Arquivos

Os arquivos solicitados estao todo dentro da pasta `/app/storage/app/jsons`