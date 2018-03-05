## Prueba de tiempo

Vamos a añadir un cronómetro a tu juego para que el jugador tenga que llegar a la isla lo más rápido posible.

+ Añade a tu escenario una nueva variable que se llame `tiempo` {.blockdata}. También puedes cambiar la visualización de tu nueva variable. Si necesitas ayuda, echa un vistazo al proyecto "Globos".

	![screenshot](images/boat-variable.png)

+ Añade este código a tu __escenario__, para que el cronómetro cuente hasta que el barco alcance la isla desierta:

	```blocks
		al presionar bandera verde
		fijar [tiempo v] a [0]
		por siempre
			esperar (0.1) segundos
			cambiar [tiempo v] por (0.1)
		fin
	```

+ ¡Ya lo tienes! ¡Prueba tu juego para ver cómo de rápido puedes llegar a la isla desierta!

	![screenshot](images/boat-variable-test.png)
