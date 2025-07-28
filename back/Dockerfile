# Dockerfile pour le serveur API (production)
FROM node:20-alpine

# Définir le répertoire de travail
WORKDIR /app

# Copier les fichiers package.json et package-lock.json
COPY package.json package-lock.json ./

# Installer les dépendances en production
RUN npm ci --only=production

# Copier le reste du code source
COPY . .

# Exposer le port (à adapter si besoin)
EXPOSE 80

# Commande de démarrage
CMD ["node", "index.js"]
