Tämä on https://devopswithdocker.com/part1/ 1.17 tehtävä.

Konttiin on asennettu Node.js kehitysympäristö:
- Ubuntu versio 16.04
- Päivitykset 30.8.2020
- curl
- Nodesourcen setup 10.x versio
- Nodejs

Imagen Dockerfile käyttö esimerkki
    FROM janka2020/omakehitysymparisto:latest
    WORKDIR /mydir 
    COPY koodi .
    RUN npm install
    EXPOSE 3000
    CMD npm start