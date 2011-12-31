# Einleitung
Hier entsteht eine Sammlung für die Firefox-Erweiterung userChromeJS.

Fast alle Skripte wurden im deutschen Firefox-Forum vorgestellt bzw. dort angepasst.

Für GitHub werden die Skripte in Unterordnern mit entsprechenden README-Dateien abgelegt. Es handelt sich dabei um 
Textdateien im markdown-Format mit der Dateiendung `md`. Screenshots bis zum 30.09.2011 wurden im Firefox 6 erstellt. 
Die Ergebnisse der für neuere Firefox-Versionen aktualisierten Skripte sehen vielleicht ein wenig anders aus. Die Screenshots 
werden nur bei extremen Unterschieden aktualisiert. 

# Testumgebung
- Win XP SP 3/ Firefox 9 (ab 27.12.2011)
- Win XP SP 3/ Firefox 8 (ab 10.11.2011)
- Win XP SP 3/ Firefox 7 (ab 01.10.2011)
- Win XP SP 3/ Firefox 6 (bis 30.09.2011)

Sollte ein Skript nicht funktionieren, bitte im Quelltext nachschauen, was in der jeweiligen Firefoxversion angepasst 
werden muss bzw. in der Historie des Skriptes stöbern.

# Installation
Zur Aktivierung der Skripte im Firefox muss 

- die **Erweiterung userChromeJS** installiert und lauffähig sein
- eine **Datei namens userChrome.js** für den Import der Skripte sorgen (weiter unten dazu mehr)
- das jeweilige Skript in den Chrome-Ordner des Profils kopiert werden

Das Einbinden der `uc.js`- und `uc.xul`-Dateien geschieht mit der beigelegten userChrome.js. Diese Datei (bitte nicht mit 
der Erweiterung verwechseln) muss ebenfalls in den Chrome-Ordner des Profils eingefügt werden. Die Zeile

    userChrome.import("*", "UChrm");

darin sorgt für den Import aller userChrome-Skripte.

# Downloads
- die benötigte **Erweiterung** userChromeJS: http://userchromejs.mozdev.org/
- eine beispielhafte **Datei** userChrome.js: https://github.com/ardiman/userChrome.js/blob/master/userChrome.js

# Hinweis
Seit Firefox 8.0 gibt es eine Art Skriptcache. Dies führt dazu, dass Änderungen von Skripten (Konfiguration/Texte usw.) nach 
einem "normalen" Neustart nicht aktiv werden. Es gibt Skripte, die dieses Problem durch Löschen des Skriptcaches lösen können:

- https://github.com/ardiman/userChrome.js/tree/master/addrestartbutton
- https://github.com/ardiman/userChrome.js/tree/master/restartfirefox
- https://github.com/ardiman/userChrome.js/tree/master/restartfirefoxbutton

# Quellen
- http://www.camp-firefox.de/forum/viewtopic.php?f=16&t=90403
- https://github.com/ardiman/userChrome.js
