FROM node:lts-alpine

RUN mkdir /app
WORKDIR /app

COPY package*.json ./
RUN npm i

COPY tsconfig.json tsconfig.json
COPY public public
COPY codegen.yml codegen.yml
COPY src src
COPY .env .env

CMD npm start