# Étape 1 : Construire et préparer l'application Node.js
FROM node:18-alpine

WORKDIR /app

COPY package.json /app
RUN npm install

COPY . .

EXPOSE 3000

CMD ["node", "app.js"]
