## Vinder!

\--- opgave \--- Tilføj nu en anden `hvis`{: class = "block3control"} erklæring til din bådsprites kode, så spilleren vinder, når de gør båden ankommer til den gule ø.

Når båden kommer til øen, skal spillet sige 'YEAH!', Og så skal det ende.

\--- tip \--- \--- tip \--- Du skal tilføje flere kodeblokke inde i din `evigt`{: class = "block3control"} løkke, så din kode fortsætter med at kontrollere, om spilleren har vundet:

`hvis`{: class = "block3control"} båden er `rørende`{: class = "block3sensing"} øens farve, skal du `sige 'YEAH!' i 2 sekunder`{: class = "block3looks"} og derefter `stop alle`{: class = "block3control"} for at afslutte spillet. \--- / hint \--- \--- hint \--- Her er de kodeblokke du har brug for: ![båd-sprite](images/boat_resize.png)

```blocks3
sig [YEAH!] for (2) sekunder

hvis <touching color [#FFFF99] ?> derefter
end

stop [all v]

```

\--- / hint \--- \--- tip \--- Her er, hvad din nye kode skal se ud: ![båd-sprite](images/boat_resize.png)

```blocks3
hvis <touching color [#FFFF99] ?> så
siger [YEAH!] for (2) sekunder
stop [all v]
end
```

Glem ikke, at denne nye kode skal være inde i `altid`{: class = "block3control"} loop. \--- / hint \--- \--- / hints \--- \--- / opgave \---