## Challenge: More obstacles! 
Can you add more obstacles to your game? Here are some ideas:

+ You could add green slime to your backdrop, which slows the player down when they touch it. You can use a `wait` {.blockcontrol} block to do this:

```blocks
	wait (0.01) secs
````

![screenshot](images/boat-algae.png)

+ You could add a moving object, like a log or a shark!

![screenshot](images/boat-obstacles.png)

These blocks may help you:

```blocks
	move (1) steps
	if on edge, bounce
````

If your new object isn't brown, you'll need to add to your boat code:

```blocks
	if <  <touching color [#603C15]?> or <touching [shark v]?> > then
	end
```

### Save your project

##### 'Saving a Scratch project' ingredient (collapsible).
[[[saving-scratch]]]
