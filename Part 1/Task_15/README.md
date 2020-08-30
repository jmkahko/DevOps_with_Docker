Tämä on https://devopswithdocker.com/part1/ 1.15 tehtävä.

Konttiin asennettu Ubuntun versio 16.04 ja kopioidaan curler.sh tiedosto.
Tiedosto sisältää lauseen:
    #!/bin/bash
    echo "Input website:"; read website; echo "Searching.."; sleep 1; curl http://$website;
Kun kontin käynnistää, pyydetään syöttämään internet sivun osoite, joka tulostaa kyseisen sivun html tiedostoa.

Kontin saa käyntiin esim. docker run -it janka2020/websivu:latest komennolla latauksen jälkeen.