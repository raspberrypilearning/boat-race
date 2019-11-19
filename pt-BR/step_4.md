## Batendo!

Por enquanto, o barco pode simplesmente navegar através das barreiras de madeira! Você vai corrigir isso agora.

\--- task \---

Você precisará de duas fantasias para representar o seu barco, uma fantasia normal e outra para quando o barco bater. Duplique a fantasia do barco e nomeie uma delas como "normal" e o outro como "batido".

\--- /task \---

\--- task \---

Clique na sua fantasia 'batido' e use a ferramenta de ** Selecionar ** para para mover e girar partes da fantasia e assim fazer parecer que o barco bateu e se quebrou.

![screenshot](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Agora adicione código ao seu barco para que ele bata e quebre quando ele tocar barreiras de madeira marrom.

\--- hints \--- \--- hint \--- Você precisa adicionar blocos de código dentro do bloco de repetição ` sempre` {: class = "block3control"} para que seu código continue verificando se o barco se chocou, e caso tiver se chocado, o código precisa reiniciar a posição do barco.

` se ` {:class="block3control"} o barco estiver ` tocando` {:class="block3sensing"} na cor marrom da madeira, você precisa mudar para a fantasia 'batida' com o bloco `mude para a fantasia 'batida' ` {:class="block3looks"}, ` e dizer Nãoooo! por 2 segundos ` {:class="block3looks"} e, em seguida, ` mude para a fantasia normal ` {:class="block3looks"}. Finalmente, você precisará ` apontar para cima ` {: class = "block3motion"} e ` ir para a posição inicial ` {:class="block3motion"}.

\--- /hint \--- \--- hint \--- Aqui estão os blocos que você vai precisar: ![boat-sprite](images/boat_resize.png)

```blocks3
se <tocando na cor []?> então
fim

vá para x: (-190) y: (-150)

muda para a fantasia (batido v)

aponte para a direção (0)

muda para a fantasia (normal v)

diga [Nãooooo!] por (2) segundos
```

\--- /hint \--- \--- hint \--- Seu código deve ficar assim: ![boat-sprite](images/boat_resize.png)

```blocks3
quando ⚑ for clicado
aponte para a direção (0)
vá para x: (-190) y: (-150)
sempre 
 se <(distância até (ponteiro do mouse v)) > [5]> então 
 aponte para (ponteiro do mouse v)
 mova (1) passos
 fim
 se <touching color [#663b00] ?> então 
 mude para a fantasia (batido v)
 diga [Nãoooo!] por (2) segundos
 mude para a fantasia (normal v)
 aponte para a direção (0)
 vá para x: (-190) y: (-150)
 fim
fim
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Você também deve ter certeza de que seu barco sempre comece com a fantasia "normal".

Teste seu código novamente. Se você tentar navegar o barco através de uma barreira de madeira agora, o barco deve colidir e então voltar para a sua posição inicial.

![screenshot](images/boat-crash.png)

\--- /task \---