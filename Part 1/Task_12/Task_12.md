Backend komennot
    Build
        % docker build -t backend .  
    
    Käynnistys
        % docker run -v "$(pwd)/logs.txt:/mydir/logs.txt" -p 3005:8000 backend

Frontend komennot
    Build
        % docker build -t frontend .  
    
    Käynnistys
        % docker run  -p 3006:5000 frontend