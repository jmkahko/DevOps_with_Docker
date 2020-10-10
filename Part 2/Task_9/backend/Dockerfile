FROM ubuntu:latest

WORKDIR /mydir 
RUN apt-get update && apt-get install -y curl 

COPY backend-example-docker-master .

RUN curl -sL https://deb.nodesource.com/setup_10.x | bash

RUN apt-get install -y node.js
RUN npm install

EXPOSE 8000

ENV FRONT_URL=http://localhost:3006

CMD npm start