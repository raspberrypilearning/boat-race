## Sfida: Altri ostacoli!
Puoi aggiungere altri ostacoli al gioco? Ecco alcune idee:

+ Puoi aggiungere una melma verde al tuo scenario, che rallenta il giocatore quando la tocca. Per fare ciò, puoi usare un blocco `aspetta` {.blockcontrol}:

```blocks
	attendi (0.01) secondi
````

![screenshot](images/boat-algae.png)

+ Puoi aggiungere un oggetto in movimento, come un tronco o uno squalo!

![screenshot](images/boat-obstacles.png)

Questi blocchi possono aiutarti:

```blocks
	fai (1) passi
	rimbalza quando tocchi il bordo
````

Se il tuo nuovo oggetto non è marrone, dovrai aggiungere al tuo codice della barca:

```blocks
	se <<sta toccando il colore [#603C15]> o <sta toccando [shark v]>> allora
	end
```
