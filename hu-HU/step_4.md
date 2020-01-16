## Ütközés!

Jelenleg a hajó szereplő egyszerűen átmegy a fa akadályokon! Ezt most meg fogod javítani.

\--- task \---

Két jelmezre van szükséged a hajó szereplőhöz: egy normál jelmezre, és egyre, amelyet a hajó ütközése után használunk. Másold le a hajó szereplőd jelmezét, majd az egyik jelmeznek add a "normál", a másiknak a "törött" nevet.

\--- /task \---

\--- task \---

Kattints a "törött" jelmezre, majd a **Kijelölés** eszközzel ragadj meg darabokat a jelmezből, mozgasd és forgasd el őket, hogy úgy nézzen ki, mintha a hajó darabokra törött volna.

![képernyőkép](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Most adj hozzá kódot a hajódhoz, hogy ütközzön és széttörjön, ha hozzáér bármilyen barna fa akadályhoz.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
ha <touching color [ ] ?> akkor
end

ugorj ide: x: (-190) y: (-150)

jelmez legyen (törött v)

nézz (0) fokos irányba

jelmez legyen (normál v)

mondd: [Neeeeee!] (2) másodpercig
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

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

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---