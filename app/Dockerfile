FROM node:latest

EXPOSE 8080

WORKDIR /app

RUN apt-get update -qq

RUN apt-get install vim -y

COPY package.json yarn.lock ./
RUN yarn install
CMD yarn run start:dev
