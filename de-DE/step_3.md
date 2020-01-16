## Das Boot steuern

Der Spieler steuert das Boot mit der Computermaus.

\--- task \---

Füge deinem Boot-Sprite Code hinzu, so dass das Boot von der linken unteren Ecke mit Fahrtrichtung nach oben startet und dann dem Mauspfeil folgt.

![Boot-Sprite](images/boat_resize.png)

```blocks3
wenn grüne flagge angeklickt wird
setze Richtung auf (0) Grad
gehe zu x: (-190) y: (-150)
wiederhole fortlaufend
dreh dich zu (Mauszeiger v)
gehe (1) er Schritt
```

\--- /task \---

\--- task \---

**Teste deinen Code** indem du auf die grüne Flagge klickst und die Maus bewegst. Bewegt sich der Boot-Sprite in Richtung Mauszeiger?

![Screenshot](images/boat-mouse.png)

\--- no-print \---

![Screenshot](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![Screenshot](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

Was passiert, wenn das Boot deinen Mauszeiger erreicht? Probier es aus, um herauszufinden, wo das Problem liegt.

\--- /task \---

\--- task \---

Um dies zu vermeiden, musst du deinem Code einen `falls`{:class="block3control"} Block hinzufügen, sodass sich der Boot-Sprite nur dann bewegt, wenn es mindestens 5 Pixel vom Mauszeiger entfernt ist.

\--- hints \--- \--- hint \---

Das Boot sollte immer in Richtung Mauszeiger zeigen und sich nur bewegen `falls`{:class="block3control"} der `Abstand zum Mauszeiger`{:class="block3sensing"} `größer als 5 Pixel`{:class="block3operators"} ist.

\--- /hint \--- \--- hint \---

Hier sind die Programmblöcke, die du Programmcode des Boot-Sprites hinzufügen musst:

![Boot-Sprite](images/boat_resize.png)

```blocks3
wenn < [ ] > [ ] > dann

(Entfernung zu (Mauszeiger v))
```

\--- / hint \--- \--- hint \---

So sollte dein Code aussehen:

![Boot-Sprite](images/boat_resize.png)

```blocks3
Wenn grüne flagge angeklickt wird
setze Richtung auf (0) Grad
gehe zu x: (-190) y: (-150)
wiederhole fortlaufend
wenn <(Entfernung von (Mauszeiger v)) > [5]> dann
drehe dich zu (Mauszeiger v)
gehe (1) er Schritt
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Teste deinen Code erneut und überprüfe, ob das Problem nun gelöst ist.

\--- /task \---