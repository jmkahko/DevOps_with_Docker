Build
    % docker build -t task11 .  

Käynnistys
    % docker run -v "$(pwd)/logs.txt:/mydir/logs.txt" -p 8000:8000 task11

Selaimessa
    Port configured correctly, generated message in logs.txt