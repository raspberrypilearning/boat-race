## Challenge: More boats!
Can you turn your game into a race between 2 players?

+ Duplicate the boat, rename it 'Player 2' and change its colour.

![screenshot](images/boat-p2.png)

+ Change Player 2's starting position, by changing this code:

```blocks
	go to x: (-190) y: (-150)
```

+ Delete the code that uses the mouse to control the boat:

```blocks
	if < (distance to [mouse-pointer v]) > [5] > then
		point towards [mouse-pointer v]
		move (1) steps
	end
```

...and replace it with code to control the boat using the arrow keys.

This is the code you'll need to move the boat forward:

```blocks
	if < key [up arrow v] pressed? > then
		move (1) steps
	end
```

You'll also need code to `turn` {.blockmotion} the boat when the left and right arrow keys are pressed.

### Save your project

##### 'Saving a Scratch project' ingredient (collapsible).
[[[saving-scratch]]]
