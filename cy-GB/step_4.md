## Llongddrylliad!

Mae dy gwch dal yn gallu hwylio trwy’r pren! Fe wnawn ni drwsio hyn.

\--- task \---

Fe fydd angen 2 wisg ar dy gwch, un normal, ac un ar gyfer pan mae’r cwch yn taro’r pren. Dyblyga gwisg y cwch, a galw nhw yn ‘normal’ a ‘wedi torri’.

\--- /task \---

\--- task \---

Clicia ar dy wisg ‘wedi torri’, a dewis y teclyn **Dewis** i ddewis darnau o’r cwch a symud a’u cylchdroi nhw. Gwna’r cwch i edrych fel ei fod wedi bod mewn llongddrylliad.

![sgrinlun](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

Ychwanega gôd i dy gwch fel ei fod yn torri pan mae’n cyffwrdd y darnau pren.

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
os <cyffwrdd lliw [ ] ?> yna
end

mynd i x: (-190) y: (-150)

newid gwisg i (hit v)

pwyntio i gyfeiriad (0)

newid gwisg i (normal v)

dweud [Naaa!] am (2) eiliad
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
pwyntio i gyfeiriad (0)
mynd i x: (-190) y: (-150)
am byth 
  os <(pellter i (pwyntydd llygoden v)) > [5]> yna 
    pwyntio tuag at (pwyntydd llygoden v)
    symud (1) cam
  end
  os <cyffwrdd lliw [#663b00] ?> yna 
    newid gwisg i (hit v)
    dweud [Naaa!] am (2) eiliad
    newid gwisg i (normal v)
    pwyntio i gyfeiriad (0)
    mynd i x: (-190) y: (-150)
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