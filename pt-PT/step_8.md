## Obstacles and boosters

Como está, o jogo **é demasiado fácil**, portanto vamos adicionar algumas coisas ao jogo para o tornar mais interessante.

Primeiro, irás acrescentar algumas ajudas para acelerar o barco.

\--- task \---

Edit your Stage backdrop by adding in some white booster arrows.

![screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

Adiciona mais blocos de código ao ciclo ` para sempre ` {: class = "block3control"} do teu barco para que o ator barco avance três passos adicionais quando toca numa seta branca.

![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

\--- /task \---

\--- task \---

Testa o teu jogo para ver se as setas de ajuda que adicionaste, aceleram o barco.

\--- /task \---

Next you'll add a spinning gate that the boat has to avoid.

\--- task \---

Adiciona um novo ator que se pareça com a barra horizontal como na figura e dá-lhe o nome 'portão':

![screenshot](images/boat-gate.png)

Make sure that the colour of the gate sprite is the same as the colour of the wooden barriers.

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Certifica-te de que o centro do ator portão está posicionado no meio da barra.

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
forever
end

turn cw (1) degrees

when flag clicked
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![gate](images/gate.png)

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