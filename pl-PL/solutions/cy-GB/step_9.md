--- challenge ---

## Her: Mwy o rwystrau! 
Alli di ychwanegu mwy o rwystrau i dy gêm? Dyma rai syniadau:

+ Fe alli di ychwanegu sleim gwyrdd i'r cefndir, sydd yn arafu'r chwareuwr pan mae'n nhw'n ei gyffwrdd. Fe alli di ddefnyddio'r bloc `aros`{:class="blockcontrol"} i wneud hyn:

```blocks
	aros (0.01) eiliad
````

![screenshot](images/boat-algae.png)

+ Fe alli di ychwanegu rhywbeth sy'n symud, fel gangen pren neu siarc!

![screenshot](images/boat-obstacles.png)

Fe all y blociau yma dy helpu:

```blocks
	symud (1) cam
		os ar ymyl, bowndio

````

Os nad yw dy wrthrych newydd yn frown, bydd angen i ti ychwanegu'r côd yma i dy gwch:

```blocks
	os <<cyffwrdd lliw [#603C15]?> neu <cyffwrdd [sharc v]?>> wedyn
		end
```

--- /challenge ---
