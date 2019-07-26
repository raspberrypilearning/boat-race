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

\--- hints \--- \--- hint \--- Ar y llwyfan `pan fo'r faner werdd wedi ei chlicio`{:class="block3control"}, `gosod yr amser i 0`{:class="block3variables"}. O fewn dy ddolen `am byth`{:class="block3control"} bydd angen i ti yn gyntaf`aros 0.1 eiliad`{:class="block3control"}, yna `newid yr amser wrth 0.1`{:class="block3variables"}. \--- /hint \--- \--- hint \--- Dyma'r blociau côd rwyt ti eu hangen: ![llwyfan](images/stage.png)

```blocks3
newid [amser v] gan (0.1)

pan fo'r flag werdd yn cael ei glicio

am byth
end

aros (0.1) eiliad

gosod [amser v] i [0]
```

\--- /hint \--- \--- hint \--- Dyma sut ddylai dy gôd edrych: ![llwyfan](images/stage.png)

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

Profa dy gêm i weld pa mor gyflym alli di gael y cwch i'r ynys!

![sgrinlun](images/boat-variable-test.png)

\--- /task \---