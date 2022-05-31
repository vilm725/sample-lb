# Lancer l'infra as code avec un réplica de 2 conteneurs pour l'app
docker-compose up --build -d --scale app=2

# Infra avec failover
Si le 1er conteneur lâche, le deuxième prendra le relais

docker -> nginx -> flaskapp1 || flaskapp2
