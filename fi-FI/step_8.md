## Esteet ja lisävoimat

Tällä hetkellä tämä peli on **aivan** liian helppo, joten sinä lisäät asioita, jotta se olisi mielenkiintoisempi.

Ensin, sinä lisäät lisävoimia nopeuttaaksesi venettä.

--- task ---

Muokkaa Esiintymislavasi taustaa lisäämällä valkoisia lisävoima nuolia.

![kuvakaappaus](images/boat-boost.png)

--- /task ---

--- task ---

Lisää nyt lisää koodilohkoja veneen `ikuisesti`{:class="block3control"} silmukkaan niin, että vene siirtyy kolme ylimääräistä askelta, kun se koskettaa valkoista nuolta.

![vene-hahmo](images/boat_resize.png)

```blocks3
jos <touching color [#FFFFFF] ?> , niin 
  liiku (3) askelta
end
```

--- /task ---

--- task ---

Testaa peliäsi nähdäksesi, onko uudet lisävoima nuolet nopeuttaneet venettä.

--- /task ---

Seuraavaksi lisätään pyörivä portti, jota veneen on vältettävä.

--- task ---

Lisää uusi hahmo, joka näyttää tältä, ja anna sille nimeksi 'portti':

![kuvakaappaus](images/boat-gate.png)

Varmista, että portin väri on sama kuin puisten esteiden väri.

![kuvakaappaus](images/brown-hsv.png)

--- /task ---

--- task ---

Varmista, että portin keskipiste on sijoitettu keskelle.

![kuvakaappaus](images/boat-center.png)

--- /task ---

--- task ---

Lisää koodia porttiisi, jotta se pyörii hitaasti ikuisesti.

--- hints --- --- hint ---

Lisää koodilohkoja porttiin niin, että se `kääntyy 1 asteen`{:class="block3motion"} `ikuisesti`{:class="block3control"}.

--- /hint --- --- hint ---

Tässä on tarvitsemasi koodilohkot:

![portti](images/gate.png)

```blocks3
ikuisesti
end

käänny ↻ (1) astetta

kun klikataan ⚑
```

--- /hint --- --- hint ---

Uuden koodisi tulisi näyttää seuraavalta:

![portti](images/gate.png)

```blocks3
kun klikataan ⚑
ikuisesti 
  käänny ↻ (1) astetta
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

Testaa peli uudelleen. Sinulla pitäisi nyt olla pyörivä portti, jonka ympäri sinun täytyy ohjata veneesi.

![kuvakaappaus](images/boat-gate-test.png)

--- /task ---