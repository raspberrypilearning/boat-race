## Controlando el barco

El jugador controlará el objeto del barco con el ratón.

\--- task \---

Añade código al objeto del barco para que comience en la esquina inferior izquierda apuntando hacia arriba y luego sigue el puntero del ratón.

![objeto barco](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

**Prueba tu código** haciendo clic en la bandera verde y moviendo el ratón. ¿El objeto barco se mueve hacia el puntero del ratón?

![captura de pantalla](images/boat-mouse.png)

\--- no-print \---

![captura de pantalla](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![captura de pantalla](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

¿Qué pasa cuando el barco llega al puntero del ratón? Pruébalo para ver cuál es el problema.

\--- /task \---

\--- task \---

Para evitar que esto pase, tendrás que añadir a tu código un bloque`si`{:class="block3control"} a tu código, para que el barco solo se mueva si estás a más de 5 píxeles del ratón.

\--- hints \--- \--- hint \---

El barco sólo debe apuntar hacia el puntero del ratón y moverse `si`{:class="block3control"} la `distancia al puntero del ratón`{:class="block3sensing"} es `mayor que 5 píxeles`{:class="block3operators"}.

\--- /hint \--- \--- hint \---

Estos son los bloques de código que necesitas añadir al código del objeto del barco:

![objeto barco](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

\--- /hint \--- \--- hint \---

Así es como debería verse tu código:

![objeto barco](images/boat_resize.png)

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

Prueba de nuevo tu código para comprobar si el problema se ha solucionado.

\--- /task \---