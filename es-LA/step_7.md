## Agregar un temporizador

Ahora agregaras un temporizador a tu juego, asi que el jugador tiene que llegar a la isla lo mas rápido posible.

\--- task \---

Agrega una nueva variable `tiempo`{:class="block3variables"} a tu escenario.

![captura de pantalla](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Además, puede elegir un aspecto para su temporizador al cambiar la manera en que se visualiza la nueva variable.

\--- /task \---

\--- task \---

Ahora agrega código de bloqueo a tu Escenario para que el temporizador cuente hasta que el bote llegue a la isla.

\--- hints \--- \--- hint \--- En el Escenario, `Cuando la bandera verde es presionada`{:class="block3control"}, `establecer el temporizador a 0`{:class="block3variables"}. Dentro de tu ciclo`infinito`{:class="block3control"}, necesitaras primero `esperar 0.1 secs`{:class="block3control"}, entonces `cambiar el tiempo por 0.1`{:class="block3variables"}. \--- /hint \--- \--- hint \--- Aqui estan los códigos de bloques que necesitaras: ![escenario](images/stage.png)

```blocks3
modifique el [tiempo v] por (0.1)

cuando la bandera sea cliquiada

siempre
fin

espere (0.1) segundos

establezca el [tiempo v] a [0]
```

\--- /hint \--- \--- hint \--- Asi es como tu nuevo código debería lucir: ![escenario](images/stage.png)

```blocks3
cuando la bandera es presionada
estableza el [tiempo v] a [0]
siempre
aguarde (0.1) segundos
modifique el [tiempo v] a (0.1)
fin
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

¡Pruebe tu juego y vea que tan rápido puede mover el bote hacia la isla!

![captura de pantalla](images/boat-variable-test.png)

\--- /task \---