# Joomla-Speeltuin

https://www.joomla.org/


## 2 opties

### Testsite bij Joomla zelf
Hier moet je een telefoonnummer invullen, verder moet je deze elke maand verlengen.
launch.joomla.org

### Complete webserver met Joomla in Docker

De simpelste manier om lokaal een Joomla-omgeving te draaien is in een Docker container. (als je al weet hoe dit werkt dan kan je gelijk naar de link bij 2. gaan.)

1. Installeer [Docker Desktop](https://www.docker.com/products/docker-desktop/). Hiermee krijg je Docker, Docker-compose (maakt het mogelijk om meerdere containers samen te draaien en beheren, dan hoef je bijvoorbeeld niet zelf los containers te maken voor webserver, database, etc.) en Docker Desktop (een programma waarmee je alle containers kan beheren).
2. Download het voorbeeldconfiguratiebestand vanaf de [Docker Hub](https://hub.docker.com/_/joomla) (scroll door naar: "Example docker-compose.yml for joomla"). Vul hier eventueel een zelf gekozen wachtwoord voor de database in (waar nu "example" staat), aangezien alles toch alleen maar lokaal draait is dit niet strikt noodzakelijk.
3. Open een terminal en ga naar de directory waar je deze configuratie hebt opgeslagen.
4. Gebruik het commando "docker-compose -f stack.yml up" (waar je stack.yml vervangt door de naam van het configuratiebestand). Als het goed is worden nu de benodigde bestanden gedownload en geconfigureerd. Vervolgens starten alle containers.
5. Als het goed is komt er ook informatie in de terminal. In principe is de website (als het installatieproces klaar is) toegangkelijk op http://localhost:8080.
6. Doorloop de configuratie van Joomla. (het kan zijn dat hier de database-credentials uit het configuratiebestand nodig zijn)
7. Aangezien alles nu geïnstalleerd is kan je de volgende keer de containers starten door gewoon Docker Desktop te openen.
