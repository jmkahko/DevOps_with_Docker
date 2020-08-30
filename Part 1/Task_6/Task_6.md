% docker build -t docker-clock .
    Sending build context to Docker daemon  2.048kB
    Step 1/4 : FROM devopsdockeruh/overwrite_cmd_exercise
    ---> 3d2b622b1849
    Step 2/4 : WORKDIR /mydir
    ---> Using cache
    ---> 0c9e47ced82b
    Step 3/4 : RUN apt-get update
    ---> Using cache
    ---> bb19138d5c88
    Step 4/4 : CMD [ "-c" ]
    ---> Running in 6360aa5f6489
    Removing intermediate container 6360aa5f6489
    ---> 01d9be08f881
    Successfully built 01d9be08f881
    Successfully tagged docker-clock:latest

% docker run docker-clock   
    1
    2
    3
    4