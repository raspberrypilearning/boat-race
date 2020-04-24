## Añadiendo un temporizador

Ahora agregaras un temporizador a tu juego, así que el jugador tiene que llegar a la isla lo mas rápido posible.

--- task ---

Agrega una nueva variable `tiempo`{:class="block3variables"} a tu escenario.

![captura de pantalla](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Además, puede elegir un aspecto para su temporizador al cambiar la manera en que se visualiza la nueva variable.

--- /task ---

--- task ---

Ahora agrega código de bloqueo a tu Escenario para que el temporizador cuente hasta que el bote llegue a la isla.

--- hints --- --- hint ---

En el Escenario, `cuando se hace clic en la bandera verde`{:class="block3control"}, `fija la hora a 0`{:class="block3variables"}. Dentro de tu ciclo`por siempre`{:class="block3control"}, necesitaras primero `esperar 0.1 secs`{:class="block3control"}, entonces `cambiar el tiempo por 0.1`{:class="block3variables"}.

--- /hint --- --- hint ---

Aquí están los bloques de código que necesitas:

![escenario](images/stage.png)

```blocks3
change [tiempo v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [tiempo v] to [0]
```

--- /hint --- --- hint ---

Así es como debería verse tu nuevo código:

![escenario](images/stage.png)

```blocks3
when flag clicked
set [tiempo v] to [0]
forever
wait (0.1) seconds
change [tiempo v] by (0.1)
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

¡Pruebe tu juego y ve que tan rápido puede mover el bote hacia la isla!

![captura de pantalla](images/boat-variable-test.png)

--- /task ---