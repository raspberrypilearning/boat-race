## Ychwanegu Amserydd

Fe awn ati i ychwanegu cloc i dy gêm i annog y chwareuwr i gyrraedd yr ynys mor gyflym â phosib.

\--- task \---

Ychwanega newidyn newydd o’r enw `amser`{:class="block3variables"} i dy Lwyfan.

![sgrinlun](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Mae modd i ti hefyd newid sut mae dy newidyn newydd yn edrych.

\--- /task \---

\--- task \---

Ychwanega blociau côd i dy lwyfan, fel fod y cloc yn cyfrif fyny nes bod y cwch yn cyrraedd yr ynys.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
newid [amser v] gan (0.1)

pan fo'r flag werdd yn cael ei glicio

am byth
end

aros (0.1) eiliad

gosod [amser v] i [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
gosod [amser v] i [0]
am byth 
  aros (0.1) eiliad
  newid [amser v] gan (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---