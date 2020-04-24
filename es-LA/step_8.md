## Obstáculos e impulsores

En este punto, el juego parece **muy** facil, por eso, necesita añadir más elementos para hacerlo lucir más interesante.

Primero, debe añadir algunos impulsores para aumentar la velocidad del bote.

--- task ---

Edite el fondo del Escenario agregando algunas flechas blancas impulsoras.

![captura de pantalla](images/boat-boost.png)

--- /task ---

--- task ---

Ahora, añade más bloqueos de código al circuito `por siempre` de tu bote para que se realice tres movimientos extra cuando esté en contacto con una flecha blanca.

![objeto-bote](images/boat_resize.png)

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

--- /task ---

--- task ---

Pruebe tu juego para determinar si la nueva flecha impulsora aumenta la velocidad de su bote.

--- /task ---

Luego, añade una puerta giratoria que el bote deberá evitar.

--- task ---

Añade un nuevo objeto que se vea así, y llámalo 'puerta':

![captura de pantalla](images/boat-gate.png)

Asegurate de que el color de la puerta sea el mismo que el de las vallas de madera.

![captura de pantalla](images/brown-hsv.png)

--- /task ---

--- task ---

Asegurate de que el centro de la puerta se encuentre en el centro.

![captura de pantalla](images/boat-center.png)

--- /task ---

--- task ---

Añada el código al objeto puerta para crear una rotación lenta infinita.

--- hints --- --- hint ---

Añade bloques de código al objeto de la puerta para que `gire 1 grado`{:class="block3motion"} `por siempre`{:class="block3control"}.

--- /hint --- --- hint ---

Aquí están los bloques de código que necesitas:

![puerta](images/gate.png)

```blocks3
forever
end

turn cw (1) degrees

when flag clicked
```

--- /hint --- --- hint ---

Así es como debería verse tu nuevo código:

![puerta](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

Pruebe tu juego nuevamente. En este momento, debería haber una puerta giratoria y deberás mover el bote al rededor de la misma.

![captura de pantalla](images/boat-gate-test.png)

--- /task ---