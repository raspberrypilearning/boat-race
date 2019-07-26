## ¡Ganador!

\--- task \--- Ahora añada otro estado `si` al código de su bote para que el jugador gane cuando logre que el bote llegue a la isla amarilla.

Cuando el bote llegue a la isla, el juego debería decir 'YEAH!' y luego debería terminar.

\--- hints \--- \--- hint \--- Necesitas agregar mas códigos de bloques dentro del `por siempre`{:class="block3control"} lazo asi tu código se mantiene verificando si el jugador a ganado:

`si`{:class="block3control"} el bote esta`tocando`{:class="block3sensing"} el color de la isla, necesitas `decir 'YEAH!' por 2 secondos`{:class="block3looks"} y despues `detener todo`{:class="block3control"} para finalizar el juego. \--- /hint \--- \--- hint \--- Estos son los bloqueos de código que necesitará: ![objeto-bote](images/boat_resize.png)

```blocks3
diga [YEAH!] durante (2) segundos

si <touching color [#FFFF99] ?> luego
fin

alto [todos los v]

```

\--- /hint \--- \--- hint \--- Asi es como tu nuevo código debería verse: ![objeto-bote](images/boat_resize.png)

```blocks3
si <touching color [#FFFF99] ?> luego
diga [YEAH!] durante (2) segundos
alto [todos los v]
fin
```

No olvide que este nuevo código necesita estar dentro del lazo `por siempre`{:class="block3control"}. \--- /hint \--- \--- /hints \--- \--- /task \---