FROM node:14

WORKDIR /app

COPY . /app/

RUN ["npm", "install", "json-server"]

EXPOSE 9000

ARG PORT_API_JSON
ENV PORT_API_JSON=$PORT_API_JSON

CMD ["npx", "json-server", "--watch", "api.json", "--port", "9000"]