FROM node:24.14.0-slim

RUN apt-get update && apt-get install -y curl

WORKDIR /app

COPY package.json .
RUN npm install

COPY . .

ENTRYPOINT ["npm", "start"]
