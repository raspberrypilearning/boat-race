## Einen Unfall bauen!

Im Moment kann dein Boot einfach durch die hölzernen Hindernisse segeln! Reparieren wir das.

\--- task \---

Du wirst zwei Kostüme für dein Boot brauchen, ein normales Kostüm und eins, wenn das Boot einen Unfall hat. Dupliziere dein Bootskostüm "**normal**" und nenne das neue Kostüm "**Unfall**".

\--- /task \---

\--- task \---

Klicke auf das "**Unfall**" -Kostüm und wähle den Befehlen ** Auswählen ** aus, um Teile des Kostüms zu greifen, zu bewegen und zu drehen. Das Boot soll am Ende total kaputt aussehen.

![Screenshot](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Jetzt füge deinem Boot neuen Code hinzu, so dass es auseinander bricht, sobald es braune Holzteile berührt.

\--- Hinweise \--- \--- Hinweis \--- Du musst dem Code in deiner ` wiederhole fortlaufend ` {: class = "block3control"}-Schleife ergänzen, damit er immer wieder prüft, ob das Boot einen Unfall hat. <0> Falls </0> {: class = "block3control"} das Boot das Braun des Holzes <0> berührt </0> {: class = "block3control"}, musst du <0> zum Unfall-Kostüm wechseln </0> {: class = "block3control"}, <0> Oh nein! sagen für 2 Sekunden </0> {: class = "block3control"} und anschließend wieder <0> zum normalen Kostüm wechseln </0> {: class = "block3control"}. Schließlich musst du <0> die Richtung auf "oben" setzen </0> {: class = "block3control"} und <0> zur Startposition gehen </0> {: class = "block3control"}.

`wenn`{:class="block3control"} das Boot `berührt`{:class="block3sensing"} die braune Farbe des Holzes berührt, musst du `zum Unfall Kostüm wechseln`{:class="block3looks"}, ` und Ohn nein! sagen. für 2 Sekunden`{:class="block3look"}, und anschließend `zurück zum normalen Kostüm wechseln`{:class="block3look"}. Als letztes musst du das Köstum `nach oben`{:class="block3motion"} zeigen lassen und `zur Startposition gehen`{:class="block3motion"}.

\--- /hint \--- \--- hint \--- Hier sind die Codeblöcke die du brauchst: ![Boot-Kostüm](images/boat_resize.png)

```blocks3
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to (hit v)

point in direction (0)

switch costume to (normal v)

say [Oh nein!] for (2) seconds
```

\--- /hint \--- \--- hint \--- So sollte dein Programmiercode aussehen: ![Boot-Kostüm](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Oh nein!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Du solltest auch sicherstellen, dass dein Boot zu Beginn eines Spiels immer "normal" aussieht und somit dieses Kostüm trägt.

Teste deinen Code erneut. Wenn dein Boot nun versucht durch einenhölzerne Barriere zu segeln, sollte das Boot zu dem Unfall Look wechseln, Oh nein! sagen und anschließend zur Startpoition zurückkehren.

![screenshot](images/boat-crash.png)

\--- /task \---