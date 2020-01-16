## ¡Estrellado!

¡Por el momento, el bote solo puede navegar a través de las vallas de madera! Es el momento de solucionarlo.

\--- task \---

Necesita dos atuendos para su bote: un atuendo normal y uno para cuando el bote se estrelle. Duplique el atuendo de su bote y nombre a uno como "normal" y a otro como "golpe".

\--- /task \---

\--- task \---

Presione el atuendo "golpe" y utilice la herramienta **Seleccionar** para tomar las piezas del atuendo y moverlas y rotarlas para que el bote parezca que se ha estrellado en mil pedazos.

![captura de pantalla](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Ahora añada el código a su bote para que se estrelle y se destruya cuando toque alguna valla de madera marrón.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
si <touching color [ ] ?> luego
fin

dirijase a x: (-190) y: (-150)

modifique el atuendo a (golpe v)

muevase en dirección (0)

modifique el atuendo a (normal v)

diga [Noooooo!] por (2) segundos
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
cuando presione el indicador
seleccione en dirección (0)
dirijase a x: (-190) y: (-150)
siempre
si <(la distancia hacia (el señalador del ratón v)) > [5]> luego
señale hacia (el señalador del ratón v)
muevase (1) paso
fin
si <touching color [#663b00] ?> luego
modifique el atuendo a (golpe v)
diga [Noooooo!] por (2) segundos
modifique el atuendo a (normal v)
seleccione en dirección (0)
dirijase a x: (-190) y: (-150)
fin
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---