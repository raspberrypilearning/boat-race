## Obstacles and power-ups 

Right now this game is _far_ too easy - let's add things to make it more interesting.

+ Let's first add some 'boosts' to your game to speed up the boat. Edit your stage backdrop and add in some white booster arrows.

	![screenshot](images/boat-boost.png)

+ Now add some code to your boat's _forever_ loop so that it moves three _extra_ steps when it touches a white booster.

--- hints ---
--- hint ---
__If__ your __boat__ is __touching a white booster__, then it should __move 3 extra steps__.  
--- /hint ---
--- hint ---
Here are the code blocks you'll need:
![screenshot](images/boat-boost-blocks.png)
--- /hint ---
--- hint ---
Here's what your code should look like:
![screenshot](images/boat-boost-code.png)
--- /hint ---
--- /hints ---

+ You can also add a spinning gate which your boat will have to avoid. Add a new sprite called 'gate' that looks like this:

	![screenshot](images/boat-gate.png)

	Make sure that the colour of the gate is the same as that of the wooden barriers.

+ Set the center of the gate sprite.

	![screenshot](images/boat-center.png)

+ Add code to your gate to make it _spin_ slowly _forever_ {.blockcontrol}.

--- hints ---
--- hint ---
Add code to the __gate__ so that it __turns 1 degree__ __forever__.
--- /hint ---
--- hint ---
Here are the code blocks you'll need:
![screenshot](images/boat-spin-blocks.png)
--- /hint ---
--- hint ---
Here's what your code should look like:
![screenshot](images/boat-spin-code.png)
--- /hint ---
--- /hints ---


+ Test out your game. You should now have a spinning gate that you must avoid.

	![screenshot](images/boat-gate-test.png)


