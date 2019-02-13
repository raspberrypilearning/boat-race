## ¡Ganador!

\--- función \--- Ahora añada otro estado `si` al código de su bote para que el jugador gane cuando logre que el bote llegue a la isla amarilla.

Cuando el bote llegue a la isla, el juego debería indicar 'YEAH!' y luego debería terminar.

Necesitas añadir más bloqueo de códigos dentro de tu circuito `infinito` para que tu código continúe analizando si el jugador ha ganado:

`si` el bote se encuentra `tocando` el color de la isla, necesitarás que `diga'YEAH!' durante 2 segundos` y luego `detener todo` para finalizar el juego. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![boat-sprite](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

Don't forget that this new code needs to be inside the `forever`{:class="block3control"} loop. \--- /hint \--- \--- /hints \--- \--- /task \---