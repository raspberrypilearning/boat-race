## Krahh!

Praegu saab paadi purjus lihtsalt läbi puidust tõkete! Sa hakkad selle kohe lahendama.

\--- ülesanne \---

Sa pead oma paadi jaoks olema kaks kostüümi: üks tavaline kostüüm ja teine paadi jooksmisel. Dubleerige oma paadisõidu kostüüm ja nimetage üks kostüüm „normaalne“ ja teine „löögi”.

\--- / ülesanne \---

\--- ülesanne \---

Klõpsa oma "hit" kostüümile ja kasuta **Select** tööriista, et haarata kostüümi tükid ja liikuda ja pöörata, et paat näeks välja nagu see on kokku kukkunud.

![ekraanipilt](images/boat-hit-costume-annotated.png)

\--- / ülesanne \---

\--- ülesanne \---

Nüüd lisage oma paadile kood nii, et see jookseb kokku ja puruneb, kui see puudutab pruuni puidust tõkkeid.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
kui <touching color [ ] ?> siis
ots

minge x: (-190) y: (-150)

lüliti kostüüm (löögi v)

punkti suunas (0)

lüliti kostüüm (tavaline v)

ütle [Noooooo!] (2) sekundit
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
kui lipp klõpsas
punkti suunas (0)
minge x: (-190) y: (-150)
igavesti
kui <(kaugus (hiirekursor v)) > [5]> siis
punkti (hiir- pointer v)
liikuda (1) sammud
lõpp
kui <touching color [#663b00] ?> siis
lüliti kostüümi (löö v)
öelda [Noooooo!] (2) sekundit
lüliti kostüüm (tavaline v)
punkti suunas (0)
punkti suunas (0) 
 minge x: (-190) y: (-150)
lõppu
```

\--- /hint \--- \--- /hints \---

\--- / ülesanne \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---