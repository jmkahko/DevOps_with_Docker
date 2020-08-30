% docker run -d nginx

    Unable to find image 'nginx:latest' locally
    latest: Pulling from library/nginx
    8559a31e96f4: Pull complete 
    8d69e59170f7: Pull complete 
    3f9f1ec1d262: Pull complete 
    d1f5ff4f210d: Pull complete 
    1e22bfa8652e: Pull complete 
    Digest: sha256:21f32f6c08406306d822a0e6e8b7dc81f53f336570e852e25fbe1e3e3d0d0133
    Status: Downloaded newer image for nginx:latest
    a102dc9cd55741608f7bc14c71ed1fdd95bfb328e5303cb6c572e1296b809c3f

% docker run -d nginx

    b8dcd08663eb2541ce102f5024f1e836cc40d3f3c32f1497bc7981a0f991c858

% docker run -d nginx

    6c48aad9d388b477798cc02fa7c5db41db4bfda68369e2bfc7c70cb5cd75898f

% docker container ls -a

    CONTAINER ID        IMAGE               COMMAND                  CREATED             STATUS              PORTS               NAMES
    6c48aad9d388        nginx               "/docker-entrypoint.…"   38 seconds ago      Up 37 seconds       80/tcp              interesting_engelbart
    b8dcd08663eb        nginx               "/docker-entrypoint.…"   40 seconds ago      Up 39 seconds       80/tcp              quizzical_matsumoto
    a102dc9cd557        nginx               "/docker-entrypoint.…"   45 seconds ago      Up 44 seconds       80/tcp              sleepy_nash

% docker stop 6c48aad9d388

    6c48aad9d388

% docker stop b8dcd08663eb

    b8dcd08663eb

% docker container ls -a  

    CONTAINER ID        IMAGE               COMMAND                  CREATED              STATUS                      PORTS               NAMES
    6c48aad9d388        nginx               "/docker-entrypoint.…"   About a minute ago   Exited (0) 12 seconds ago                       interesting_engelbart
    b8dcd08663eb        nginx               "/docker-entrypoint.…"   About a minute ago   Exited (0) 3 seconds ago                        quizzical_matsumoto
    a102dc9cd557        nginx               "/docker-entrypoint.…"   About a minute ago   Up About a minute           80/tcp              sleepy_nash

% docker ps -a

    CONTAINER ID        IMAGE               COMMAND                  CREATED              STATUS                      PORTS               NAMES
    6c48aad9d388        nginx               "/docker-entrypoint.…"   About a minute ago   Exited (0) 19 seconds ago                       interesting_engelbart
    b8dcd08663eb        nginx               "/docker-entrypoint.…"   About a minute ago   Exited (0) 9 seconds ago                        quizzical_matsumoto
    a102dc9cd557        nginx               "/docker-entrypoint.…"   About a minute ago   Up About a minute           80/tcp              sleepy_nash

% 
