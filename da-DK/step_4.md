## Sammenstød!

I øjeblikket kan bådens sprite simpelthen sejle gennem træbarriererne! Du skal rette det nu.

\--- task \---

Du har brug for to kostumer til din bådsprite: et normalt kostume, og en til, når båden går i stykker. Dupliker dit bådsprit kostume, og navngiv et kostume 'normal' og det andet 'hit'.

\--- /task \---

\--- task \---

Klik på dit "hit" kostume, og brug **Select** værktøjet til at få fat i stykker af kostume og flyt og drej dem for at få båden til at se ud som om den er styrtet i stykker.

![skærmbillede](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Tilføj nu kode til din båd, så den nedbrud og bryder op, når det berører eventuelle brune træbarrierer.

\--- tip \--- \--- tip \--- Du skal føje kodeblokke inde i din `evigt`{: class = "block3control"} løkke, så din kode fortsætter med at kontrollere, om bådsprite er nedbrudt, og hvis den er styrtet, skal koden nulstille bådens sprite position.

`hvis`{: class = "block3control"} båden er `rørende`{: class = "block3sensing"} træets brune farve, skal du `skifte til hit kostume`{: class = "block3looks"} `siger nej! i 2 sekunder`{: class = "block3looks"}, og derefter `skift tilbage til det normale kostume`{: class = "block3looks"}. Endelig skal du `point op`{: class = "block3motion"} og `gå til startposition`{: class = "block3motion"}.

\--- / hint \--- \--- tip \--- Her er de kodeblokke du har brug for: ![båd-sprite](images/boat_resize.png)

```blocks3
hvis <touching color [ ] ?> så
slut

gå til x: (-190) y: (-150)

skift kostume til (hit v)

point i retning (0)

skift kostume til (normal v)

siger [Noooooo!] for (2) sekunder
```

\--- / hint \--- \--- hint \--- Her er hvad din kode skal se ud: ![båd-sprite](images/boat_resize.png)

```blocks3
når flag klikker
point i retning (0)
Gå til x: (-190) y: (-150)
evigt
hvis <(afstand til (musemarkør v)) > [5]> derefter
punkt mod pointer v)
træk (1) trin
ende
, hvis <touching color [#663b00] ?> derefter
switch kostume til (hit v)
sige [Noooooo!] for (2) sekunder
switch kostume til (normal v)
point i retning (0)
gå til x: (-190) y: (-150)
ende
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Du skal også tilføje kode for at sikre, at din bådsprite altid begynder at se 'normal'.

Test din kode igen. Hvis du forsøger at sejle båden gennem en træbarriere nu, skal båden gå ned og derefter gå tilbage til startpositionen.

![skærmbillede](images/boat-crash.png)

\--- /task \---