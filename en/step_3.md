## Controlling the boat

--- task ---

You are going to control the boat with your mouse. Add code to your boat so that it starts in the bottom left corner pointing up and then follows the mouse pointer. __Test your code__ to make sure that it does what it's supposed to do.

![boat-sprite](images/boat_sprite.png
```blocks
when flag clicked
point in direction (0 v)
go to x: (-190) y: (-150)
forever
point towards [mouse-pointer v]
move (1) steps
```
--- task ---

Test out your boat by clicking the flag and moving the mouse. Does the boat sail towards the mouse?

 ![screenshot](images/boat-mouse.png)

 ![screenshot](images/boat-pointer-test-anim.gif)

--- /task ---

--- collapse ---
---
title: If you have problems ...
---
__Note:__ There is currently a bug in Scratch which means your boat may not move towards the mouse pointer. If this happens, click the arrow on the `point towards`{:class=”blocksensing”} block and re-select `mouse-pointer`{:class=”blocksensing”}.

![screenshot](images/boat-bug.png)
--- /collapse ---



--- task ---

What happens if the boat reaches the mouse pointer? Try it.

--- /task ---

--- task ---

To stop this from happening, you'll need to add an `if` block to your code, so that the boat only moves if it is more than 5 pixels away from the mouse.

--- hints ---
--- hint ---
The boat should only point towards the mouse pointer and move `if`{:class=”blockcontrol”} the `distance to the mouse pointer`{:class=”blocksensing”} is `greater than 5 pixels`{:class=”blockoperators”}.
--- /hint ---
--- hint ---
Here are the code blocks you'll need to add to the code for the boat:
![screenshot](images/boat-pointer-blocks.png)
--- /hint ---
--- hint ---
This is what your code should look like:
![boat-sprite](images/boat_sprite.png
```blocks
when flag clicked
point in direction (0 v)
go to x: (-190) y: (-150)
forever
+ if <(distance to [mouse-pointer v]) > [5]> then
point towards [mouse-pointer v]
move (1) steps
```
--- /hint ---
--- /hints ---

--- /task ---

--- task ---

Test out your boat again to check whether the problem has been fixed.

--- /task ---

