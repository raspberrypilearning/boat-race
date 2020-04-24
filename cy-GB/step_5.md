## ¡Ganador!

\--- task \---

Ahora añade otra declaración `si`{:class="block3control"} al código de tu objeto de barco para que el jugador gane cuando haga que el barco llegue a la isla amarilla.

Cuando el bote llegue a la isla, el juego debería decir 'Siiiii!' y luego debería terminar.

\--- hints \--- \--- hint \---

Necesitas añadir más bloques de código dentro de tu bucle `por siempre`{:class="block3control"} para que tu código siga comprobando si el jugador ha ganado:

`si`{:class="block3control"} el bote esta`tocando`{:class="block3sensing"} el color de la isla, necesitas `decir 'Siiiii!' por 2 secondos`{:class="block3looks"} y despues `detener todo`{:class="block3control"} para finalizar el juego.

\--- /hint \--- \--- hint \---

Aquí están los bloques de código que necesitas:

![objeto-bote](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \---

Así es como debería verse tu nuevo código:

![objeto-bote](images/boat_resize.png)

```blocks3
si <¿tocando el color [#FFFF99] ?> entonces 
  decir [Siiiii!] por (2) segundos
  detener [all v]
end
```

No olvides que este nuevo código debe estar dentro del bucle `por siempre`{:class="block3control"}.

\--- /hint \--- \--- /hints \--- \--- /task \---