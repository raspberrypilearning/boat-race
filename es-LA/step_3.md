## Control del bote

El jugador controlará el bote con el ratón.

\--- task \--- Inserte el código en el bote para que comience en la esquina inferior izquierda dirigido hacia arriba y que luego siga el señalador del ratón.

![bote](images/boat_resize.png)

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

**Pruebe su código** presionando el indicador verde y moviendo el ratón. ¿El bote se mueve en dirección al señalador del ratón?

![captura de pantalla](images/boat-mouse.png)

\--- no imprimir \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- no imprimir \---

\--- solo imprimir \--- ![screenshot](images/boat-pointer-test-anim.png) \--- solo imprimir \---

\--- /task \---

\--- task \---

¿Qué ocurre cuando el bote alcanza el señalador del ratón? Pruébalo para ver cual es el problema.

\--- /task \---

\--- task \---

Para evitar que esto ocurra, necesitas añadir un bloqueo `si` en tu codigo para que el bote solo se mueva si se encuentra a más de 5 pixeles del señalador del ratón.

El bote solo debería apuntar en sentido del señalador del ratón y moverse `si` la ` distancia hacia el señalador del ratón` es ` mayor a 5 pixeles`. Estos son los bloqueos de los códigos que necesitas incluir al código del bote: ![bote](images/boat_resize.png)

```blocks3
si < [ ] > [ ] > luego

(distancia hacia el (señalador del ratón))
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