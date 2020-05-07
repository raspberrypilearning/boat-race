## Obstáculos e impulsores

En este punto, el juego parece **muy** facil, por eso, necesitas añadir más elementos para hacerlo lucir más interesante.

Primero, debes añadir algunos impulsores para aumentar la velocidad del bote.

\--- task \---

Edita el fondo del Escenario agregando algunas flechas blancas impulsoras.

![captura de pantalla](images/boat-boost.png)

\--- /task \---

\--- task \---

Ahora, añade más bloques de código al circuito `por siempre` de tu bote para que se realice tres movimientos extra cuando esté en contacto con una flecha blanca.

![objeto-bote](images/boat_resize.png)

```blocks3
si <¿tocando el color [#FFFFFF] ?> entonces 
  mover (3) pasos
end
```

\--- /task \---

\--- task \---

Prueba tu juego para determinar si la nueva flecha impulsora aumenta la velocidad de tu bote.

\--- /task \---

A continuación, añade una puerta giratoria que el bote tiene que evitar.

\--- task \---

Añade un nuevo objeto que se vea así, y llámalo 'puerta':

![captura de pantalla](images/boat-gate.png)

Asegurate de que el color de la puerta sea el mismo que el de las vallas de madera.

![captura de pantalla](images/brown-hsv.png)

\--- /task \---

\--- task \---

Asegúrate de que el centro de la puerta se encuentre en el centro.

![captura de pantalla](images/boat-center.png)

\--- /task \---

\--- task \---

Añade tu código al objeto puerta para crear una rotación lenta infinita.

\--- hints \--- \--- hint \---

Añade bloques de código al objeto puerta para que `gire 1 grado`{:class="block3motion"} `por siempre`{:class="block3control"}.

\--- /hint \--- \--- hint \---

Aquí están los bloques de código que necesitas:

![puerta](images/gate.png)

```blocks3
por siempre
end

girar ↻ (1) grados

al presionar ⚑
```

\--- /hint \--- \--- hint \---

Así es como debería verse tu nuevo código:

![puerta](images/gate.png)

```blocks3
al presionar ⚑
por siempre 
  girar ↻ (1) grados
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Prueba tu juego nuevamente. Ahora, deberias tener una puerta giratoria que necesitas para mover el bote alrededor.

![captura de pantalla](images/boat-gate-test.png)

\--- /task \---