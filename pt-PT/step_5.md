## Vencer!

--- task ---

Agora adiciona outro bloco `se`{:class="block3control"} ao código do ator barco, para que o jogador ganhe quando o barco chegar à ilha amarela.

Quando o barco chegar à ilha, o jogo deve dizer 'SIIIIMMM!' E depois deve terminar.

--- hints --- --- hint ---

Vais ter que adicionar blocos de código ao teu ciclo `para sempre`{:class="block3control"} para que o teu código verifique continuamente se o ator barco colidiu, e se tiver colidido, o código deve redefinir a posição do ator barco:

`se`{:class="block3control"} o barco está `a tocar`{:class="block3sensing"} na cor da ilha, vais precisar de `dizer 'SIIIIMMM!' durante 2 segundos`{:class="block3looks"} e depois `pára tudo`{:class="block3control"} para terminar o jogo.

--- /hint --- --- hint ---

Estes são os blocos de que necessitas:

![ator barco](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

--- /hint --- --- hint ---

Este é o aspeto que o teu código deve ter:

![ator barco](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

Não te esqueças que este novo código deve estar dentro do ciclo `para sempre`{:class="block3control"}.

--- /hint --- --- /hints --- --- /task ---