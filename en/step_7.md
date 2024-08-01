## Adding a timer

Now you will add a timer to your game, so that the player has to get to the island as quickly as possible.

--- task ---

Make sure you have selected the Stage.

--- /task ---

--- task ---

Add a new variable called `time`{:class="block3variables"} to your Stage.

[[[generic-scratch3-add-variable]]]

You can change how your new variable is displayed.
 
![screenshot](images/boat-variable-annotated.png)

--- /task ---

--- task ---

Add code blocks to your Stage so that the timer counts up in tenths (0.1) of a second. 

Here's the code to add:

![stage](images/stage.png)

```blocks3
when flag clicked
set [time v] to [0]
forever
wait (0.1) seconds
change [time v] by (0.1)
end
```

--- /task ---

--- task ---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

--- /task ---
