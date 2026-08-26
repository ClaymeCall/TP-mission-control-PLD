FROM node:20-alpine

WORKDIR /app

COPY package*.json .
COPY ../package*.json .
RUN npm ci

COPY . .
COPY .. .

EXPOSE 3000

CMD ["node", "SYSTEME_MISSION_NE_PAS_MODIFIER/app/server.js"]
