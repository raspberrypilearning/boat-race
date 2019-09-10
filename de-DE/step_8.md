## Zeitfahren

Also, dieses Spiel ist **echt** zu einfach, damit es interessanter wird, lass' uns einige Sachen ergänzen.

Fügen wir zuerst einige Beschleunigungen in dein Spiel ein, um das Boot schneller zu machen.

\--- task \---

Bearbeite dein Bühnenhintergrund und füge einige weiße Beschleunigungspfeile hinzu.

![Screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

Jetzt erweitere den Code in der `Wiederhole-fortlaufend`-Schleife des Bootes{:class="block3control"}, sodass es sich drei Schritte zusätzlich nach vorne bewegt, wenn es einen weißen Pfeil berührt. ![Boot-Figur](images/boat_resize.png)

```blocks3
wenn <touching color [#FFFFFF] ?> dann 
gehe (3) er Schritt
ende
```

\--- /task \---

\--- task \---

Teste dein Spiel, um zu sehen, ob das Boot durch die Beschleunigungspfeile schneller wird.

\--- /task \---

Als nächstes kannst du ein Drehtor hinzufügen, dass das Boot nicht berühren darf.

\--- task \---

Erstelle eine neue Figur die wie folgt aussieht und geb ihr den Namen “Drehtor”:

![screenshot](images/boat-gate.png)

Achte darauf, dass die Farbe der Figur "Drehtor" genau der braunen Farbe der Hindernisse auf der Bühne gleicht.

![Screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Stelle sicher, dass der Mittelpunkt des Drehtor-Sprite genau in der Mitte der Figur liegt

![Screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Füge den Code für die Hindernis Figur hinzu, damit es sich langsam und fortlaufend dreht.

\--- hints \--- \--- hint \--- Füge Code Blöcke zum Drehtor-Sprite hinzu, so dass es sich `drehe dich um 1Grad`{:class="block3motion"} `fortlaufend wiederholt`{:class="block3control"}. \--- /hint \--- \--- hint \--- Hier sind die Codeblöcke die du brauchst: ![Tor](images/gate.png)

```blocks3
wiederhole fortlaufend
ende

drehe dich im Uhrzeigersinn um (1) Grad

Wenn die grüne Flagge angeklickt wird
```

\--- /hint \--- \--- hint \--- So sollte dein neuer Programmiercode aussehen: ![Tor](images/gate.png)

```blocks3
Wenn grüne Flagge angeklickt wird
wiederhole fortlaufend
drehe dich im Uhrzeigersinn um (1) Grad
ende
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Teste dein Spiel. Du solltest jetzt ein drehendes Hindernis haben, das nicht berührt werden darf.

![Screenshot](images/boat-gate-test.png)

\--- /task \---