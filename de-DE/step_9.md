## Herausforderung: Noch mehr Hindernisse!
Kannst Du noch mehr Hindernisse in dein Spiel einbauen? Hier sind ein paar Ideen:

+ Du kannst einen Schlammgebiet ins Bühnenbild einfügen, das das Boot verlangsamt, wenn es in den Schlamm reinsegelt. Nutze dafür das `warte`{:class="blockcontrol"} Skript:

```blocks
	warte (0.01) Sek.
````

![screenshot](images/boat-algae.png)

+ Du kannst ein Objekt einfügen, das sich ständig bewegegt, z.B. einen Holzklotz oder einen Hai sein!

![screenshot](images/boat-obstacles.png)

Diese Skripte können dir helfen:

```blocks
	gehe (1) er-Schritt
	pralle vom Rand ab
````

Wenn das neue Objekt ist nicht braun, denke dran, seine Farbe im Code aufzunehmen:

```blocks
	falls <<wird Farbe [#603C15] berührt?> oder <wird [shark v] berührt?>> dann
	Ende
```
