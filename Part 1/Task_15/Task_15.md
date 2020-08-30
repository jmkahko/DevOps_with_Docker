Harjoituksen sivu Docker hubissa https://hub.docker.com/repository/docker/janka2020/websivu

Build

    % docker build -t websivu .  

Projektin luonti ensin Docker Hub sivustolle nimellä websivu

Kirjautuminen

    % docker login                         
    Login with your Docker ID to push and pull images from Docker Hub. If you don't have a Docker ID, head over to https://hub.docker.com to create one.
    Username: janka2020
    Password: 
    Login Succeeded

Imagen nimeäminen

    % docker tag websivu janka2020/websivu 

Imagen siirtäminen Docker Hubiin

    % docker push janka2020/websivu        
    The push refers to repository [docker.io/janka2020/websivu]
    223b2ab3ac73: Pushed 
    b22c457f2225: Pushed 
    021348909f76: Pushed 
    d0f5924061f6: Pushed 
    21dabaeb6afb: Mounted from library/ubuntu 
    f182989ffc12: Mounted from library/ubuntu 
    0cf0b0655e84: Mounted from library/ubuntu 
    88b486ee59d1: Mounted from library/ubuntu 
    latest: digest: sha256:ee11f5c22063cd9ff38a1ae54c3a56dd2e2a8053de2e56c1bb9639577ab2acf6 size: 1983

Projektin käynnistys

    % docker run -it janka2020/websivu:latest
