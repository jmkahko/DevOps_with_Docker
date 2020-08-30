Secret message: "Docker is easy"

% docker run -d --name loki devopsdockeruh/exec_bash_exercise       
    f8f9da8ac93212445e2b2be93b38a87496d85ba5399cfe2e20f3dfa23174559c

% docker start loki
    loki

% docker exec -it loki bash
    root@f8f9da8ac932:/usr/app# ls
    Dockerfile  README.md  index.js  logs.txt
    root@f8f9da8ac932:/usr/app# tail -f ./logs.txt
    Fri, 26 Jun 2020 11:06:33 GMT
    Fri, 26 Jun 2020 11:06:36 GMT
    Fri, 26 Jun 2020 11:06:39 GMT
    Fri, 26 Jun 2020 11:06:42 GMT
    Secret message is:
    "Docker is easy"
    Fri, 26 Jun 2020 11:06:48 GMT
    Fri, 26 Jun 2020 11:06:51 GMT
    Fri, 26 Jun 2020 11:06:54 GMT
    Fri, 26 Jun 2020 11:06:57 GMT
    Secret message is:
    "Docker is easy"
    ^XFri, 26 Jun 2020 11:07:03 GMT
    ^C
    root@f8f9da8ac932:/usr/app# exit
    exit

% 