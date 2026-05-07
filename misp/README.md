# SOC Threat Intelligence Layer — MISP

## Prérequis
- Docker
- Docker Compose
## Déploiement

### 1. Cloner le projet
git clone https://github.com/fatimaezzahra123-wq/soc-orchestration
cd soc-orchestration/misp

### 2. Configurer l'environnement
cp .env.example .env

### 3. Lancer les services
docker compose up -d

## Accès Web

### MISP
http://localhost:8080

## Images Docker Hub utilisées
- fatimaezzahraennassiri/soc-misp-core:latest
- fatimaezzahraennassiri/soc-misp-db:latest
- fatimaezzahraennassiri/soc-misp-modules:latest
- fatimaezzahraennassiri/soc-misp-redis:latest
- fatimaezzahraennassiri/soc-misp-mail:latest

## Backups
Les sauvegardes sont dans :
misp/backups/

## Comment ça marche
Les images Docker Hub contiennent déjà la configuration.
docker compose up -d télécharge automatiquement les images nécessaires.
