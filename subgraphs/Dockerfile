FROM node:22.18.0-slim

RUN apt-get update && apt-get install -y curl

WORKDIR /app

COPY package.json .
RUN npm install

COPY . .

ENTRYPOINT ["npm", "start"]
