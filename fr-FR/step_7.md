## Ajouter un chronomètre

Tu vas maintenant ajouter une minuterie à ton jeu, de sorte que le joueur doive se rendre sur l'île le plus rapidement possible.

\--- task \---

Ajoute une nouvelle variable appelée `temps`{:class="block3variables"} à ta scène.

![capture d'écran](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Tu peux également choisir l'apparence de ta minuterie en modifiant le mode d'affichage de ta nouvelle variable.

\--- /task \---

\--- task \---

Ajoute maintenant des blocs de code à ta scène afin que le minuteur compte jusqu'à ce que le bateau atteigne l'île.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
ajouter (0.1) à [temps v]

lorsque le drapeau est cliqué

répéter indéfiniment
fin

attendre (0.1) secondes

mettre [temps v] sur [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
lorsque le drapeau est cliqué
mettre [temps v] à [0]
répéter indéfiniment
attendre (0.1) secondes
ajouter (0.1) à [heure v]
fin
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---