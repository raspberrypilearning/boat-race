## ¡Ganador!

\--- task \--- Ahora añada otro estado `si` al código de su bote para que el jugador gane cuando logre que el bote llegue a la isla amarilla.

Cuando el bote llegue a la isla, el juego debería indicar 'YEAH!' y luego debería terminar.

Necesita añadir más bloqueo de códigos dentro de su circuito `infinito` para que su código continúe analizando si el jugador ha ganado:

`si` el bote se encuentra `tocando` el color de la isla, necesitará que `diga'YEAH!' durante 2 segundos` y luego `detener todo` para finalizar el juego. \--- /hint \--- \--- hint \--- Estos son los bloqueos de código que necesitará: ![bote](images/boat_resize.png)

```blocks3
diga [YEAH!] durante (2) segundos

si <touching color [#FFFF99] ?> luego
fin

alto [todos los v]

```

\--- /hint \--- \--- hint \--- Así es como debería lucir el nuevo código:![bote](images/boat_resize.png)

```blocks3
si <touching color [#FFFF99] ?> luego
diga [YEAH!] durante (2) segundos
alto [todos los v]
fin
```

Recuerde que el nuevo código debe encontrarse dentro del circuito `infinito`. \--- /hint \--- \--- /hints \--- \--- /task \---