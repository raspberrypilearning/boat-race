## Colisão!

Até ao momento, o ator barco pode simplesmente navegar através das barreiras de madeira! Agora vais corrigir isso.

\--- task \---

Vais necessitar de dois trajes para o ator barco: um normal e outro para quando o barco bater. Duplica o traje do teu ator barco e nomeia um traje como 'normal' e o outro como 'atingido'.

\--- /task \---

\--- task \---

Clica no teu traje 'atingido' e usa a ferramenta ** Selecionar ** para agarrar em partes do traje e mover-las de forma a parecer que o barco se fez em pedaços.

![captura de ecrã](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Agora adiciona código ao seu barco para que ele colida e se faça em pedaços quando toca em alguma das barreiras de madeira castanha.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
se <estás a tocar na cor []>, então
end

vai para a posição x: (-190) y: (-150)

muda o teu traje para (hit v)

altera a tua direcção para (0) °

muda o teu traje para (normal v)

diz [Noooooo!] durante (2) s
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
quando alguém clicar na bandeira verde
altera a tua direcção para (0) °
vai para a posição x: (-190) y: (-150)
repete para sempre 
 se <(a distância até (mouse-pointer v)) > [5]>, então 
 aponta em direcção a (mouse-pointer v)
 anda (1) passos
 end
 se <estás a tocar na cor [#663b00]>, então 
 muda o teu traje para (hit v)
 diz [Noooooo!] durante (2) s
 muda o teu traje para (normal v)
 altera a tua direcção para (0) °
 vai para a posição x: (-190) y: (-150)
 end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---