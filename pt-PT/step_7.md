## Adicionar um temporizador

Agora poderás adicionar um cronómetro ao teu jogo, para que o jogador chegue à ilha o mais rápido possível.

\--- task \---

Cria uma nova variável chamada `tempo`{:class="block3variables"}.

![captura de ecrã](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Podes também escolher uma aparência para o teu cronómetro, alterando a forma como a nova variável é apresentada.

\--- /task \---

\--- task \---

Acrescenta blocos de código ao seu Palco para que o cronómetro contabilize o tempo que barco leva a chegar à ilha.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
adiciona a [time v] o valor (0.1)

Quando alguém clicar na bandeira verde

repete para sempre
end

espera (0.1) s

altera [time v] para [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
quando alguém clicar na bandeira verde
altera [time v] para [0]
repete para sempre 
 espera (0.1) s
 adiciona a [time v] o valor (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---