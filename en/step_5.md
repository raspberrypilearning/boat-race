## Winning!

Now add another `if`{:class="blockcontrol"} statement to your boat's code, so that the player wins when they get to the desert island?

When the boat gets to the yellow desert island, the game should say 'YEAH!' and then it should stop. 

--- hints ---
--- hint ---
You need to more add code inside your `forever`{:class="blockcontrol"} loop so that your code keeps checking if the player has won. `if`{:class="blockcontrol"} the boat is `touching`{:class="blocksensing"} the colour of the treasure island, you need to `say 'YEAH!' for 2 seconds`{:class="blocklooks"} and then `stop all`{:class="blockcontrol"} to end the game. 
--- /hint ---
--- hint ---
Here are the code blocks you'll need:
![boat-sprite](images/boat_resize.png)
```blocks
say [YEAH!] for (2) secs

if <touching color [#FFFF99] ?> then
end

stop [all V]

```
--- /hint ---
--- hint ---
Here's what your code should look like:
![boat-sprite](images/boat_resize.png)
```blocks
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) secs
stop [all V]
end
```

Don't forget that the new code needs to be inside your `forever`{:class="blockcontrol"} loop. 
--- /hint ---
--- /hints ---

