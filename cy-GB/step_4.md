## Llongddrylliad!

Mae dy gwch dal yn gallu hwylio trwy'r pren! Fe wnawn ni drwsio hyn.

+ Fe fydd angen 2 wisg ar dy gwch, un normal, ac un ar gyfer pan mae'r cwch yn taro'r pren.  Dyblyga gwisg y cwch, a galw nhw yn 'normal' a 'wedi torri'

+ Clicia ar dy wisg 'wedi torri', a dewis y teclyn 'Dewis' i ddewis darnau o'r cwch a symud a'u cylchdroi nhw.  Gwna'r cwch i edrych fel ei fod wedi bod mewn llongddrylliad.

	![screenshot](images/boat-hit-costume.png)

+ Ychwanega'r côd yma i dy gwch, yn y ddolen `am byth`{:class="blockcontrol#2}, fel ei fod yn torri pan mae'n cyffwrdd y darnau pren:

	```blocks
		os <cyffwrdd lliw [#603C15]?> wedyn
   		newid i wisg [wedi torri v]
   		dweud [Naaaa!] am (1) eiliad
   		newid i wisg [normal v]
   		pwyntio i gyfeiriad (0 v)
   		mynd i x:(-215) y:(-160)
		end
	```

Mae'r côd yma yn y ddolen `am byth`{:class="blockcontrol"}, fel bod dy gôd yn cadw gwirio os yw'r cwch wedi taro yn erbyn y pren.

+ Fe ddylet ti wneud yn siwr bod dy gwch bob tro yn dechrau'r gêm yn edrych yn 'normal'.

+ Nawr os wyt ti'n hwylio trwy'r pren, fe ddylet ti weld bod dy gwch yn torri ac yn symud nol i'r dechrau.

	![screenshot](images/boat-crash.png)
