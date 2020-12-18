FROM ubuntu:20.04
WORKDIR /dist

COPY package.json package-lock.json ./

RUN apt-get update && apt-get install -y curl
RUN curl -sL https://deb.nodesource.com/setup_10.x | bash

RUN apt-get update && apt-get install -y nodejs

COPY . .
RUN npm install

EXPOSE 5000

CMD npm start