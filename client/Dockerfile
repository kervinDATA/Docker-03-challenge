FROM node:lts-alpine

# Créer le dossier de l'application
RUN mkdir /app

# Définir le dossier de travail
WORKDIR /app

# Copier les fichiers package.json et package-lock.json
COPY package*.json ./

# Installer les dépendances
RUN npm i

# Copier le dossier public
COPY public ./public

# Commande pour démarrer l'application React
CMD ["npm", "start"]
