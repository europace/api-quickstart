# Postman Calls für die EUROPACE APIs

Probeaufrufe der APIs sind sehr hilfreich, um schnell einzusteigen. Dafür empfehlen wir [Postman](https://www.getpostman.com/), was auf Windows, Mac OS und Linux funktioniert.

Eine Übersicht aller APIs ist hier zu finden: https://developer.europace.de/

📣Voraussetzung: sie benötigen von EUROPACE eine PartnerID und einen API Key. Diese können sie von ihrem EUROPACE Ansprechpartner bekommen.


## Schritte um Postman einzurichten

1. Postman installieren. Es ist *keine* Anmeldung erforderlich.
1. Oben links auf _Import_ Button klicken, dann auf _Import from Link_

4. Folgenden Link in die Textbox pasten: `https://raw.githubusercontent.com/europace/api-sandbox/master/EUROPACE%20API%20Calls.postman_collection.json`
![](screen1.png)

5.
1. Ein neues "Environment" anlegen, in dem Dein API Key und Parnter ID als Variable gespeichert wird. Dafür das Icon oben rechts klicken:
![](screen3.png)
1. Gebe deinem Environment einen Namen und legen darin die 2 Variablen folgendermassen an:
![](screen4.png)
1. Nach dem anlegen des Environments stelle sicher, dass es auch aktiv ist:
![](screen5.png)
1. . Der ersten Call in der Collection (`Login -> JWT erzeugen  mit PartnerId und API-Key`) anklicken
1. Bei klick auf _send_ müsste jetzt ein `access_token` zurück kommen.
1. Dieses ist (k)ein Testeintrag - hier gibt es nichts zu sehen.
