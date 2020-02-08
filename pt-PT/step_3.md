## Controlar o barco

O jogador controlará o ator barco com o rato.

\--- task \---

Adiciona código ao ator barco para que ele comece no canto inferior esquerdo a apontar para cima e que depois siga o ponteiro do rato.

![ator barco](images/boat_resize.png)

```blocks3
quando alguém clicar na bandeira verde
altera a tua direcção para (0) °
vai para a posição x: (-190) y: (-150)
repete para sempre 
 aponta em direcção a (ponteiro do rato v)
 anda (1) passos
end
```

\--- /task \---

\--- task \---

** Testa o teu código ** clicando na bandeira verde e movendo o rato. O actor barco move-se em direção ao ponteiro?

![captura de ecrã](images/boat-mouse.png)

\--- no-print \---

![captura de ecrã](images/boat-pointer-test-anim.gif)

\--- /no-print \---

\--- print-only \---

![captura de ecrã](images/boat-pointer-test-anim.png)

\--- /print-only \---

\--- /task \---

\--- task \---

O que é que acontece quando o barco atinge o ponteiro do rato? Experimenta para ver qual é o problema.

\--- /task \---

\--- task \---

Para impedir que isto aconteça, deve adicionar o bloco ` se ` {: class = "block3control"} ao código, para que o ator barco se mova apenas quando estiver a mais de 5 pixeis do ponteiro do rato.

\--- hints \--- \--- hint \---

O barco deve apontar apenas para o ponteiro do rato e deslocar-se `se` {: class = "block3control"} a distância ` para o ponteiro do rato` {: class = "block3sensing"} fôr ` maior do que 5 píxeis ` {: class = "block3operators"}.

\--- /hint \--- \--- hint \---

Estes são os blocos que necessitas de acrescentar ao código para do ator barco:

![ator barco](images/boat_resize.png)

```blocks3
se < [ ] > [ ] > , então
end

(a distância até (ponteiro do rato v))
```

\--- /hint \--- \--- hint \---

Este é o aspeto que o teu código deve ter:

![ator barco](images/boat_resize.png)

```blocks3
quando alguém clicar na bandeira verde
altera a tua direcção para (0) °
vai para a posição x: (-190) y: (-150)
repete para sempre 
 se <(a distância até (ponteiro do rato v)) > [5]>, então 
 aponta em direcção a (ponteiro do rato v)
 anda (1) passos
 end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Testa o teu código novamente para verificar se o problema está resolvido.

\--- /task \---