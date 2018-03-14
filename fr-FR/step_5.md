## Collision!

En ce moment, ton bateau peut naviguer à travers les barrières en bois! Réglons ça.

+ Tu auras besoin de deux costumes pour ton bateau, un costume normal, et un pour quand le bateau se heurte. Dupliquer ton costume de bateau, et nommer un costume «normal» et l'autre «heurté».

+ Clique sur ton costume 'heurté', et choisis l'outil 'Selectionner' pour saisir les morceaux du bateau, les déplacer et les faire pivoter pour donner l'impression d'être heurté.
    
    ![screenshot](images/boat-hit-costume.png)

+ Now add code to your boat so that it crashes and breaks up when it touches any brown wooden bits.

\--- hints \--- \--- hint \--- You need to add code inside your `forever` loop so that your code keeps checking if the boat has crashed. `If` the boat is `touching` the brown colour of the wood, you need to `switch to the hit costume`, `say Noooo! for 2 seconds`, and then `switch back to the normal costume`. Finally, you'll need to `point up` and `go to the start position`. \--- /hint \--- \--- hint \--- Here are the code blocks you'll need: ![screenshot](images/boat-hit-blocks.png) \--- /hint \--- \--- hint \--- Here's what your code should look like: ![screenshot](images/boat-hit-code.png) \--- /hint \--- \--- /hints \---

+ You should also make sure that your boat always starts out looking 'normal'.
    
    If you try to sail through a wooden barrier now, you should see that your boat crashes and moves back to the start.
    
    ![screenshot](images/boat-crash.png)