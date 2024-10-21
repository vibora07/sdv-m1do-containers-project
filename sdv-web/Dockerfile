# Dockerfile pour le Front-End
FROM node:23.0.0 AS dev

# Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Copier les fichiers package.json et package-lock.json
COPY package.json package-lock.json ./

# Installer les dépendances
RUN npm install 


# Copier le reste du code de l'application
COPY . .

# Exposer le port utilisé par l'application (3000 pour Next.js)
EXPOSE 3000

# Lancer le serveur Next.js en mode développement
CMD ["npm", "run", "dev"]
