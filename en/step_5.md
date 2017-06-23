## Crashing!

At the moment, your boat can sail through the wooden barriers! Let's fix that.

+ You'll need two costumes for your boat, one normal costume, and one for when the boat crashes. Duplicate your boat costume, and name one costume 'normal' and the other 'hit'.

+ Click on your 'hit' costume, and choose the 'Select' tool to grab bits of the boat and move and rotate them around to make it look as if it's crashed.

	![screenshot](images/boat-hit-costume.png)
	
+ Now add code to your boat so that it crashes and breaks up when it touches any brown wooden bits. 

--- hints ---
--- hint ---
You need to add code _inside_ your __forever__ loop so that your code keeps checking if the boat has crashed. __If__ the boat is __touching__ the brown colour of the wood, you need to __switch to the hit costume__, __say Noooo! for 2 seconds__, and then __switch back to the normal costume__. Finally, you'll need to __point up__ and __go to the start position__.
--- /hint ---
--- hint ---
Here are the code blocks you'll need:
![screenshot](images/boat-hit-blocks.png)
--- /hint ---
--- hint ---
Here's what your code should look like:
![screenshot](images/boat-hit-code.png)
--- /hint ---
--- /hints ---

+ You should also make sure that your boat always starts out looking 'normal'.

If you try to sail through a wooden barrier now, you should see that your boat crashes and moves back to the start.

	![screenshot](images/boat-crash.png)
	

