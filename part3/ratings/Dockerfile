FROM node:12.18.1-slim

WORKDIR /opt/microservices/

COPY package.json .

COPY ratings.js .

ARG service_version

ENV SERVICE_VERSION ${service_version:-v1}

RUN npm install

EXPOSE 9080

CMD ["node", "ratings.js", "9080"]

