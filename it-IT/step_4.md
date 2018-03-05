## Scontro!

+ Avrai bisogno di 2 costumi per la tua barca, un costume normale e uno per quando la barca si scontra. Duplica il costume della tua barca, e assegna loro il nome 'normale' e 'colpito'.

+ Clicca sul tuo costume 'colpito' e scegli lo strumento 'Seleziona' per acchiappare pezzi della barca, e per muoverli e ruotarli. Fai apparire la tua barca come se si fosse scontrata.

	![screenshot](images/boat-hit-costume.png)

+ Aggiungi questo codice alla tua barca, dentro il loop 'per sempre' {.blockcontrol}, in modo che si schianti quando tocca qualsiasi pezzo di legno marrone:

	```blocks
		se <sta toccando il colore [#603C15]> allora
  			passa al costume [colpito v]
  			dire [Noooooo!] per (1) secondi
  			passa al costume [normale v]
  			punta in direzione (0 v)
  			vai a x: (-215) y: (-160)
		end
	```

	Questo codice si trova dentro il loop 'per sempre' {.blockcontrol}, per cui il tuo codice continua a controllare se la barca si è schiantata.

+ Ricordati di assicurarti che la tua barca appaia sempre 'normale'.

+ Se provi a navigare attraverso una barriera di legno, vedrai che la tua barca si schianta e ritornerà alla posizione iniziale.

	![screenshot](images/boat-crash.png)
