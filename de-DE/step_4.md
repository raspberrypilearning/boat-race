## Das Boot steuern

\--- task \---

Du wirst das Boot mit der Maus steuern. Füge deiner Bootsfigur Code hinzu, so dass sie in der unteren linken Ecke nach oben zeigend losfährt und dann dem Mauszeiger folgt. **Probiere deinen Code aus** um sicherzustellen, dass er tut was er soll.

\--- hints \--- \--- hint \--- Du wirst dein Boot, sobald die `grüne Flagge angeklickt wird`, `zur Startposition gehen` lassen und die `Richtung auf oben setzen` müssen. Als nächstes muss es `sich zum Mauszeiger drehen` und einen `1 er-Schritt gehen`. Das muss es `fortlaufend wiederholen`.

\--- /hint \--- \--- hint \--- Hier sind die Code-Blöcke, die du brauchen wirst: ![screenshot](images/boat-move-blocks.png) \--- /hint \--- \--- hint \--- So sollte dein Code aussehen: ![screenshot](images/boat-move-code.png) \--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Probiere dein Boot aus, indem du die grüne Flagge anklickst und die Maus bewegst. Fährt das Boot dem Mauszeiger hinterher?

![screenshot](images/boat-mouse.png)

![screenshot](images/boat-pointer-test-anim.gif)

## \--- collapse \---

title: Wenn du Probleme hast...

## image: images/image.png

**Note:** Es gibt momentan einen Fehler in Scratch, der dazu führt, dass dein Boot sich vielleicht nicht in Richtung des Mauszeigers bewegt. If this happens, click the arrow on the `point towards` block and re-select `mouse-pointer`.

![screenshot](images/boat-bug.png) \--- /collapse \---

\--- /task \---

\--- task \---

What happens if the boat reaches the mouse pointer? Try it.

\--- /task \---

\--- task \---

To stop this from happening, you'll need to add an `if` block to your code, so that the boat only moves if it is more than 5 pixels away from the mouse.

\--- hints \--- \--- hint \--- The boat should only point towards the mouse pointer and move `if` the `distance to the mouse pointer` is `greater than 5 pixels`. \--- /hint \--- \--- hint \--- Here are the code blocks you'll need to add to the code for the boat: ![screenshot](images/boat-pointer-blocks.png) \--- /hint \--- \--- hint \--- This is what your code should look like: ![screenshot](images/boat-pointer-code.png) \--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your boat again to check whether the problem has been fixed.

\--- /task \---