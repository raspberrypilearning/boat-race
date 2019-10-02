## Adicionando um cronômetro

Vamos adicionar um cronômetro a seu jogo para que o jogador tenha que chegar à ilha o mais rápido possível.

\--- task \---

Adicione uma nova variável chamada ` tempo` {: class = "block3variables"} ao Palco.

![screenshot](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Você também pode escolher um visual para seu timer, alterando a forma como sua nova variável é exibida.

\--- /task \---

\--- task \---

Agora adicione blocos de código ao Palco para que o cronômetro faça contagem do tempo até que o barco chegue à ilha.

\--- dicas \--- \--- dica \--- No painel Stage, ` quando a bandeira verde for clicada ` {: class = "block3control"}, ` defina o tempo como 0 ` {: class = "block3variables"}. Dentro do bloco ` sempre` {: class = "block3control"}, primeiro ` espere 0.1 segundos ` {: class = "block3control"}, então ` mude o tempo para 0.1 ` {: class = "block3variables"}. \--- /hint \--- \--- hint \--- Aqui estão os blocos que você vai precisar: ![stage](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

\--- /hint \--- \--- hint \--- Seu código deve ficar assim: ![stage](images/stage.png)

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

Teste seu jogo e veja quão rapidamente você pode levar o barco para a ilha!

![screenshot](images/boat-variable-test.png)

\--- /task \---