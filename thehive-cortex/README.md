# SOC Incident Response Layer — TheHive + Cortex

## Prérequis
- Docker
- Docker Compose
- 8 GB RAM minimum

## Déploiement

### 1. Cloner le projet
git clone https://github.com/fatimaezzahra123-wq/soc-orchestration
cd soc-orchestration/thehive-cortex

### 2. Lancer les services
docker compose up -d

## Accès Web

### TheHive
http://localhost:9000

### Cortex
http://localhost:9001

## Images Docker Hub utilisées
- fatimaezzahraennassiri/soc-thehive:latest
- fatimaezzahraennassiri/soc-cortex:latest
- fatimaezzahraennassiri/soc-cassandra:latest
- fatimaezzahraennassiri/soc-elasticsearch:latest

## Backups
Les sauvegardes sont dans :
thehive-cortex/backups/

## Comment ça marche
Les images Docker Hub contiennent déjà la configuration.
docker compose up -d télécharge automatiquement les images nécessaires.
