# SOC Orchestration Layer — Shuffle SOAR

## Prérequis
- Docker + Docker Compose installés
- 8GB RAM minimum

## Déploiement

### 1. Cloner le repo
git clone https://github.com/fatimaezzahra123-wq/soc-orchestration
cd soc-orchestration/shuffle

### 2. Configurer l'environnement
cp .env.example .env
mkdir -p shuffle-apps shuffle-files shuffle-database

### 3. Lancer les conteneurs
docker compose up -d

### 4. Accéder à Shuffle
http://localhost:3001

### 5. Importer les workflows
- Aller dans Workflows
- Importer le fichier workflows-export/all-workflows.json

## Images Docker Hub
- fatimaezzahraennassiri/soc-shuffle-frontend:latest
- fatimaezzahraennassiri/soc-shuffle-backend:latest
- fatimaezzahraennassiri/soc-shuffle-orborus:latest
- fatimaezzahraennassiri/soc-tenzir:latest
- fatimaezzahraennassiri/soc-shuffle-opensearch:latest
