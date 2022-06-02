# Déploiement flaskapp avec nginx en front loadbalancer sur AWS EC2
## Déploiement de l'infra as code avec un réplica de 3 conteneurs pour l'app et nginx en front pour faire du loadbalancing
docker-compose up --build -d --scale app=3

## Infra avec failover
docker -> nginx -> flaskapp1 || flaskapp2 || flaskapp3
