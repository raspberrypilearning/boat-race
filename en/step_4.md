## Step 3: Crashing!

Your boat can sail through the wooden barriers! Let's fix that.

### Activity Checklist

+ You'll need 2 costumes for your boat, one normal costume, and one for when the boat crashes. Duplicate your boat costume, and name them 'normal' and 'hit'.

+ Click on your 'hit' costume, and choose the 'Select' tool to grab bits of the boat and move and rotate them around. Make your boat look as if it's crashed.

	![screenshot](images/boat-hit-costume.png)
	
+ Now add code to your boat so that it crashes and breaks up when it touches any brown wooden bits. 

--- hints ---
--- hint ---
You need to add code _inside_ your __forever__ loop so that your code keeps checking if the boat has crashed. __if__ the boat is __touching__ the brown colour of the wood then you need to __switch to the hit costume__, __say Noooo! for 2 seconds__ and then __switch to the normal costume___. Then you'll need to __point up__ and __go to the start position__
--- /hint ---
--- hint ---
Here are the code blocks you'll need:
![screenshot](images/boat-hit-blocks.png)
--- /hint ---
--- hint ---
Here's how your code should look:
![screenshot](images/boat-hit-code.png)
--- /hint ---
--- /hints ---

+ You should also make sure that your boat always starts looking like it's 'normal'.

+ Now if you try to sail through a wooden barrier, you should see that your boat crashes and moves back to the start.

	![screenshot](images/boat-crash.png)
	

