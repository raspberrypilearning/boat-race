## Colisão!

Até ao momento, o ator barco pode simplesmente navegar através das barreiras de madeira! Agora vais corrigir isso.

\--- task \---

Vais necessitar de dois trajes para o ator barco: um normal e outro para quando o barco bater. Duplica o traje do teu ator barco e dá o nome 'normal' a um traje e o nome 'atingido' ao outro.

\--- /task \---

\--- task \---

Clica no teu traje 'atingido' e usa a ferramenta ** Selecionar ** para agarrar em partes do traje e mover-las de forma a parecer que o barco se fez em pedaços.

![captura de ecrã](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Agora adiciona código ao seu barco para que ele colida e se faça em pedaços quando toca em alguma das barreiras de madeira castanha.

\--- hints \--- \--- hint \---

Vais ter que adicionar blocos de código ao teu ciclo `para sempre` {: class = "block3control"} para que o código verifique continuamente se o ator barco colidiu, e se tiver colidido, o código deve redefinir a posição do ator barco.

` se ` {: class = "block3control"} o barco está a ` tocar ` {: class = "block3sensing"} na cor castanha da madeira, tens de ` mudar para o traje destruído ` {: class = "block3looks"}, ` diz Nãããooo! durante 2 segundos ` {: class = "block3looks"} e depois ` volta para o traje normal ` {: class = "block3looks"}. Finalmente, vais necessitar ` apontar ` {: class = "block3motion"} e ` ir para a posição inicial ` {: class = "block3motion"}.

\--- /hint \--- \--- hint \---

Estes são os blocos de que necessitas:

![ator barco](images/boat_resize.png)

```blocks3
se <touching color [ ] ?>, então
end

vai para a posição x: (-190) y: (-150)

muda o teu traje para (destruído)

altera a tua direcção para (0) °

muda o teu traje para (normal v)

diz [Noooooo!] durante (2) s
```

\--- /hint \--- \--- hint \---

Este é o aspeto que o teu código deve ter:

![ator barco](images/boat_resize.png)

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

Também deves acrescentar código para garantir que o ator barco começa sempre com a aparência 'normal'.

Testa o teu código novamente. Agora se tentares navegar através de uma barreira de madeira, o barco deve bater e voltar à sua posição inicial.

![captura de ecrã](images/boat-crash.png)

\--- /task \---