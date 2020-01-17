## Collision!

Pour le moment, le sprite du bateau peut simplement naviguer à travers les barrières de bois! Tu vas résoudre ce problème maintenant.

\--- task \---

Tu auras besoin de deux costumes pour ton sprite bateau: un costume normal et un pour le crash du bateau. Duplique le costume de ton sprite bateau et nomme un costume "normal" et l'autre "touché".

\--- /task \---

\--- task \---

Clique sur ton costume "touché", et utilise l'outil **Sélectionner** pour récupérer des pièces du costume et les déplacer et les faire tourner pour le faire ressembler à bateau qui est détruit en plusieurs morceaux.

![capture d'écran](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Ajoute maintenant du code à ton bateau pour qu’il se brise au contact des barrières en bois brun.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
si <touching color [ ] ?> alors
fin

allez à x: (-190) y: (-150)

changez de costume en (touché v)

s'orienter en direction de (0)

basculer sur le costume (normal v)

dire [Noooonn!] pendant (2) secondes
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
lorsque le drapeau est cliqué
pointer dans la direction (0)
aller à x: (-190) y: (-150)
répéter indéfiniment
si <(distance de (pointeur de souris v)) > [5]> alors
s'orienter vers (pointeur de souris v)
déplacez de (1) pas
fin
si <touching color [#663b00] ?> alors
basculer sur le costume (touché v)
dire [Noooonn!] pendant (2) secondes
basculer sur le costume (normal v)
s'orienter en direction de (0)
aller à x: (-190) y: (-150)
fin
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---