## Crashing!

At the moment, your boat can sail through the wooden barriers! Let's fix that.

--- task ---

You'll need two costumes for your boat, one normal costume, and one for when the boat crashes. Duplicate your boat costume, and name one costume 'normal' and the other 'hit'.

--- /task ---

--- task ---

Click on your 'hit' costume, and choose the Select tool to grab bits of the boat and move and rotate them around to make it look as if it's crashed.

 ![screenshot](images/boat-hit-costume.png)

--- /task ---

--- task ---

Now add code to your boat so that it crashes and breaks up when it touches any brown wooden bits.

--- hints ---
--- hint ---
You need to add code inside your `forever`{:class="blockcontrol"} loop so that your code keeps checking if the boat has crashed. `if`{:class="blockcontrol"} the boat is `touching`{:class="blocksensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="blocklooks"}, `say Noooo! for 2 seconds`{:class="blocklooks"}, and then `switch back to the normal costume`{:class="blocklooks"}. Finally, you'll need to `point up`{:class="blockmotion"} and `go to the start position`{:class="blockmotion"}.

--- /hint ---
--- hint ---
Here are the code blocks you'll need:
```blocks
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to [hit v]

point in direction (0 v)

switch costume to [normal v]

say [Noooooo!] for (2) secs
```
--- /hint ---
--- hint ---
Here's what your code should look like:
```blocks
when flag clicked
point in direction (0 v)
go to x: (-190) y: (-150)
forever
if <(distance to [mouse-pointer v]) > [5]> then
point towards [mouse-pointer v]
move (1) steps
end
+if <touching color [#663b00] ?> then
switch costume to [hit v]
say [Noooooo!] for (2) secs
switch costume to [normal v]
point in direction (0 v)
go to x: (-190) y: (-150)
end
```
--- /hint ---
--- /hints ---

--- /task ---

--- task ---

You should also make sure that your boat always starts out looking 'normal'.

 If you try to sail through a wooden barrier now, you should see that your boat crashes and moves back to the start.

 ![screenshot](images/boat-crash.png)

--- /task ---

