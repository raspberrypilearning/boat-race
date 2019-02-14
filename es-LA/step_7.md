## Añadir un temporizador

Añada un temporizador a su juego para que el jugador deba dejar la isla lo más rápido posible.

\--- task \---

Añada a su proyecto una nueva variable llamada `tiempo`.

![screenshot](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Además, puede elegir una aspecto para su temporizador al cambiar la manera en que se visualiza la nueva variable.

\--- /task \---

\--- task \---

Añada un bloqueo del código a su proyecto para que el temporizador cuente hasta que el bote llega a la isla.

\--- hints \--- \--- hint \--- En el proyecto, `cuando se seleccione el indicador verde`, `establezca el tiempo a 0`. Dentro del circuito `infinito`, necesitará primero `esperar 0.1 segundos`, luego `modifique el tiempo a 0.1`. \--- /hint \--- \--- hint \--- Here are the code blocks you'll need: ![stage](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![stage](images/stage.png)

```blocks3
when flag clicked
set [time v] to [0]
forever
wait (0.1) seconds
change [time v] by (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---