## Zeitfahren

Also, dieses Spiel ist **echt** zu einfach - damit es interessanter wird, lass' uns einige Sachen ergänzen.

Fügen wir zuerst einige Beschleunigungen in dein Spiel ein, um das Boot schneller zu machen. 

\--- task \---

Bearbeite dein Bühnenbild und füge einige weiße Beschleunigungspfeile hinzu.

![Screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

Jetzt erweitere den Code in der Wiederhole-fortlaufend-Schleife des Bootes so, dass es sich drei Schritte zusätzlich nach vorne bewegt, wenn es einen weißen Pfeil berührt. ![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

\--- /task \---

\--- task \---

Teste dein Spiel, um zu sehen, ob das Boot schneller wird, sobald es einen weissen Pfeil berührt.

\--- /task \---

Als nächstes kannst du ein drehendes Hinderniss hinzufügen, dass das Boot nicht berühren darf.

\--- task \---

Erstelle eine neue Figur die wie folgt aussieht und geb ihr den Namen “Hindernis”:

![screenshot](images/boat-gate.png)

Achte darauf, dass die Farbe der Figur "Hindernis" genau der braunen Farbe der Hindernisse auf der Bühne gleicht.

\--- /task \---

\--- task \---

Die Mitte der neuen Figur muss in der Mitte des Balken liegen, damit er sich anschließend schön rund im Kreis bewegt.

![Screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Ergänze deinen Code zur Figur Hindernis, damit es sich langsam fortlaufend dreht.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![gate](images/gate.png)

```blocks3
forever
end

turn cw (1) degrees

when flag clicked
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![Screenshot](images/boat-gate-test.png)

\--- /task \---