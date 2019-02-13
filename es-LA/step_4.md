## ¡Estrellado!

¡Por el momento, el bote solo puede navegar a través de las vallas de madera! Es el momento de solucionarlo.

\--- función \---

Necesitas dos atuendos para tu bote: un atuendo normal y uno para cuando el bote se estrelle. Duplica el atuendo de tu bote y nombra a uno como "normal" y a otro como "golpe".

\--- función \---

\--- función \---

Presione el atuendo "golpe" y utilice la herramienta **Seleccionar** para tomar las piezas del atuendo y moverlas y rotarlas para que el bote parezca que se ha estrellado en mil pedazos.

![screenshot](images/boat-hit-costume-annotated.png)

\--- función \---

\--- función \---

Ahora añada el código a su bote para que se estrelle y se destruya cuando toque alguna valla de madera marrón.

Necesitas añadir un bloqueo de código dentro de tu circuito `infinito` para que el código continue analizando si el bote se ha estrellado y, de ser así, el código deberá reiniciar la posición del bote.

`si` el bote se encuentra `touching` tocando el color marrón de la madera, necesitarás `modificar el atuendo de golpe`, `di Noooo! durante 2 segundos `, y luego ` regresa al atuendo normal`. Para finalizar, necesitarás `señalar` y `dirigirte a la posición inicial `.

Estos son los bloqueos de los códigos que necesitarás: ![boat-sprite](images/boat_resize.png)

```blocks3
si <touching color [ ] ?> luego
fin

dirigete a x: (-190) y: (-150)

modifica el atuendo a (golpe v)

muevete en dirección (0)

modifica el atuendo a (normal v)

di [Noooooo!] por (2) segundos
```

Así es como el código debería lucir: ![boat-sprite](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Noooooo!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---