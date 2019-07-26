## Tilføjelse af en timer

Nu vil du tilføje en timer til dit spil, så spilleren skal komme til øen så hurtigt som muligt.

\--- task \---

Tilføj en ny variabel kaldet `time`{: class = "block3variables"} til dit trin.

![skærmbillede](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Du kan også vælge et kig efter din timer ved at ændre, hvordan din nye variabel vises.

\--- /task \---

\--- task \---

Tilføj nu kodeblokke til dit trin, så timeren tæller indtil båden når øen.

\--- hint \--- \--- tip \--- På scenen, `når det grønne flag er klikket`{: class = "block3control"}, sæt `klokken til 0`{: class = "block3variables "}. Inde i din `altid`loop: {{class = "block3control"} skal du først `vente 0,1 sekunder`{: class = "block3control"}, så `ændre tiden med 0,1`{: class = "block3variables" }. \--- / hint \--- \--- tip \--- Her er de kodeblokke du skal bruge: ![scene](images/stage.png)

```blocks3
ændre [tid v] med (0,1)

når flag klikket

evigt
slut

vente (0,1) sekunder

sæt [tid v] til [0]
```

\--- / hint \--- \--- tip \--- Her er, hvad din nye kode skal se ud: ![scene](images/stage.png)

```blocks3
når flag klikket
sæt [tid v] til [0]
evigt
vent (0,1) sekunder
skift [tid v] af (0,1)
ende
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Tjek dit spil og se, hvor hurtigt du kan få båden til øen!

![skærmbillede](images/boat-variable-test.png)

\--- /task \---