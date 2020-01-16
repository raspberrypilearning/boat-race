## Xocar!

De moment, l’sprite del vaixell només pot navegar per les barreres de fusta! Ara ho millorarem.

\--- task \---

Necessitaràs dues disfresses per al teu vaixell, una disfressa normal i una per quan el vaixell s'estavella. Duplica la disfressa del vaixell i anomena una disfressa "normal" i l'altra "xoc".

\--- /task \---

\--- task \---

Fes clic a la disfressa "xoc" i fes servir l'eina ** Selecciona ** per agafar trossos de la disfressa, moure'ls i fer-los girar per fer que el vaixell sembli que s'ha estavellat.

![screenshot](images / boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Ara afegeix codi al teu vaixell perquè xoqui i es trenqui quan toca els trossos de fusta marró.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
si <touching color [ ] ?> llavors
fi

anar a x: (-190) y: (-150)

canviar la disfressa a (xoc v)

apuntar en direcció (0)

canviar la disfressa a (normal v)

dir [Noooooo!] durant (2) segons
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
quan es fa clic a la bandera
apuntar en la direcció (0)
anar a x: (-190) y: (-150)
infinitament
si <(distància del (punter del ratolí v)) > [5]> llavors,
apuntar al (punter del ratolív)
avançar (1) passos
fi
si <touching color [#663b00] ?> llavors
canviar disfressa a (xoc v)
dir [noooooo!] durant (2) segons
canviar disfressa a ( normal v)
apuntar en la direcció (0)
anar a x: (-190) y: (-150)
fi
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---