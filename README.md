# chatwoot git

git clone https://github.com/jmlcas/chatwoot

#Ejecutar primero este comando

docker compose run --rm rails bundle exec rails db:chatwoot_prepare

#Una vez ha terminado la operación 

docker compose up -d

Ver en "localhost:3000"



## Errores comunes

--> vector de postgress

- cd chatwoot
- docker ps
- docker exec -it chatwoot-postgres-1 bash
- apt-get update
- apt-get install wget
- wget --quiet -O - https://packages.postgresql.org/keys/ACCC4CF8.asc | tee /etc/apt/trusted.gpg.d/postgresql.asc
- echo "deb http://apt.postgresql.org/pub/repos/apt/ bookworm-pgdg main" > /etc/apt/sources.list.d/pgdg.list
- apt-get update
- apt-get install postgresql-15-pgvector
- psql -U postgres
- CREATE EXTENSION IF NOT EXISTS vector;
- \q
- exit
- docker compose run --rm rails bundle exec rails db:chatwoot_prepare
- docker compose up -d
