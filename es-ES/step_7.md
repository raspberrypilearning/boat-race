## Agregar un contador de tiempo

Ahora añadirás un cronómetro a tu juego, para que el jugador tenga que llegar a la isla lo más rápido posible.

\--- task \---

Añade a tu escenario una nueva variable llamada `tiempo`{:class="block3variables"}.

![captura de pantalla](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

También puedes elegir un aspecto para tu cronómetro cambiando cómo se muestra tu nueva variable.

\--- /task \---

\--- task \---

Ahora añade bloques de código a tu Escenario para que el cronómetro cuente hasta que el barco llegue a la isla desierta.

\--- hints \--- \--- hint \---

En el Escenario, `cuando se hace clic en la bandera verde`{:class="block3control"}, `fija el tiempo a 0`{:class="block3variables"}. Dentro de tu bucle `por siempre`{:class="block3control"}, necesitarás primero `esperar 0.1 segundos`{:class="block3control"}, luego `cambia el tiempo por 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Aquí están los bloques de código que necesitas:

![escenario](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

\--- /hint \--- \--- hint \---

Así es como debería verse tu nuevo código:

![escenario](images/stage.png)

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

¡Prueba tu juego y mira cómo de rápido puedes llevar el barco a la isla!

![captura de pantalla](images/boat-variable-test.png)

\--- /task \---