## Controlando el bote

El jugador controlará el objeto bote con el ratón.

\--- task \---

Añade código al objeto del barco para que comience en la esquina inferior izquierda apuntando hacia arriba y luego sigue el puntero del ratón.

![objeto-bote](images/boat_resize.png)

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

**Pruebe tu código** haciendo clic en la bandera verde y moviendo el ratón. ¿El obejto bote se mueve en dirección del puntero del ratón?

![captura de pantalla](images/boat-mouse.png)

\--- no-print \---

![captura de pantalla](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![captura de pantalla](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

¿Qué ocurre cuando el bote alcanza el puntero del ratón? Pruébalo para ver cual es el problema.

\--- /task \---

\--- task \---

Para evitar que esto ocurra, necesitas añadir un bloqueo `si`{:class="block3control"} en tu código para que el bote solo se mueva si se encuentra a más de 5 pixeles del puntero del ratón.

\--- hints \--- \--- hint \---

El bote sólo debe apuntar hacia el puntero del ratón y moverse `si`{:class="block3control"} la `distancia al puntero del ratón`{:class="block3sensing"} es `mayor que 5 píxeles`{:class="block3operators"}.

\--- /hint \--- \--- hint \---

Estos son los bloques de código que necesitas añadir al código del objeto del bote:

![objeto-bote](images/boat_resize.png)

```blocks3
si <[ ] > [ ]> entonces
end

(distancia a (puntero v))
```

\--- /hint \--- \--- hint \---

Así es como debería verse tu código:

![objeto-bote](images/boat_resize.png)

```blocks3
al presionar ⚑
apuntar en dirección (0)
ir a x: (-190) y: (-150)
por siempre 
  si <(distancia a (puntero v)) > [5]> entonces 
    apuntar hacia (puntero v)
    mover (1) pasos
  end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Prueba nuevamente tu código para verificar si el problema se encuentra resuelto.

\--- /task \---