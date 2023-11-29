FROM node:latest

WORKDIR /usr/src/app

COPY package*.json ./

RUN npm install -g json-server

COPY . .

EXPOSE 3000

CMD ["npx", "json-server", "--watch", "api.json"]