# EPR-3_Gruppenuebung_DiceGame

Die Aufgabe bringt bis zu 20 Punkte. 
Abgabe ist der 18.11.2017 um 16 Uhr. 

Aufgabe 3.2: Das Spiel
”16-ist-tot“ ist ein Knobelspiel, das haufig in Kneipen gespielt wird. Oft ist der
Einsatz das Bezahlen der n¨achsten Runde. Gew¨urfelt wird reihum mit einem W¨urfel.
Jeder Spieler darf solange w¨urfeln, wie er will, dieW¨urfe werden summiert und notiert.
Danach wird der Knobelbecher weiter gereicht. Ziel ist es, durch mehrmaliges Wurfeln
und aufsummieren der W¨urfelergebnisse so nahe an 16 zu kommen wie moglich. Wer
16 oder mehr erreicht, hat sofort verloren – das Spiel ist beendet. Es gelten folgende
Sonderregeln:
• Wer als Summenpunkte 9 erreicht, darf nicht mehr w¨urfeln. Der nachste Spieler
kommt dran.
• Wer als Summenpunkte 10 erreicht, muss noch einmal werfen. Erfolgt im programmierten
Spiel automatisch nach drei Sekunden Wartezeit.
Hat keiner der Spieler direkt verloren (also in Summe 16 oder mehr Punkte erreicht),
so verliert(en) diejenigen, die am wenigsten Punkte erreicht haben.


Aufgabe 3.3: Implementierung Punkte: / 13
Implementieren Sie dieses Spiel!
(a) (4 Punkte) Implementieren Sie eine Funktion roll dice(number=1, faces=6,
seed=None).
Diese Funktion gibt einen String zur¨uck, in dem die gew¨urfelten Zahlen im Intervall
[1..faces] durch Komma getrennt stehen. Es wird mit number Wurfeln (number
im Intervall [1,10]) gewurfelt, je mit faces Fl¨achen. faces ist aus dem Intervall
[2,100] zu w¨ahlen. Bei jedem W¨urfel soll die Verteilung der Zahlen m¨oglichst
gleichverteilt sein und im Intervall [1,faces] liegen. seed ist eine Float-Zahl, die
dem Quasi-Zufallszahlen Generator von Python als Parameter ubergeben wird.
Dies wird genutzt, um W¨urfelergebnisse wiederholbar (d.h. reproduzierbar) zu
machen.
(b) (4 Punkte) Implementieren Sie eine Funktion roll cheating dice(). Modifizieren
Sie dabei den W¨urfelwurf eines elektronischen W¨urfel mit 6 Fl¨achen (nur
diesen!) so, dass die Zahl 3 relativ mit der doppelten Wahrscheinlichkeit erscheint,
wie die anderen f¨unf Zahlen.
(c) (5 Punkte) Implementieren Sie eine Funktion sixteen is dead(players), welche
den Ablauf des gesamten Spiels implementiert. players bezeichnet dabei die
Anzahl an Spielern


Aufgabe 3.4: User Interface Punkte: / 4
Entwickeln Sie eine einfache Benutzungsschnittstelle auf Konsolenebene, die sich
durch Tastatureingaben bedienen lasst. Diese soll folgende M¨oglichkeiten bieten:
1. Dem Benutzer zu Beginn mittleilen, was g¨ultige Eingaben sind und was diese
bewirken. Dabei soll Eingabe <Return> das erneute W¨urfeln bewirken. Das Weiterreichen
des Knobelbechers zeigt man durch die Eingabe von n (f¨ur next) an.
2. Kennzeichnung, welcher Spieler gerade am Zug ist,
3. dem Benutzer des Spieles die Moglichkeit zu bieten, das Spiel jederzeit zu beenden
oder eine neue Runde zu starten,

Aufgabe 3.5: Fehlerbehandlung Punkte: / 3
Ihr User Interface soll robust angelegt sein, sodass falsche Eingaben des Benutzers
nicht zu einem Absturz f¨uhren.
