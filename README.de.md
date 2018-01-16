# ip_login

Benutzer einloggen auf Grundlage Ihrer IP-Adresse

## Haftungsausschluss

Alle IP-Adressen in diesem Dokument wurden zufällig generiert.
Das UliCMS Projekt steht mit keiner dieser IP-Adressen in Verbindung.

Wörter in eckigen Klammern sind als Platzhalter gedacht

**Beispiel:** 

```
[IP-Adresse]
```

## Was ist ip_login?

ip_login ist ein UliCMS Modul um Benutzer auf Grundlage ihrer IP-Adresse automatisch einzuloggen.
Wenn ein Client von der IP-Adresse [IP-Adresse] auf das UliCMS Backend zugreift, wird der Benutzer [Benutzername] automatisch eingeloggt. In diesem Fall wird der Logout-Button entfernt, da ein Logout nicht möglich ist. Wenn sich seit der Authentifizierung auf diese Weise die IP-Adresse des Clients ändert, wird dieser automatisch ausgeloggt.

ip_login kann gleichzeitig mit anderen Authentifizierungsmodulen und -Methoden betrieben werden.

## Voraussetzungen

* UliCMS 2018.2 oder eine neuere Version von uliCMS 2018.x

## Konfiguration

Um die IP-zu-User Mappings zu konfigurieren, benötigt Ihre Benutzergruppe das Recht "ip_login".

1. Klicken Sie auf **Pakete** > **ip_login** > **Einstellungen**
2. Es gibt eine Textbox für die Eingabe von Mappings.

Ein Eintrag je Zeile.

Die Einträge müssen in der folgenden Form erfolgen

```
[IP-Adresse]=>[Benutzername]
```

Hier sind einige Beispiel-Zuweisungen

```
131.213.138.20=>maxmuster
209.143.210.186=>sabinemuster
60.226.125.233=>johndoe
``` 
