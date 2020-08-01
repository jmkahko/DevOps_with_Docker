FROM ubuntu:latest

WORKDIR /mydir 
RUN apt-get update && apt-get install -y curl 

COPY frontend-example-docker-master .

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash

RUN apt-get install -y node.js
RUN npm install

EXPOSE 5000

CMD npm start