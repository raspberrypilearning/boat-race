## Rheoli'r cwch

Bydd y chwaraewr yn rheoli'r cwch gyda'r llygoden.

--- task --- Ychwanega gôd at dy gwch fel ei fod yn cychwyn o'r gornel chwith isaf gan bwyntio i fyny ac yna'n dilyn pwyntydd y llygoden.

![corlun-cwch](images/boat_resize.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
pwyntio i gyfeiriad (0)
mynd i x: (-190) y: (-150)
am byth 
  pwyntio tuag at (pwyntydd llygoden v)
  symud (1) cam
end
```

--- /task ---

--- task ---

**Profa dy gôd** drwy glicio ar y faner werdd a symud y llygoden. A yw'r cwch yn troi'n symud tuag at bwyntydd y llygoden?

![sgrinlun](images/boat-mouse.png)

--- no-print --- 
![screenshot](images/boat-pointer-test-anim.gif) 
--- /no-print ---

--- print-only --- 
![screenshot](images/boat-pointer-test-anim.png) 
--- /print-only ---

--- /task ---

--- task ---

Beth sy'n digwydd pan fydd y cwch yn cyrraedd pwyntydd y llygoden? Rho gynnig arni i weld beth yw'r broblem.

--- /task ---

--- task ---

I atal hyn rhag digwydd, mae angen ychwanegu bloc `os`{:class="block3control"} i'r côd, fel bod y cwch yn symud dim ond os yw'n fwy na 5 picsel i ffwrdd o bwyntydd y llygoden.

--- hints ---
 --- hint --- Fe ddylai'r cwch ddim ond pwyntio tuag at bwyntydd y llygoden a symud `os`{:class="block3control"} yw'r `pellter at y pwyntydd llygoden`{:class="block3sensing"} yn `fwy na 5 picsel`{:class="block3operators"}.
--- /hint ---
 --- hint --- Dyma'r blociau côd sydd angen arno ti i ychwanegu côd i'r cwch: ![corlun-cwch](images/boat_resize.png)

```blocks3
os < [ ] > [ ] > yna
end

(pellter i (pwyntydd llygoden v))
```

--- /hint --- --- hint --- Dyma sut dylai dy gôd edrych: ![corlun-cwch](images/boat_resize.png)

```blocks3
pan fo'r flag werdd yn cael ei glicio
pwyntio i gyfeiriad (0)
mynd i x: (-190) y: (-150)
am byth 
  os <(pellter i (pwyntydd llygoden v)) > [5]> yna 
    pwyntio tuag at (pwyntydd llygoden v)
    symud (1) cam
  end
end
```

--- /hint --- --- /hints ---

--- /task ---

--- task ---

Profa dy gôd eto i weld a yw'r broblem bellach wedi datrys.

--- /task ---