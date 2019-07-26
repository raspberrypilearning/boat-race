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

\--- /task \---

\--- task \---

Certifique-se de que o centro do sprite (imagem) do portão esteja posicionado no meio da área de desenho.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Adicione código ao sprite do seu portão para fazê-lo girar sempre e lentamente.

\--- hints \--- \--- hint \--- Adicione blocos de código ao sprite (imagem) do portão para que ele ` gire 1 grau `, {: class = "block3motion"} ` sempre ` {: class = "block3control"}. \--- /hint \--- \--- hint \--- Aqui estão os blocos que você vai precisar: ![gate](images/gate.png)

```blocks3
forever
end

turn cw (1) degrees

when flag clicked
```

\--- /hint \--- \--- hint \--- Seu código deve ficar assim: ![gate](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Teste seu jogo novamente. Agora você deve ter um portão giratório do qual você precisa desviar com seu barco.

![screenshot](images/boat-gate-test.png)

\--- /task \---