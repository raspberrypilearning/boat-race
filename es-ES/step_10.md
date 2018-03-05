--- challenge ---

## Desafío: ¡Más barcos!
¿Puedes convertir tu juego en una carrera entre 2 jugadores?

+ Duplica el barco, renómbralo 'Jugador 2' y cámbiale el color.

![screenshot](images/boat-p2.png)

+ Cambia este código para modificar la posición de inicio del Jugador 2:

	```blocks
		ir a x: (-190) y: (-150)
	```

+ Elimina el código que usa el ratón para controlar el barco:

	```blocks
		si < (distancia a [puntero del ratón v]) > [5] > entonces
			apuntar hacia [puntero del ratón v]
			mover (1) pasos
		fin
	```

...y reemplázalo con código para controlar el barco usando las teclas de flechas.

Éste es el código que necesitarás para mover el barco hacia adelante:

	```blocks
		si <¿tecla [flecha arriba v] presionada?> entonces
   		mover (1) pasos
	fin
	```

También necesitarás un código para `girar`{:class="blockmotion"} el barco cuando se presionen las teclas de flecha izquierda y derecha.

--- /challenge ---
