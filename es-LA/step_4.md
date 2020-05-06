## Crashing!

¡Por el momento, el bote solo puede navegar a través de las vallas de madera! Es el momento de solucionarlo.

\--- task \---

Usted necesita dos disfraces para su bote: un disfraz normal y uno para cuando el bote se estrelle. Duplique el disfraz de su bote y nombre a uno como "normal" y a otro como "golpe".

\--- /task \---

\--- task \---

Haga clic sen su disfraz "golpe" y utilice la herramienta **Seleccionar** para tomar las piezas del disfraz, moverlas y rotarlas para que el bote parezca que se ha estrellado en mil pedazos.

![captura de pantalla](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Ahora añada el código a su bote para que se estrelle y se destruya cuando toque alguna valla de madera marrón.

\--- hints \--- \--- hint \---

Necesitas añadir bloques de código dentro de tu ciclo `por siempre`{:class="block3control"} para que tu código siga comprobando si el objeto del barco se ha estrellado, y si se ha estrellado, el código necesita reiniciar la posición del objeto del barco.

`si` el bote se encuentra `tocando` tocando el color marrón de la madera, necesitará `modificar el disfraz de golpe`, `diga Noooo! durante 2 segundos `, y luego ` regrese al disfraz normal`. Para finalizar, necesitará `la tecla flecha arriba` y `dirijase a la posición inicial`.

\--- /hint \--- \--- hint \---

Aquí están los bloques de código que necesitas:

![objeto-bote](images/boat_resize.png)

```blocks3
si <¿tocando el color [ ] ?> entonces
end
ir a x: (-190) y: (-150)
cambiar disfraz a (golpe v)
apuntar en dirección (0)
cambiar disfraz a (normal v)
decir [Noooooo!] por (2) segundos
```

\--- /hint \--- \--- hint \---

Así es como debería verse tu código:

![objeto-bote](images/boat_resize.png)

```blocks3
al presionar ⚑
apuntar en dirección (0)
ir a x: (-190) y: (-150)
por siempre 
  si <(distancia a (mouse-pointer v)) > [5]> entonces 
    apuntar hacia (puntero v)
    mover (1) pasos
  end
  si <¿tocando el color [#663b00] ?> entonces 
    cambiar disfraz a (golpe v)
    decir [Noooooo!] por (2) segundos
    cambiar disfraz a (normal v)
    apuntar en dirección (0)
    ir a x: (-190) y: (-150)
  end
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

También debería añadir un código para asegurarse de que su bote siempre comience luciendo "normal".

Pruebe su código nuevamente. Si ahora intenta navegar el bote a través de las vallas de madera, el bote debería estrellarse y volver a la posición inicial.

![captura de pantalla](images/boat-crash.png)

\--- /task \---