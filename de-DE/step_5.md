## Absturz!

Im Moment kann dein Boot durch die Holz-Hindernisse segeln! Reparieren wir das.

+ Du wirst zwei Kostüme für dein Boot brauchen, ein normales Kostüm und eins, wenn das Boot abstürzt. Dupliziere dein Bootskostüm und nenne ein Kostüm "normal" und den anderen "Absturz".

+ Klicke auf das "abgestürzt"-Kostüm und wähle das Auswählen-Tool um Stücke des Boots zuzugreifen, zu bewegen und zu drehen, damit es abgestürzt aussieht.
    
    ![screenshot](images/boat-hit-costume.png)

+ Jetzt füge Code deinem Boot hinzu, damit es absturzt und zerbricht, wenn es braune Holzstücke berührt.

\--- hints \--- \--- hint \--- Du musst Code zu deinem `forever` Schleife hinfügen, damit dein Code immer wieder prüft, ob das Boot abgestürzt ist. `If` das Boot das Braun der Holz `touching` musst du `switch to the abgestürzt costume`, `say Noooo! für 2 Sekunden`, und dann `switch back to the normal costume`. Schließlich musst du `point up` und `go to the start position`. \--- /hint \--- \--- hint \--- Hier sind die Code-Blöcker, die du brauchen wirst: ![screenshot](images/boat-hit-blocks.png) \--- /hint \--- \--- hint \--- So sollte dein Code aussehen: ![screenshot](images/boat-hit-code.png) \--- /hint \--- \--- /hints \---

+ Du solltest auch sicherstellen, dass dein Boot immer zunächst "normal" aussieht.
    
    Wenn du jetzt versuchst, durch eine Holzbarriere zu segeln, solltest du sehen, dass dein Boot abstürzt und zur Startposition zurückfährt.
    
    ![screenshot](images/boat-crash.png)