Backend komennot
    Build
        jannekahkonen@Janne-MBP Task_11 % docker build -t backend .  
    
    Käynnistys
        jannekahkonen@Janne-MBP backend % docker run -v "$(pwd)/logs.txt:/mydir/logs.txt" -p 3005:8000 backend

Frontend komennot
    Build
        jannekahkonen@Janne-MBP Task_11 % docker build -t frontend .  
    
    Käynnistys
        jannekahkonen@Janne-MBP frontend % docker run  -p 3006:5000 frontend