# M300 - LB2 Safari
Im Modul 300 haben wir uns auf Docker, Kubernetes und Vagrant konzentriert. 
## Auftrag LB2
Einen Dienst mit Docker zur Verfügung stellen.
## Auswertung
* Umgebung (funktionsfähig auf Notebook (Note 4.0)
* Bestehende Docker Container kombinieren (Note 4.5)
* Eigene Container erstellen (Note 5.0 – 5.5)
* Projekt auf github Ablegen und mit Markdown dokumentieren (Markdown) (Note 5.5 – 6.0)

## Beschreibung des Services
Mein Service besteht aus drei verknüpften Containern. Einem Wordpress, MySQL und PHPMyAdmin Server. Der Service soll die Erstellung einer Webumgebung vereinfachen und automatisieren. Die Services wurden mit einem Docker-Compose file erstellt und kann mithilfe von einem vagrantfile ausgeführt werden. 

## Benutzerhilfe plus Netzwerkplan

**Netzwerkplan:**

![Netzwerkplan](https://github.com/Rooholla1234/Rep2/blob/master/Netzwerkplan.png)


**Aufschaltung**

Um die Dienste erfolgreich benutzen zu können, sollte man im Vagrant File die IP der VM nach Wunsch ändern. Danach sollte man im Docker-Compose File den Benutzernamen, Passwort und Root Passwort für die Datenbank abändern. Die Änderung im Wordpress Service nachgetragen werden muss.

DB Standardname und Passwort sind: <br>
  - Name = dbuser <br>
  - Passwort = Test1234

Um es zu bedienen einfach mithilfe einer Konsole wie Git Bash das File anschauen. Im Repository Verzeichnis, den Befehl vagrant up auszuführen.
Die Installation geht eine Weile, doch nachher können die Dienste wie folgt erreicht werden:

Wordpress Seite anzeigen (Port 8000): http://IP:8000 <br>
Wordpress Admin Account (Port 8000 wp-admin(WordPress Admin)): http://IP:8000/wp-admin <br>
PHPMyAdmin Interface (Port 8080): http://IP:8080 (Username und Passwort welche man vorhin geändert hat. <br>
## Test
Getestet können die Dienste wie folgt: <br>
Auf die Webseite zugreiffen<br>
Datenbank User erstellen, löschen. 
Container neu starten, DB kontrollieren, ob die Dateien immer noch bestehen. 
## Troubleshooting

Mögliche Probleme können entstehen: <br>
  - Netzwerk (Kontrollieren sie wie die Netzwerkkonfiguration ist. <br>