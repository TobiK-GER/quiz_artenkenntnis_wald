# Quiz zur Artenkenntnis Lebensraum Wald

## Ziel der Anwendung

Im Quizformat soll ermöglicht werden Kenntnisse zu Tieren und Pflanzen des Lebensraumes Wald spielerisch abzufragen.</br>
Der Spieler bekommt zu Beginn eine Vielzahl von Tieren und Pflanzen präsentiert, von denen sich der Spieler eine fixe Anzahl selbst auswählt. Von den verbleibdenden, nicht ausgewählten Beispielen werden dem Spieler zusätzlich eine weitere Auswahl vorgelegt.</br>
Zur Lösung der jeweiligen Quizaufgabe soll der Spieler die korrekte umsprangliche Bezeichnung der Pflanze oder des Tieres eintippen.</br>

## Ablauf

1. 20 Tiere werden als Kacheln angezeigt.
2. Der Spieler wählt 4 Tiere aus, die er auf jeden Fall benennen muss.
3. Das Benennen soll sofort erfolgen. Spieler wählt 1 von 4 aus und muss/kann sofort den Namen eingeben
4. Aus den verbleibenden 16 Tierkacheln werden dem Spieler noch 6 zufällig ausgewählte Tiere zur Benennung vorgelegt - dabei verschwinden allerdings die übrigen Karten (also anders als während der ersten 4 Karten)
5. Anschließend das gleiche Vorgehen für 20 Pflanzen
6. Dem Nutzer werden die 2 x 10 Fragen und die richtigen Antworten sowie die Nutzereingaben angezeigt

## Anforderungen Aufgabensteller

- die Anwendung muss auf den schuleigenen iPads laufen und per Touch-Eingabe komplett bedienbar sein
- es soll ausdrücklich keine Nutzerverwaltung /-authentifizierung eingerichtet werden, um Zustimmungspflichten der Eltern zu vermeiden
- trotzdem soll eine Session ID aus date + individuelle ID in die DB geschrieben werden
- als "Kontrollmechanismus" zur Vermeidung von mehrfachem Reload der Anwendung bei Schlechtleistung soll eine Stopuhr beim Start des Quiz beginnen zu laufen, die eine Abschätzung eines Neuladens nach erstem Durchlauf ermöglichen soll
- in einer Art Endbildschirm muss erkennbar sein, wie viele Fragen der Spieler richtig hatte
- der Endbildschirm / das Spielergebnis muss durch die Lehrkraft kontrollierbar sein und sollte entsprechend gegen versehentliches "Wegklicken" gesichert sein (Mehrfachbestätigung erforderlich, gar kein Fortschritt ohne Seite neu laden möglich etc)


### technische Herausforderungen

- Die Antwort des Spielers erfolgt durch Eingabe über die OnScreen-Tastatur des iPads. Dies verkleinert einerseits den darstellbaren Bereich und erfordert andererseits eine "Ähnlichkeitsprüfung" der Antwort (kein 100% richtiges Benennen erforderlich)