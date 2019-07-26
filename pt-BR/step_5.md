## Ganhando o jogo!

\--- task \--- Agora adicione outro comando se ` if ` {: class = "block3control"} para o código de seu barco para que o jogador ganhe quando ele fizer o barco chegar na ilha amarela.

Quando o barco chegar à ilha deserta amarela, o jogo deve dizer "Muito bem!" e então terminar o jogo.

\--- hints \--- \--- hint \--- Você precisa adicionar código dentro do bloco de repetição `sempre` para que o seu código continue a verificar se jogador ganhou:

`Se` o barco está tocando `touching` na cor da ilha do tesouro, você precisa `dizer "Muito bem!" por 2 segundos` e depois ` pare todos` os códigos para terminar o jogo. \--- /hint \--- \--- hint \--- Aqui estão os blocos que você vai precisar: ![boat-sprite](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \--- Seu código deve ficar assim: ![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [Muito bem!] for (2) seconds
stop [all v]
end
```

Não esqueça que este novo código precisa estar dentro do bloco de repetição `sempre` {: class = "block3control"}. \--- / hint \--- \--- / hints\--- \--- / task \---