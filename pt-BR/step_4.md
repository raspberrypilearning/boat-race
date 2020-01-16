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

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
se <tocando na cor []?> então
fim

vá para x: (-190) y: (-150)

muda para a fantasia (batido v)

aponte para a direção (0)

muda para a fantasia (normal v)

diga [Nãooooo!] por (2) segundos
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

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

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---