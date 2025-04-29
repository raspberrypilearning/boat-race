## Vencer!

Quando o barco chegar à ilha, o jogo deve dizer 'SIIIIMMM!' E depois deve terminar.

\--- task \---

Add more code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the player has won:

Este é o aspeto que o teu código deve ter:

```blocks3
when flag clicked
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Noooooo!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
+if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

\--- /task \---

\--- task \---

Test your code.

Click the green flag and make sure the game runs as expected. To make it a little easier to test, you can change the numbers in the first `go to`{:class="block3motion"} block to be this:

```blocks3
when flag clicked
switch costume to (normal v)
point in direction (0)
go to x: (150) y: (-90)
```

Don't forget to change it back once you've tested!

\--- /task \---