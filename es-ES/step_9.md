## Desafío: ¡Más obstáculos!
¿Puedes añadir más obstáculos a tu juego? Aquí te damos algunas ideas:

+ Podrías añadir cieno verde a tu escenario, que haga que el jugador vaya más lento cuando lo toque. Para hacer esto, puedes usar un bloque `espera`{:class="blockcontrol"}:

	```blocks
		esperar (0.01) segundos
	```

![screenshot](images/boat-algae.png)

+ ¡Podrías añadir un objeto en movimiento, como un tronco o un tiburón!

![screenshot](images/boat-obstacles.png)

Estos bloques pueden ayudarte:

	```blocks
		mover (1) pasos
		rebotar si toca un borde
	```

Si tu nuevo objeto no es marrón, tendrás que añadir lo siguiente al código de tu barco:

	```blocks
	si <<¿tocando el color [#603C15]?> o <¿tocando [tiburón v]?>> entonces
	fin
	```

