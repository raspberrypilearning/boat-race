## ¡Estrellado!

¡Por el momento, el bote solo puede navegar a través de las vallas de madera! Es el momento de solucionarlo.

--- task ---

Necesita dos disfraces para tu bote: un disfraz normal y uno para cuando el bote se estrelle. Duplique el disfraz de su bote y nombre a uno como "normal" y a otro como "golpe".

--- /task ---

--- task ---

Presione el disfraz "golpe" y utilice la herramienta **Seleccionar** para tomar las piezas del disfraz, moverlas y rotarlas para que el bote parezca que se ha estrellado en mil pedazos.

![captura de pantalla](images/boat-hit-costume-annotated.png)

--- /task ---

--- task ---

Ahora añada el código a su bote para que se estrelle y se destruya cuando toque alguna valla de madera marrón.

--- hints --- --- hint ---

Necesitas añadir bloques de código dentro de tu bucle `por siempre`{:class="block3control"} para que tu código siga comprobando si el objeto del barco se ha estrellado, y si se ha estrellado, el código necesita reiniciar la posición del objeto del barco.

`si`{:class="block3control"} el bote se encuentra `tocando`{:class="block3sensing"} tocando el color marrón de la madera, necesitará `modificar el disfraz de golpe`{:class="block3looks"}, `diga Noooo! durante 2 segundos`{:class="block3looks"}, y luego `regrese al disfraz normal`{:class="block3looks"}. Para finalizar, necesitará `señalar`{:class="block3motion"} y `dirijase a la posición inicial`{:class="block3motion"}.

--- /hint --- --- hint ---

Aquí están los bloques de código que necesitas:

![objeto-bote](images/boat_resize.png)

```blocks3
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to (golpe v)

point in direction (0)

switch costume to (normal v)

say [Noooooo!] for (2) seconds
```

--- /hint --- --- hint ---

Así es como debería verse tu código:

![objeto-bote](images/boat_resize.png)

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
switch costume to (golpe v)
say [Noooooo!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

También debería añadir un código para asegurarse de que su bote siempre comience luciendo "normal".

Pruebe su código nuevamente. Si ahora intenta navegar el bote a través de las vallas de madera, el mismo debería estrellarse y volver a la posición inicial.

![captura de pantalla](images/boat-crash.png)

--- /task ---