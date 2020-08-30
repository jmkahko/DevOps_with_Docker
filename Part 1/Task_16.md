Harjoituksen Heroku sivu https://dockerharjoitus.herokuapp.com/

Dockerharjoitus apin luonti Herokuuhun eka

Heroku kirjautuminen
    jannekahkonen@Janne-MBP Task_16 % heroku login

Imagen haku
    jannekahkonen@Janne-MBP Task_16 % docker pull devopsdockeruh/heroku-example

Nimen muutos
    jannekahkonen@Janne-MBP Task_16 % docker tag devopsdockeruh/heroku-example registry.heroku.com/dockerharjoitus/web

Herokuuhun laitto
    jannekahkonen@Janne-MBP Task_16 % docker push registry.heroku.com/dockerharjoitus/web
    The push refers to repository [registry.heroku.com/dockerharjoitus/web]

Heroku julkaisu
    jannekahkonen@Janne-MBP Task_16 % heroku container:release web --app dockerharjoitus
    Releasing images web to dockerharjoitus... done