## Zeitfahren

Also, dieses Spiel ist **echt** zu einfach - damit es interessanter wird, lass' uns einige Sachen ergänzen.

Fügen wir zuerst einige Beschleunigungen in dein Spiel ein, um das Boot schneller zu machen. 

\--- task \---

Bearbeite dein Bühnenbild und füge einige weiße Beschleunigungspfeile hinzu.

![Screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

Jetzt erweitere den Code in der Wiederhole-fortlaufend-Schleife des Bootes so, dass es sich drei Schritte zusätzlich nach vorne bewegt, wenn es einen weißen Pfeil berührt. ![Boot-Kostüm](images/boat_resize.png)

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

\--- hinweise \--- \--- hinweis \--- Fügen der Hindernis-Figur Codeblöcke hinzu, mit dem es sich ` fortlaufend ` {: class = "block3control"} ` um 1 Grad dreht ` {: class = "block3motion"}. \--- /hint \--- \--- hint \--- Hier sind die Codeblöcke die du brauchst: ![Hindernis](images/gate.png)

```blocks3
forever
end

turn cw (1) degrees

when flag clicked
```

\--- /hint \--- \--- hint \--- So sollte dein Programmiercode aussehen: ![Hindernis](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Teste dein Spiel. Du solltest jetzt ein rotierendes Hindernis haben, das nicht berührt werden darf.

![Screenshot](images/boat-gate-test.png)

\--- /task \---