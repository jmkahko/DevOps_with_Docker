jannekahkonen@Janne-MBP DevOps_with_Docker % docker run -d --rm -it --name webbisivu ubuntu:16.04 sh -c 'echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;'

jannekahkonen@Janne-MBP DevOps_with_Docker % docker start webbisivu
    webbisivu

jannekahkonen@Janne-MBP DevOps_with_Docker % docker exec -it webbisivu bash
    root@fd8cf09e9040:/# apt-get install curl wget
    Reading package lists... Done
    Building dependency tree       
    Reading state information... Done
    E: Unable to locate package curl
    E: Unable to locate package wget

    root@fd8cf09e9040:/# apt-get update

    root@fd8cf09e9040:/# apt-get install curl wget

    root@fd8cf09e9040:/# ps aux
    USER       PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
    root         1  0.0  0.0   4504   696 pts/0    Ss+  12:12   0:00 sh -c echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;
    root         6  0.0  0.1  18236  3296 pts/1    Ss   12:12   0:00 bash
    root      2668  0.0  0.1  34424  2776 pts/1    R+   12:13   0:00 ps aux

    root@fd8cf09e9040:/# sh -c echo "InputWebsite:"; read website; echo "Searching.."; sleep 1; curl http://$website;

    helsinki.fi
    Searching..
    <!DOCTYPE HTML PUBLIC "-//IETF//DTD HTML 2.0//EN">
    <html><head>
    <title>301 Moved Permanently</title>
    </head><body>
    <h1>Moved Permanently</h1>
    <p>The document has moved <a href="http://www.helsinki.fi/">here</a>.</p>
    </body></html>

    root@fd8cf09e9040:/# exit
    exit

jannekahkonen@Janne-MBP DevOps_with_Docker % docker kill webbisivu
    webbisivu

jannekahkonen@Janne-MBP DevOps_with_Docker % 