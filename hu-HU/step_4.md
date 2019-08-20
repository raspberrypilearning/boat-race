## Ütközés!

Jelenleg a hajó szereplő egyszerűen átmegy a fa akadályokon! Ezt most meg fogod javítani.

--- task ---

Két jelmezre van szükséged a hajó szereplőhöz: egy normál jelmezre, és egyre, amelyet a hajó ütközése után használunk. Másold le a hajó szereplőd jelmezét, majd az egyik jelmeznek add a "normál", a másiknak a "törött" nevet.

--- /task ---

--- task ---

Kattints a "törött" jelmezre, majd a **Kijelölés** eszközzel ragadj meg darabokat a jelmezből, mozgasd és forgasd el őket, hogy úgy nézzen ki, mintha a hajó darabokra törött volna.

![képernyőkép](images/boat-hit-costume-annotated.png)

--- /task ---

--- task ---

Most adj hozzá kódot a hajódhoz, hogy ütközzön és széttörjön, ha hozzáér bármilyen barna fa akadályhoz.

--- hints ---
 --- hint --- Kódblokkokat kell hozzáadnod a `mindig`{: class = "block3control"} ciklushoz úgy, hogy a kódod folyamatosan ellenőrizze, hogy a hajó szereplő ütközött-e, és ha ütközött, a kódnak vissza kell állítania a hajó szereplő pozícióját.

`ha`{:class="block3control"} a hajó `érinti`{:class="block3sensing"} a fa barna színét, át kell változtatnod a `törött jelmezre`{:class="block3looks"}, és azt `mondani, hogy Neeeeee! 2 másodpercig`{:class="block3looks"}, majd `visszaváltani a normál jelmezre`{:class="block3looks"}. Végül `felfelé kell mutatni`{:class="block3motion"} és `visszamenni a kezdő helyre`{:class="block3motion"}.

--- /hint --- --- hint --- Íme a szükséges kódblokkok: ![hajó szereplő](images/boat_resize.png)

```blocks3
ha <touching color [ ] ?> akkor
end

ugorj ide: x: (-190) y: (-150)

jelmez legyen (törött v)

nézz (0) fokos irányba

jelmez legyen (normál v)

mondd: [Neeeeee!] (2) másodpercig
```

--- /hint --- --- hint --- Így kell kinéznie a kódodnak: ![hajó szereplő](images/boat_resize.png)

```blocks3
⚑ -ra kattintáskor
nézz (0) fokos irányba
ugorj ide: x: (-190) y: (-150)
mindig 
 ha <((egérmutató v) távolsága) > [5]> akkor 
 nézz (egérmutató v) felé
 menj (1) lépést
 end
 ha <touching color [#663b00] ?> akkor 
 jelmez legyen (törött v)
 mondd: [Neeeeee!] (2) másodpercig
 jelmez legyen (normál v)
 nézz (0) fokos irányba
 ugorj ide: x: (-190) y: (-150)
 end
end
```

--- /hint ------ /hints ---

--- /task ---

--- task ---

Ahhoz is hozzá kell adnod a kódot, hogy a hajó kezdéskor mindig "normál" kinézetű legyen.

Teszteld újra a kódodat. Ha most megpróbálsz keresztülhajózni egy fa akadályon, a hajónak össze kell törnie, majd visszaugrania a kezdőhelyre.

![képernyőkép](images/boat-crash.png)

--- /task ---