## Step 5: Obstacles and power-ups 

This game is _far_ too easy - let's add things to make it more interesting.

+ First let's add some 'boosts' to your game, which will speed up the boat. Edit your stage backdrop and add in some white booster arrows.

	![screenshot](images/boat-boost.png)

+  You can now add some code to your boat's `forever` loop, so that it moves 3 _extra_ steps when touching a white booster.

--- hints ---
--- hint ---
If your __boat__ is __touching a white booster__ then it should __move 3 extra steps__.  
--- /hint ---
--- hint ---
Here are the code blocks you'll need:
![screenshot](images/boat-boost-blocks.png)
--- /hint ---
--- hint ---
Here's how your code should look:
![screenshot](images/boat-boost-code.png)
--- /hint ---
--- /hints ---

+ You can also add in a spinning gate, which your boat has to avoid. Add in a new sprite called 'gate', which looks like this:

	![screenshot](images/boat-gate.png)

	Make sure that the colour of the gate is the same as the other wooden barriers.

+ Set the center of the gate sprite.

	![screenshot](images/boat-center.png)

+ Add code to your gate, to make it spin slowly `forever` {.blockcontrol}.

--- hints ---
--- hint ---
Add code to the __gate__ so that it __turns 1 degree__ __forever__.
--- /hint ---
--- hint ---
Here are the code blocks you'll need:
![screenshot](images/boat-spin-blocks.png)
--- /hint ---
--- hint ---
Here's how your code should look:
![screenshot](images/boat-spin-code.png)
--- /hint ---
--- /hints ---


+ Test out your game. You should now have a spinning gate that you must avoid.

	![screenshot](images/boat-gate-test.png)


