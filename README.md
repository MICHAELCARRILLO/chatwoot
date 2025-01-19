# chatwoot git

git clone https://github.com/jmlcas/chatwoot

#Ejecutar primero este comando

docker compose run --rm rails bundle exec rails db:chatwoot_prepare

#Una vez ha terminado la operación 

docker compose up -d

Ver en "localhost:3000"
