## Adicionar um temporizador

Agora poderás adicionar um cronómetro ao teu jogo, para que o jogador chegue à ilha o mais rápido possível.

\--- task \---

Cria uma nova variável chamada `tempo`{:class="block3variables"}.

![captura de ecrã](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Podes também escolher uma aparência para o teu cronómetro, alterando a forma como a nova variável é apresentada.

\--- /task \---

\--- task \---

Acrescenta blocos de código ao seu Palco para que o cronómetro contabilize o tempo que o barco leva a chegar à ilha.

\--- hints \--- \--- hint \---

No palco, `quando a bandeira verde é clicada` {: class = "block3control"}, ` define o tempo para 0 ` {: class = "block3variables"}. Dentro do teu ciclo ` para sempre ` {: class = "block3control"}, vais necessitar ` esperar 0,1 segundos ` {: class = "block3control"} e depois ` alterar o tempo em 0,1 ` {: class = "block3variables"}.

\--- /hint \--- \--- hint \---

Estes são os blocos de código de que necessitarás:

![palco](images/stage.png)

```blocks3
change [tempo v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [tempo v] to [0]
```

\--- /hint \--- \--- hint \---

Este é o aspeto que o teu código deve ter:

![palco](images/stage.png)

```blocks3
when flag clicked
set [tempo v] to [0]
forever
wait (0.1) seconds
change [tempo v] by (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Testa o teu jogo e vê com que rapidez consegues levar o teu barco até à ilha!

![captura de ecrã](images/boat-variable-test.png)

\--- /task \---