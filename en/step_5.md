## Winning!


When the boat gets to the island, the game should say 'YEAH!', and then it should end.

--- task ---

Add more code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the player has won:

Here's what your new code should look like:

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
+if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Noooooo!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

--- /task ---
