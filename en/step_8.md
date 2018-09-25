## Obstacles and power-ups

Right now this game is _far_ too easy - let's add things to make it more interesting.

--- task ---

Let's first add some 'boosts' to your game to speed up the boat. Edit your stage backdrop and add in some white booster arrows.

 ![screenshot](images/boat-boost.png)

--- /task ---

--- task ---

Now add some code to your boat's forever loop so that it moves three extra steps when it touches a white booster.

```blocks
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```
--- /task ---

--- task ---

You can also add a spinning gate which your boat will have to avoid. Add a new sprite called 'gate' that looks like this:

 ![screenshot](images/boat-gate.png)

 Make sure that the colour of the gate is the same as that of the wooden barriers.

--- /task ---

--- task ---

Set the center of the gate sprite.

 ![screenshot](images/boat-center.png)

--- /task ---

--- task ---

Add code to your gate to make it spin slowly forever.

--- hints ---
--- hint ---
Add code to the gate sprite so that it `turns 1 degree`{:class="blockmovement"} `forever`{:class="blockcontrol"}. {:class="block"}
--- /hint ---
--- hint ---
Here are the code blocks you'll need:
```blocks
forever
end

turn cw (1) degrees

when flag clicked
--- /hint ---
--- hint ---
Here's what your code should look like:
```blocks
when flag clicked
forever
turn cw (1) degrees
end
```
--- /hint ---
--- /hints ---

--- /task ---

--- task ---

Test out your game. You should now have a spinning gate that you must avoid.

 ![screenshot](images/boat-gate-test.png)

--- /task ---

