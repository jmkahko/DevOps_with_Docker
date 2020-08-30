% docker ps -as

    CONTAINER ID        IMAGE               COMMAND                  CREATED             STATUS                     PORTS               NAMES                   SIZE
    6c48aad9d388        nginx               "/docker-entrypoint.…"   3 minutes ago       Exited (0) 2 minutes ago                       interesting_engelbart   1.11kB (virtual 132MB)
    b8dcd08663eb        nginx               "/docker-entrypoint.…"   3 minutes ago       Exited (0) 2 minutes ago                       quizzical_matsumoto     1.11kB (virtual 132MB)
    a102dc9cd557        nginx               "/docker-entrypoint.…"   3 minutes ago       Up 3 minutes               80/tcp              sleepy_nash             1.12kB (virtual 132MB)

% docker images

    REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
    nginx               latest              2622e6cca7eb        5 days ago          132MB

% docker rm 6c48aad9d388 

    6c48aad9d388

% docker rm b8dcd08663eb

    b8dcd08663eb

% docker rm a102dc9cd557 

    Error response from daemon: You cannot remove a running container a102dc9cd55741608f7bc14c71ed1fdd95bfb328e5303cb6c572e1296b809c3f. Stop the container before attempting removal or force remove

% docker stop a102dc9cd557 

    a102dc9cd557

% docker rm a102dc9cd557   

    a102dc9cd557

% docker rmi nginx

    Untagged: nginx:latest
    Untagged: nginx@sha256:21f32f6c08406306d822a0e6e8b7dc81f53f336570e852e25fbe1e3e3d0d0133
    Deleted: sha256:2622e6cca7ebbb6e310743abce3fc47335393e79171b9d76ba9d4f446ce7b163
    Deleted: sha256:e86d1b8b130bec203609b4b1d7b851bd763fa16e513e5a3fa6102ebea23260e0
    Deleted: sha256:8f9f007533543813bb1aef80b791a16e5e16c7cbbbc456a3a483d0fa7a9effcc
    Deleted: sha256:e2c0065a77fee75795cdcf9f19a72f11769332423cd52ec9e19aacfb878aec8b
    Deleted: sha256:059442698ef65fe8545e4fe9657988a10329b9c3663b368ae7ee0007a9c43949
    Deleted: sha256:13cb14c2acd34e45446a50af25cb05095a17624678dbafbcc9e26086547c1d74

% docker ps -a

    CONTAINER ID        IMAGE               COMMAND             CREATED             STATUS              PORTS               NAMES

% docker images

    REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE

% 
