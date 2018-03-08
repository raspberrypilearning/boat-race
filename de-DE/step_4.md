## Das Boot steuern

+ Du wirst das Boot mit der Maus steuern. Füge deinem Boot Code hinzu, damit es in der unteren linken Ecke beginnt, nach oben zeigt und dann dem Mauszeiger folgt. **Probiere deinen Code aus** um sicherzustellen, das er richtig funktioniert.

\--- hints \--- \--- hint \--- Sobald die `green flag is clicked`, wirst du dein Boot `go to the start position` (zu der Startposition bringen) and `point up` (nach oben zeigen). Als nächstes muss es `point towards the mouse pointer` und `move 1 step`. Es muss das `forever` wiederholen.

\--- /hint \--- \--- hint \--- Hier sind die Code-Blöcke, die du brauchen wirst: ![screenshot](images/boat-move-blocks.png) \--- /hint \--- \--- hint \--- So sollte dein Code aussehen: ![screenshot](images/boat-move-code.png) \--- /hint \--- \--- /hints \---

+ Probier dein Boot aus, in dem du an die Fahne klickst und die Maus bewegst. Segelt das Boot dem Mauszeiger gegenüber?
    
    ![screenshot](images/boat-mouse.png)
    
    ![screenshot](images/boat-pointer-test-anim.gif)

## \--- collapse \---

title: Wenn du Probleme hast...

## image: images/image.png

**Note:** Es gibt momentan einen Fehler in Scratch, der bedeutet, dass dein Boot sich vielleicht nicht in Richtung des Mauszeigers bewegt. In diesem Fall klicke den Pfeil auf dem `point towards` Block und wähle erneut `mouse-pointer`.

![screenshot](images/boat-bug.png) \--- /collapse \---

+ Was passiert, wenn das Boot den Mauszeiger erreicht? Versuch es.

+ Um dies zu verhindern, musst du einen `if` Block Sie zu deinem Code hinzufügen, damit das Boot nur sich bewegt, wenn es mehr als 5 Pixel von der Mauszeiger entfernt ist.

\--- hints \--- \--- hint \--- Das Boot sollte nur auf den Mauszeiger zeigen und sich bewegen `if` die `distance to the mouse pointer` /`greater than 5 pixels` ist. \--- /hint \--- \--- hint \--- Hier sind die Code-Blöcke, die du brauchen wirst, um den Code für das Boot hinzuzufügen: ![screenshot](images/boat-pointer-blocks.png) \--- /hint \--- \--- hint \--- So sollte dein Code aussehen: ![screenshot](images/boat-pointer-code.png) \--- /hint \--- \--- /hints \---

+ Probier dein Boot wieder aus, um zu prüfen, ob das Problem gelöst worden ist.