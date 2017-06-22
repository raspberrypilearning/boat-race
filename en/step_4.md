## Step 2: Controlling the boat

+ You are going to control the boat with your mouse. Add code to your boat so that it starts in the bottom left corner pointing up and then follows the mouse pointer. __Test your code__ (ingredient/definition) to make sure that it does what it's supposed to do.

--- hints ---
--- hint ---
Once the __green flag is clicked__, you'll need to make your boat __go to the start position__ and __point up__. Next it will need to __point towards the mouse pointer__ and __move 1 step__, it will need to repeat this __forever__.

--- /hint ---
--- hint ---
Here are the code blocks you'll need:
![screenshot](images/boat-move-blocks.png)
--- /hint ---
--- hint ---
Here's how your code should look:
![screenshot](images/boat-move-code.png)
--- /hint ---
--- /hints ---

+ Test out your boat, by clicking the flag and moving the mouse. Does the boat sail towards the mouse?

	![screenshot](images/boat-mouse.png)
	
	![screenshot](images/boat-pointer-test-anim.gif)

--- collapse ---
---
title: If you have problems ...
image: images/image.png
---
__Note: There is currently a bug in Scratch which means your boat may not move towards the mouse pointer. If this happens, click the arrow on the `point towards` block and re-select 'mouse-pointer'.__

![screenshot](images/boat-bug.png) 
--- /collapse ---


+ What happens if the boat reaches the mouse pointer? Try it. 

+ To stop this happening, you'll need to add an `if` block to your code, so that the boat only moves if it is more than 5 pixels away from the mouse.

--- hints ---
--- hint ---
The boat should only point towards the mouse pointer and move __if__ the __distance to the mouse pointer is greater than 5 pixels__.
--- /hint ---
--- hint ---
Here are the code blocks you'll need to add to the code for the boat:
![screenshot](images/boat-pointer-blocks.png)
--- /hint ---
--- hint ---
Here's how your code should look:
![screenshot](images/boat-pointer-code.png)
--- /hint ---
--- hint ---
Here's how you add the code:
![screenshot](images/boat-pointer-anim.gif)
--- /hint ---
--- /hints ---

+ Test out your boat again to check whether the problem has been fixed.
