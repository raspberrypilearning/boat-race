## Obstáculos e ajudas

Neste momento, o jogo **está demasiado fácil**, portanto vamos adicionar algumas coisas ao jogo para o tornar mais interessante.

Primeiro, vais acrescentar algumas ajudas para acelerar o barco.

\--- task \---

Edita o teu palco para adicionar algumas setas brancas de ajuda.

![captura de ecrã](images/boat-boost.png)

\--- /task \---

\--- task \---

Adicione mais blocos de código ao ciclo ` para sempre ` {: class = "block3control"} do teu barco para que o ator barco avance três passos adicionais quando toca numa seta branca.

![boat-sprite](images/boat_resize.png)

```blocks3
se <estás a tocar na cor [#FFFFFF]>, então 
 anda (3) passos
end
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
repete para sempre
end

gira para a direita (1) º

Quando alguém clicar na bandeira verde
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

```blocks3
quando alguém clicar na bandeira verde
repete para sempre 
 gira para a direita (1) º
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---