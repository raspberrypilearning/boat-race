## Obstáculos e ajudas

Como está, o jogo **é demasiado fácil**, portanto vamos adicionar algumas coisas ao jogo para o tornar mais interessante.

Primeiro, irás acrescentar algumas ajudas para acelerar o barco.

--- task ---

Edita o teu palco para adicionar algumas setas brancas de ajuda.

![captura de ecrã](images/boat-boost.png)

--- /task ---

--- task ---

Adiciona mais blocos de código ao ciclo `para sempre`{:class="block3control"} do teu barco para que o ator barco avance três passos adicionais quando toca numa seta branca.

![ator barco](images/boat_resize.png)

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

--- /task ---

--- task ---

Testa o teu jogo para ver se as setas de ajuda que adicionaste, aceleram o barco.

--- /task ---

Agora, vais acrescentar um portão giratório que o barco deve evitar.

--- task ---

Adiciona um novo ator que se pareça com a barra horizontal como na figura e dá-lhe o nome 'portão':

![captura de ecrã](images/boat-gate.png)

Certifica-te de que a cor do ator portão é igual à das barreiras de madeira.

![captura de ecrã](images/brown-hsv.png)

--- /task ---

--- task ---

Certifica-te de que o centro do ator portão está posicionado no meio da barra.

![captura de ecrã](images/boat-center.png)

--- /task ---

--- task ---

Adiciona código ao seu ator portão para que gire lentamente para sempre.

--- hints --- --- hint ---

Adiciona blocos de código ao ator portão para que `gire 1 grau`{:class="block3motion"} `para sempre`{:class="block3control"}.

--- /hint --- --- hint ---

Estes são os blocos de que necessitas:

![portão](images/gate.png)

```blocks3
forever
end

turn cw (1) degrees

when flag clicked
```

--- /hint --- --- hint ---

Este é o aspeto que o teu código deve ter:

![portão](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

Testa o teu jogo novamente. Agora já deves ter um portão giratório que tens que contornar com o barco.

![captura de ecrã](images/boat-gate-test.png)

--- /task ---