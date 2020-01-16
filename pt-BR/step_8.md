## Obstáculos e aceleradores

Por enquanto o jogo está ** bastante ** fácil, então você adicionará algumas coisas para torná-lo mais interessante.

Primeiro, você adicionará alguns aceleradores para acelerar o barco.

\--- task \---

Edite o pano de fundo do Palco adicionando algumas setas de reforço brancas.

![screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

Agora adicione mais código ao bloco de repetição ` sempre ` {: class = "block3control"} de seu barco para que a imagem do barco mova três passos extras quando ele tocar uma seta branca.

![boat-sprite](images/boat_resize.png)

```blocks3
se <touching color [#FFFFFF] ?> então
mova (3) passos
fim
```

\--- /task \---

\--- task \---

Test your game to see whether your new booster arrows speed up the boat.

\--- /task \---

Next you'll add a spinning gate that the boat has to avoid.

\--- task \---

Add a new sprite that looks like this, and call it 'gate':

![screenshot](images/boat-gate.png)

Make sure that the colour of the gate sprite is the same as the colour of the wooden barriers.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \---

Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![gate](images/gate.png)

```blocks3
sempre
fim

gire para a direita (1) graus

quando ⚑ for clicado
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
quando ⚑ for clicado
sempre 
 gire para direita (1) graus
fim
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---