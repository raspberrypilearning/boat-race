## Control del vaixell

El jugador controlarà l'sprite del vaixell amb el ratolí.

\--- task \--- Afegeix codi al vaixell per tal que comenci des de l'extrem inferior esquerre mirant cap amunt i després segueixi el cursor del ratolí.

![vaixell-sprite](images / boat_race_demo.png)

```blocks3
quan es fa clic a la bandera
apunta en la direcció (0)
ves a x: (-190) y: (-150)
infinitament
apunta cap a (punter del ratolí v)
moure (1) pas
```

\--- /task \---

\--- task \---

** Prova el teu codi ** fent clic a la bandera verda i movent el ratolí. L'sprite del vaixell es mou cap al punter del ratolí?

![screenshot](imatges / boat-mouse.png)

\--- no-print \--- ![screenshot](images/boat-pointer-test-anim.gif) \--- /no-print \---

\--- print-only \--- ![screenshot](images/boat-pointer-test-anim.png) \--- /print-only \---

\--- /task \---

\--- task \---

Què passa quan el vaixell arriba al punter del ratolí? Proveu-ho per veure quin és el problema.

\--- /task \---

\--- task \---

Per evitar que això passi, hauràs d’afegir un bloc condicional ` si `{: class = "block3control"} al teu codi, de manera que l'sprite del vaixell només es mou si és a més de 5 píxels de distància del punter del ratolí.

\--- hints \--- \--- hint \--- El vaixell hauria d'apuntar cap al ratolí i moure's ` si ` {: class = "block3control"} la ` distància al punter del ratolí ` {: class = "block3sensing"} és ` superior a 5 píxels ` {: class = "block3operators"}. \--- /hint \--- \--- hint \--- Aquests són els blocs de codi que has d’afegir al codi de l'sprite del vaixell: ![vaixell-sprite](images / boat_race_demo.png)

```blocks3
if < [ ] > [ ] > llavors

(distància amb el (punter del ratolí v))
```

\--- /hint \--- \--- hint \--- Això és el que hauria de tenir el vostre codi: ![vaixell-sprite](images / boat_race_demo.png)

```blocks3
quan es fa clic a la bandera
apunta en la direcció (0)
anar a x: (-190) y: (-150)
infinitament
si <(distància al (ratolí-punter v)) > [5]> continuació,
apunta al (punter del ratolí v)
avançar (1) pas
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Prova el teu codi de nou per comprovar si el problema està arreglat.

\--- /task \---