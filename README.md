# Postman Calls für die EUROPACE APIs

Probeaufrufe (Calls) der APIs sind sehr hilfreich, um schnell einzusteigen. Dafür empfehlen wir [Postman](https://www.getpostman.com/), was auf Windows, Mac OS und Linux funktioniert.

## Voraussetzung um diese Calls auszuführen:

1. Du benötigst eine API Zugriff. Das beinhaltet entweder:
   * OAuth Client Credentials. Wo diese herkommen ist [hier beschrieben](https://europace2.zendesk.com/hc/de/articles/360012514780).
   * eine PartnerID und einen API Key (für eine "Legacy Autorisierung").
2. Du benötigst mindestens einen Vorgang oder einen Antrag, um die Daten auszulesen.

## Schritte um Postman einzurichten

1. Postman [runterladen](https://www.getpostman.com/) und installieren. Es ist *keine* Anmeldung erforderlich.
2. Oben links auf _Import_ Button klicken, dann auf _Import from Link_

3. Folgenden Link in die Textbox pasten: `https://raw.githubusercontent.com/europace/api-sandbox/master/EUROPACE%20API%20Calls.postman_collection.json`
![](https://raw.githubusercontent.com/europace/api-schnellstart/master/screen1.png)

4. Ein neue Umgebung (_Environment_) anlegen in dem mehrere notwendige Variablen eingetragen werden müssen. Dafür das Icon oben rechts klicken:
![](https://raw.githubusercontent.com/europace/api-schnellstart/master/screen3.png)
5. Gib deiner _Environment_ einen Namen und lege darin die folgende Variablen an:

| Variablen Name | Woher bekomme ich das? |
| -------------- | ---------------------- |
| API_KEY        | Siehe oben unter "Voraussetzung" |
| PARTNER_ID     | Siehe oben unter "Voraussetzung" |
| CLIENT_ID      | Siehe oben unter "Voraussetzung" |
| CLIENT_SECRET  | Siehe oben unter "Voraussetzung" |
| SCOPES         | Optional. Siehe [hier](https://github.com/europace/authorization-api/blob/master/docs/scopes.md) |

![](https://raw.githubusercontent.com/europace/api-schnellstart/master/screen4.png)
5. Stelle nach dem Anlegen der _Environment_ sicher, dass diese auch aktiv ist:
![](https://raw.githubusercontent.com/europace/api-schnellstart/master/screen5.png)
6. Den Aufruf in der neuen Collection in der Linken spalte (`Get Access-Token`) anklicken
7. Beim Klick auf _send_ müsste jetzt ein `access_token` zurück kommen.
