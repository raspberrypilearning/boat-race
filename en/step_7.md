## Time trial

Let's add a timer to your game, so that the player has to get to the desert island as quickly as possible.

--- task ---

Add a new variable called `time`{:class="blockdata"} to your stage. You can also change the display of your new variable.

 ![screenshot](images/boat-variable.png)

[[[generic-scratch-add-variable]]]

--- /task ---

--- task ---

Now add code to your Stage so that the timer counts up until the boat reaches the desert island.

--- hints ---
--- hint ---
On the Stage, `when the green flag is clicked`{:class="blockcontrol"}, `set the time to 0`{:class="blockdata"}. Inside your `forever`{:class="blockcontrol"} block, you'll need to first `wait 0.1 secs`{:class="blockcontrol"}, then `change the time by 0.1`{:class="blockdata"}.
--- /hint ---
--- hint ---
Here are the code blocks you'll need:
```blocks
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) secs

set [time v] to [0]
```
--- /hint ---
--- hint ---
Here's what your code should look like:
```blocks
when flag clicked
set [time v] to [0]
forever
wait (0.1) secs
change [time v] by (0.1)
end
```
--- /hint ---
--- /hints ---

--- /task ---

--- task ---

That's it! Test out your game and see how quickly you can get to the desert island!

 ![screenshot](images/boat-variable-test.png)

--- /task ---
