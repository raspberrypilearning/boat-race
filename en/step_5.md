## Winning!

--- task ---
Now add another `if`{:class="blockcontrol"} statement to your boat sprite's code so that the player wins when they make the boat arrive at the yellow island.

When the boat gets to the island, the game should say 'YEAH!', and then it should end.

--- hints ---
--- hint ---
You need to add more code blocks inside your `forever`{:class="blockcontrol"} loop so that your code keeps checking if the player has won:

`if`{:class="blockcontrol"} the boat is `touching`{:class="blocksensing"} the colour of the island, you need to `say 'YEAH!' for 2 seconds`{:class="blocklooks"} and then `stop all`{:class="blockcontrol"} to end the game.
--- /hint ---
--- hint ---
Here are the code blocks you need:
![boat-sprite](images/boat_resize.png)
```blocks
say [YEAH!] for (2) secs

if <touching color [#FFFF99] ?> then
end

stop [all v]

```
--- /hint ---
--- hint ---
Here's what your new code should look like:
![boat-sprite](images/boat_resize.png)
```blocks
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) secs
stop [all v]
end
```

Don't forget that this new code needs to be inside the `forever`{:class="blockcontrol"} loop.
--- /hint ---
--- /hints ---
--- /task ---
