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

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
modifique el [tiempo v] por (0.1)

cuando la bandera sea cliquiada

siempre
fin

espere (0.1) segundos

establezca el [tiempo v] a [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

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

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---