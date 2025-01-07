# Étape 1 : Utilisez une image officielle de Node.js
FROM node:18-alpine

# Étape 2 : Définir le répertoire de travail dans le conteneur
WORKDIR /app

# Étape 3 : Copier les fichiers nécessaires et installer les dépendances
COPY package.json package-lock.json ./
RUN npm install

# Étape 4 : Copier tout le reste des fichiers de l'application
COPY . .

# Étape 5 : Exposer le port que l'application utilise
EXPOSE 3000

# Étape 6 : Démarrer l'application
CMD ["node", "app.js"]
