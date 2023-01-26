## Ennill!

\--- task \---

Pan mae’r cwch yn cyrraedd y traeth melyn ar yr ynys, fe ddylai ddweud ‘Hwre!’ ac yna fe ddylai’r gêm orffen. make my changes

completely retranslate this sentence

\--- hints \--- \--- hint \---

\--- /hint \--- \--- hint \--- Dyma sut ddylai dy gôd edrych: 

Paid anghofio bod angen i'r côd yma fod o fewn dolen `am byth`{:class="block3control"}. \--- /hint \--- \--- /hints \--- \--- /task \---

\--- /hint \--- \--- hint \---

Dyma'r blociau côd rwyt ti eu hangen:

![corlun-cwch changed](images/boat_resize.png)

```blocks3
dweud [HWRE!] am (2) eiliad

os <cyffwrdd lliw [#FFFF99] ?> yna
end

aros [y cyfan v]

```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![corlun-cwch](images/boat_resize.png)

```blocks3
os <cyffwrdd lliw [#FFFF99] ?> yna 
  dweud [HWRE!] am (2) eiliad
  aros [y cyfan v]
end
```

Don't forget that this new code needs to be inside the `forever`{:class="block3control"} loop.

\--- /hint \--- \--- /hints \--- \--- /task \---