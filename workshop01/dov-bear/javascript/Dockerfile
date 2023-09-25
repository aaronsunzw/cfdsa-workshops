FROM node:latest

LABEL name=workshop01

WORKDIR /app

COPY main.js .
COPY package-lock.json .
COPY package.json .
COPY public public
COPY views views

RUN npm ci

ENV PORT=3000

EXPOSE ${PORT}

ENTRYPOINT node main.js
