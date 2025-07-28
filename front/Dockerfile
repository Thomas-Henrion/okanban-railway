# Dockerfile pour servir le front avec Nginx
FROM nginx:alpine

# Copier le contenu du dossier dist dans le dossier par défaut de Nginx
COPY dist/ /usr/share/nginx/html/

# Exposer le port HTTP
EXPOSE 80

# Aucun CMD personnalisé, on utilise celui de l'image officielle
