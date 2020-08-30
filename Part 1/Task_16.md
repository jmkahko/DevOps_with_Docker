Harjoituksen Heroku sivu https://dockerharjoitus.herokuapp.com/

Dockerharjoitus apin luonti Herokuuhun eka

Heroku kirjautuminen

    % heroku login

Imagen haku

    % docker pull devopsdockeruh/heroku-example

Nimen muutos

    % docker tag devopsdockeruh/heroku-example registry.heroku.com/dockerharjoitus/web

Herokuuhun laitto

    % docker push registry.heroku.com/dockerharjoitus/web
    The push refers to repository [registry.heroku.com/dockerharjoitus/web]

Heroku julkaisu

    % heroku container:release web --app dockerharjoitus
    Releasing images web to dockerharjoitus... done
