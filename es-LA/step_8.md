## Obstáculos e impulsores

En este punto, el juego parece **muy** facil, por eso, necesita añadir más elementos para hacerlo lucir más interesante.

Primero, debe añadir algunos impulsores para aumentar la velocidad del bote.

\--- task \---

Edite el fondo del Escenario agregando algunas flechas blancas impulsoras.

![screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

Ahora, añade más bloqueos de código al circuito `por siempre` de tu bote para que se realice tres movimientos extra cuando esté en contacto con una flecha blanca.

![boat-sprite](images/boat_resize.png)

```blocks3
si <¿tocando el color [#FFFFFF] ?> entonces 
  mover (3) pasos
end
```

\--- /task \---

\--- task \---

Pruebe tu juego para determinar si la nueva flecha impulsora aumenta la velocidad de su bote.

\--- /task \---

Luego, añade una puerta giratoria que el bote deberá evitar.

\--- task \---

Añade un nuevo objeto que se vea así, y llámalo 'puerta':

![screenshot](images/boat-gate.png)

Asegurate de que el color de la puerta sea el mismo que el de las vallas de madera.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Asegurate de que el centro de la puerta se encuentre en el centro.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Añada el código al objeto puerta para crear una rotación lenta infinita.

\--- hints \--- \--- hint \---

Añade bloques de código al objeto de la puerta para que `gire 1 grado`{:class="block3motion"} `por siempre`{:class="block3control"}.

\--- /hint \--- \--- hint \---

Aquí están los bloques de código que necesitas:

![gate](images/gate.png)

```blocks3
por siempre
end

girar ↻ (1) grados

al presionar ⚑
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---