## Ganhando o jogo!

\--- task \--- Agora adicione outro comando `se` {:class="block3control"} para o código de seu barco para que o jogador ganhe quando ele fizer o barco chegar na ilha amarela.

Quando o barco chegar à ilha, o jogo deve dizer "Muito bem!" e então deve terminar.

\--- hints \--- \--- hint \--- Você precisa adicionar mais blocos de código dentro da repetição `sempre`{:class="block3control"} para que seu código continue verificando se jogador ganhou:

`Se`{:class="block3control"} o barco está tocando `tocando`{:class="block3sensing"} na cor da ilha, você precisa `dizer "Muito bem!" por 2 segundos`{:class="block3looks"} e depois ` pare todos`{:class="block3control"} para terminar o jogo. \--- /hint \--- \--- hint \--- Aqui estão os blocos que você precisa: ![boat-sprite](images/boat_resize.png)

```blocks3
diga [Muito bem!] por (2) segundos

se <tocando na cor [#ffff99]?> então 
fim

pare [todos v]

```

\--- /hint \--- \--- hint \--- Seu código deve ficar assim: ![boat-sprite](images/boat_resize.png)

```blocks3
se <tocando na cor [#ffff99]?> então
diga [Muito bem!] por (2) segundos
pare [todos v]
fim
```

Não esqueça que este novo código precisa estar dentro da repetição `sempre` {:class="block3control"}. \--- / hint \--- \--- / hints\--- \--- / task \---