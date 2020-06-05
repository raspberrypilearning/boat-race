## Chocando

\--- task \---

Ahora añade otra declaración `si`{:class="block3control"} al código de tu objeto de barco para que el jugador gane cuando haga que el barco llegue a la isla amarilla.

Cuando el barco llega a la isla, el juego debería decir "SIII!", y entonces terminar.

\--- hints \--- \--- hint \---

Necesitas añadir más bloques de código dentro de tu bucle `por siempre`{:class="block3control"} para que tu código siga comprobando si el jugador ha ganado:

`si`{:class="block3control"} el barco está `tocando`{:class="block3sensing"} el color de la isla, tienes que `decir '¡SI! durante 2 segundos`{:class="block3looks"} y luego `parar todo`{:class="block3control"} para terminar la partida.

\--- /hint \--- \--- hint \---

Aquí están los bloques de código que necesitas:

![objeto barco](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \---

Así es como debería verse tu nuevo código:

![objeto barco](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

No olvides que este nuevo código debe estar dentro del bucle `por siempre`{:class="block3control"}.

\--- /hint \--- \--- /hints \--- \--- /task \---