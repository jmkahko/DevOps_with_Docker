jannekahkonen@Janne-MBP Task_1.7 % docker build -t curler .
    Sending build context to Docker daemon  3.584kB
    Step 1/6 : FROM ubuntu:16.04
    ---> 330ae480cb85
    Step 2/6 : WORKDIR /mydir
    ---> Using cache
    ---> 64eb02902a28
    Step 3/6 : RUN apt-get update && apt-get install -y curl wget
    ---> Using cache
    ---> 8ff3ea762b54
    Step 4/6 : COPY curler.sh .
    ---> d438cd8e36da
    Step 5/6 : RUN chmod +x curler.sh
    ---> Running in 6dc461dee8e3
    Removing intermediate container 6dc461dee8e3
    ---> 9949719a7aa3
    Step 6/6 : CMD ["/mydir/curler.sh"]
    ---> Running in 782d07bfedb3
    Removing intermediate container 782d07bfedb3
    ---> 4f5b91da5078
    Successfully built 4f5b91da5078
    Successfully tagged curler:latest

jannekahkonen@Janne-MBP Task_1.7 % docker run -it curler   
    Input website:
    helsinki.fi
    Searching..
    <!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
    <html><head>
    <title>301 Moved Permanently</title>
    </head><body>
    <h1>Moved Permanently</h1>
    <p>The document has moved <a href="http://www.helsinki.fi/">here</a>.</p>
    </body></html>
    
jannekahkonen@Janne-MBP Task_1.7 % 