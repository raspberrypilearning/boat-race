## Controlando el bote

El jugador controlará el objeto bote con el ratón.

\--- task \--- Agreguar código al objeto bote para que comience en la esquina inferior izquierda apuntando hacia arriba y despues siguiendo el puntero del ratón.

![objeto-bote](images/boat_resize.png)

```blocks3
cuando presione el indicador
señale en dirección (0)
dirijase a x: (-190) y: (-150)
siempre
dirijase hacia (señalador del ratón v)
muevase (1) paso
```

\--- /task \---

\--- task \---

**Pruebe tu código** hacieno clic en la bandera verde y moviendo el ratón. ¿El obejto bote se mueve en dirección del puntero del ratón?

![captura de pantalla](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /no-print \---

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /no-print \---

\--- /task \---

\--- task \---

¿Qué ocurre cuando el bote alcanza el puntero del ratón? Pruébalo para ver cual es el problema.

\--- /task \---

\--- task \---

Para evitar que esto ocurra, necesitas añadir un bloqueo `if`{:class="block3control"} en tu código para que el bote solo se mueva si se encuentra a más de 5 pixeles del puntero del ratón.

\--- hints \--- \--- hint \--- El bote debería apuntar y moverse solamente hacia el puntero del ratón `if`{:class="block3control"} la `distancia hacia el puntero del ratón`{:class="block3sensing"} es `mayor de 5 pixeles`{:class="block3operators"}. \--- /hint \--- \--- hint \--- Estos son los códigos de bloque que necesitas agregar al código para el objeto bote: ![objeto-bote](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distancia a (mouse-pointer v))
```

Así es como debería lucir su código: ![bote](images/boat_resize.png)

```blocks3
cuando seleccione el indicador
señale en dirección (0)
dirijase a (-190) y: (-150)
siempre
si <(la distancia al (señalador del ratón v)) > [5]> luego
apunte hacia (el señalador del ratón v)
muevase (1) paso
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Puebe nuevamente su código para verificar si el problema se encuentra resuelto.

\--- /task \---