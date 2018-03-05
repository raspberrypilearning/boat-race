## ¡Choques!

¡Tu barco puede navegar a través de las barreras de madera! Vamos a arreglar eso.

+ Necesitarás 2 disfraces para tu barco, uno normal y otro para cuando el barco choque. Duplica el disfraz de tu barco y llámalos 'normal' y 'chocado'.

+ Haz clic en el disfraz 'chocado', y elige la herramienta 'Seleccionar' para separar trocitos del barco y moverlos y rotarlos por todos lados. Haz que parezca que tu barco ha chocado.

	![screenshot](images/boat-hit-costume.png)

+ Añade este código a tu barco, dentro del bucle `por siempre` {.blockcontrol}, para que choque cuando toque cualquier trozo de madera marrón:

	```blocks
	si <¿tocando el color [#603C15]?> entonces
   		cambiar disfraz a [chocado v]
   		decir [¡Noooooo!] por (1) segundos
   		cambiar disfraz a [normal v]
   		apuntar en dirección (0 v)
   		ir a x:(-215) y:(-160)
	fin
	```

	Este código está dentro del bucle `por siempre` {.blockcontrol}, para que tu código constantemente verifique si tu barco ha chocado.

+ También deberías asegurarte de que tu barco al principio siempre parezca 'normal'.

+ Ahora si intentas navegar a través de una barrera de madera, deberías ver cómo tu barco choca y vuelve al principio.

	![screenshot](images/boat-crash.png)
