## Cómo controlar el barco

+ Si el líder de tu club te ha dado una carpeta de 'Recursos', haz clic en 'Cargar objeto desde archivo' y añade la imagen 'boat.png'. Deberías encoger el objeto y colocarlo en la posición de inicio.

	![screenshot](images/boat-boat.png)

	Si no tienes la imagen boat.png, ¡puedes dibujar tu propio barco!

+ Para poder controlar el barco con el ratón, añade este código al barco:

	```blocks
		al presionar bandera verde
		apuntar en dirección (0 v)
		ir a x: (-190) y: (-150)
		por siempre
			apuntar hacia [puntero del ratón v]
			mover (1) pasos
		fin
	```

+ Prueba tu barco haciendo clic en la bandera y moviendo el ratón. ¿Navega el barco hacia el ratón?

	![screenshot](images/boat-mouse.png)

+ ¿Qué ocurre si el barco llega al puntero del ratón?

	Para que esto no suceda, necesitarás añadir un bloque 'si'{.blockcontrol} a tu código, para que el barco sólo se mueva si está a más de 5 píxeles del ratón.

	![screenshot](images/boat-pointer.png)

+ Prueba tu barco una vez más para ver si se ha solucionado el problema.
