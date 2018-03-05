## Controllare la barca

+ Controllerai la tua barca con il mouse. Aggiungi questo codice alla tua barca:

	```blocks
		quando si clicca sulla bandiera verde
		punta in direzione (0 v)
		vai a x: (-190) y: (-150)
		per sempre
  			punta verso [puntatore del mouse v]
  			fai (1) passi
		end
	```

+ Prova la tua barca cliccando la bandiera e muovendo il mouse. La barca naviga verso il mouse?

	![screenshot](images/boat-mouse.png)

	__Note: + Attualmente c'è un bug in Scratch a causa del quale la tua barca non riesce a muoversi in direzione del cursore del mouse. Se questo succede, clicca la freccia sul blocco 'punta verso' {.blockmotion} e riseleziona 'cursore-mouse'.

	![screenshot](images/boat-bug.png)

+ Che succede se la barca raggiunge il cursore del mouse?

	Per evitare che questo succeda, dovrai aggiungere un blocco 'if' {.blockcontrol} al tuo codice, in modo che la barca si muova solo se si trova a più di 5 pixel dal mouse.

	![screenshot](images/boat-pointer.png)

+ Prova di nuovo la tua barca per controllare se il problema è stato risolto.
