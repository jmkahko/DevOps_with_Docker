Otettu pohjaksi tehtävän 2.8 docker-compose, backend ja frontend tiedot.
Korjattu, että tietokanta tallentaa paikalliseen database hakemistoon tehtävän 2.9 mukaan.
Aloituksessa tilanne:

- Sivulta http://localhost:3006/ toimii tehtävät 1.10, 1.12, 2.5 ja 2.6
- Sivulta http://localhost/ toimii tehtävä 2.8

Korjaus, että kaikki tehtävät toimii sivulta http://localhost/ suoraan.

- Muutettu frontend Dockerfile tiedostoon rivi ENV API_URL=http://localhost:3005 kommenttiin

Backendin oletus polku on /api, aikaisemmin frontend Dockerfilessä oli muuttuja ENV API_URL, jolloin oletusarvoa ei käytetty tiedon hakuun.
