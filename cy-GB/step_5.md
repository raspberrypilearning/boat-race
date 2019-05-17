## Ennill!

Nawr ychwanega ddatganiad `os`{:class="block3control"} i gôd dy gwch, fel bod y chwareuwr yn ennill pan mae nhw'n cyrraedd yr ynys.

Pan mae’r cwch yn cyrraedd y traeth melyn ar yr ynys, fe ddylai ddweud ‘HWRE!’ ac yna fe ddylai’r gêm orffen.

\--- hints \--- \--- hint \--- Bydd angen i ti ychwanegu mwy o flociau côd o fewn y ddolen `am byth`{:class="block3control"} fel bod y côd yn cadw gwirio os yw'r chwareuwr wedi ennill:

`os`{:class="block3control"} yw'r cwch yn `cyffwrdd`{:class="block3sensing"} lliw yr ynys, mae angen `dweud 'HWRE' am 2 eiliad`{:class="block3looks"} yna `stopiwch y cyfan`{:class="block3control"} i orffen y gêm. \--- /hint \--- \--- hint \--- Dyma'r blociau côd rwyt ti eu hangen: ![corlun-cwch](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \--- Dyma sut ddylai dy gôd edrych: ![corlun-cwch](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

Paid anghofio bod angen i'r côd yma fod o fewn dolen `am byth`{:class="block3control"}. \--- /hint \--- \--- /hints \--- \--- /task \---