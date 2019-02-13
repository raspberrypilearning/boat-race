## Control del bote

El jugador controlará el bote con el ratón.

\--- función \--- Inserte el codigo en bote para que comience en la esquina inferior izquierda dirigido hacia arriba y que luego siga el señalador del ratón.

![boat-sprite](images/boat_resize.png)

```blocks3
cuando presione el indicador
señale en dirección (0)
dirijase a x: (-190) y: (-150)
siempre
dirijase hacia (señalador del ratón v)
muevase (1) paso
```

\--- función \---

\--- función \---

**Pruebe su codigo** presionando el indicador verde y moviendo el ratón. ¿El bote se mueve en dirección al señalador del ratón?

![screenshot](images/boat-mouse.png)

\--- no imprimir \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- no imprimir \---

\--- solo imprimir \--- ![screenshot](images/boat-pointer-test-anim.png) \--- solo imprimir \---

\--- función \---

\--- función \---

¿Qué ocurre cuando el bote alcanza el señalador del ratón? Pruébalo para ver cual es el problema.

\--- función \---

\--- función \---

Para evitar que esto ocurra, necesitas añadir un bloqueo `si`en tu codigo para que el bote solo se mueva si se encuentra a más de 5 pixeles del señalador del ratón.

\--- hints \--- \--- hint \--- The boat should only point towards the mouse pointer and move `if`{:class="block3control"} the `distance to the mouse pointer`{:class="block3sensing"} is `greater than 5 pixels`{:class="block3operators"}. \--- /hint \--- \--- hint \--- These are the code blocks you need to add to the code for the boat sprite: ![boat-sprite](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

\--- /hint \--- \--- hint \--- This is what your code should look like: ![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your code again to check whether the problem is now fixed.

\--- /task \---