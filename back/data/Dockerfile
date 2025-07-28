# Dockerfile pour initialiser une base PostgreSQL avec des scripts SQL
FROM postgres:17.5-alpine

# Définir le répertoire de travail pour les scripts
WORKDIR /docker-entrypoint-initdb.d

# Copier les scripts d'initialisation
COPY create_tables.sql seed_database.sql ./

# Les scripts seront automatiquement exécutés à l'initialisation du conteneur
# Aucun CMD personnalisé nécessaire, on garde celui de l'image officielle
