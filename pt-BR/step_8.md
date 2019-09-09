## Obstáculos e aceleradores

Por enquanto o jogo está ** bastante ** fácil, então você adicionará algumas coisas para torná-lo mais interessante.

Primeiro, você adicionará alguns aceleradores para acelerar o barco.

\--- task \---

Edite o o pano de fundo do Palco adicionando algumas setas de reforço brancas.

![screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

Agora adicione mais código ao bloco de repetição ` sempre ` {: class = "block3control"} de seu barco para que a imagem do barco mova três passos extras quando ele tocar uma seta branca. ![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

\--- /task \---

\--- task \---

Teste seu jogo para ver se suas novas flechas de aceleração aceleram o barco.

\--- /task \---

Em seguida, você adicionará um portão giratório que o barco deve evitar.

\--- task \---

Adicione um novo sprite (imagem) com esta aparência e chame-a de "portao":

![screenshot](images/boat-gate.png)

Certifique-se de que a cor do sprite (imagem) do portão seja a mesma cor das barreiras de madeira.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![gate](images/gate.png)

```blocks3
forever
end

turn cw (1) degrees

when flag clicked
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---