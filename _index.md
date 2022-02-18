# Quiz zur Artenkenntnis Lebensraum Wald

## Ziel der Anwendung

Im Quizformat soll ermöglicht werden Kenntnisse zu Tieren und Pflanzen des Lebensraumes Wald spielerisch abzufragen.</br>
Der Spieler bekommt zu Beginn eine Vielzahl von Tieren und Pflanzen präsentiert, von denen sich der Spieler eine fixe Anzahl selbst auswählt. Von den verbleibdenden, nicht ausgewählten Beispielen werden dem Spieler zusätzlich eine weitere Auswahl vorgelegt.</br>
Zur Lösung der jeweiligen Quizaufgabe soll der Spieler die korrekte umsprangliche Bezeichnung der Pflanze oder des Tieres eintippen.</br>

## Ablauf

1. 20 Tiere werden als Kacheln angezeigt.
2. Der Spieler wählt 3 Tiere aus, die er auf jeden Fall benennen muss.
3. Aus den verbleibenden 17 Tierkacheln werden dem Spieler noch 7 zufällig ausgewählte Tiere zur Benennung vorgelegt
4. Anschließend das gleiche Vorgehen für 20 Pflanzen

## Anforderungen Aufgabensteller

- die Anwendung muss auf den schuleigenen iPads laufen und per Touch-Eingabe komplett bedienbar sein
- es soll ausdrücklich keine Nutzerverwaltung /-authentifizierung eingerichtet werden, um Zustimmungspflichten der Eltern zu vermeiden
- als "Kontrollmechanismus" zur Vermeidung von mehrfachem Reload der Anwendung bei Schlechtleistung soll eine Stopuhr beim Start des Quiz beginnen zu laufen, die eine Abschätzung eines Neuladens nach erstem Durchlauf ermöglichen soll
- in einer Art Endbildschirm muss erkennbar sein, wie viele Fragen der Spieler richtig hatte
- der Endbildschirm / das Spielergebnis muss durch die Lehrkraft kontrollierbar sein und sollte entsprechend gegen versehentliches "Wegklicken" gesichert sein (Mehrfachbestätigung erforderlich, gar kein Fortschritt ohne Seite neu laden möglich etc)


### technische Herausforderungen

- Die Antwort des Spielers erfolgt durch Eingabe über die OnScreen-Tastatur des iPads. Dies verkleinert einerseits den darstellbaren Bereich und erfordert andererseits eine "Ähnlichkeitsprüfung" der Antwort (kein 100% richtiges Benennen erforderlich)