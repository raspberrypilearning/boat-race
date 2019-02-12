## Uspešen!

\--- naloga \--- Sedaj dodajte še `izjavo <code> če`{: class = "block3control"} v kodo spritovega čolna, tako da bo igralec zmagal, ko bo ladja prispela na rumeni otok.

Ko bo čoln prispel do otoka, bi morala igra reči 'YEAH!' In potem se mora končati.

\--- namigi \--- \--- namig \--- svojo zanko `vedno`{: class = "block3control"} morate dodati več kodnih blokov, tako da vaša koda še naprej preverja, ali je igralec zmagal:

`če`{: class = "block3control"} čoln je `dotika`{: class = "block3sensing"} barva otoka, morate `reči "YEAH! za 2 sekundi`{: class = "block3looks"} in nato `ustavi vse`{: class = "block3control"}, da končate igro. \--- / namig \--- \--- namig \--- Tu so kodni bloki, ki jih potrebujete: ![čoln](images/boat_resize.png)

```blocks3
recite [YEAH!] za (2) sekundo

če <touching color [#FFFF99] ?> potem
konča

stop [vse v]

```

\--- / namig \--- \--- namig \--- Evo, kakšna naj bo vaša nova koda: ![čoln](images/boat_resize.png)

```blocks3
če <touching color [#FFFF99] ?> potem
pomeni [YEAH!] za (2) sekunde
stop [all v]
konec
```

Ne pozabite, da mora biti ta nova koda znotraj zanke `forever`{: class = "block3control"}. \--- / namig \--- \--- / namigi \--- \--- / naloga \---