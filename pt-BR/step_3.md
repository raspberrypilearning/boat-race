## Controlando o barco

O jogador irá controlar o sprite (imagem) do barco com o mouse.

\--- task \--- Adicione o código à imagem do barco para que ele comece no canto inferior esquerdo apontando para cima e depois siga o ponteiro do mouse.

![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
point towards (mouse-pointer v)
move (1) steps
```

\--- /task \---

\--- task \---

** Teste seu código ** clicando na bandeira verde e movendo o mouse. O barco se move em direção ao ponteiro do mouse?

![screenshot](images/boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /no-print \---

\--- print-only \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /print-only \---

\--- /task \---

\--- task \---

O que acontece quando o barco alcança o ponteiro do mouse? Faça testes para identificar qual é o problema.

\--- /task \---

\--- task \---

Para impedir que isso aconteça, você precisará adicionar um bloco `se` a seu código, para que o barco mova-se apenas se estiver a mais de 5 pixels de distância do mouse.

\--- hints \--- \--- hint \--- O barco deve apontar em direção ao mouse e mover-se somente `se`{:class="block3control"} a`distância até o ponteiro do mouse`{:class="block3sensing"} for `maior que 5 pixels`{:class="block3operators"}. \--- / hint \--- \--- hint \--- Estes são os blocos de código que você precisa adicionar ao código da imagem do barco: ![boat-sprite](images/boat_resize.png)

```blocks3
if < [ ] > [ ] > then

(distance to (mouse-pointer v))
```

\--- /hint \--- \--- hint \--- Seu código deve ficar assim: ![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
```

\---/hints \--- \--- /hint \---

\--- /task \---

\--- task \---

Teste seu código novamente para verificar se o problema foi corrigido.

\--- /task \---