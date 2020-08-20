## Kazanan!

--- task ---

Şimdi teknenizin görüntüsünün koduna başka bir `eğer`{:class="block3control"} ifadesi ekleyin. Böylelikle oyuncular teknelerini sarı adaya getirdiklerinde oyunu kazanır.

Tekne adaya ulaştığında, oyunda 'EVET!' ifadesi belirecek ve sonra da bitecektir.

--- hints ---
 --- hint ---

`Sonsuz`{:class="block3control"} döngünüzün içine daha fazla kod bloğu eklemeniz gerekir; böylece kodunuz, oyuncunun kazanıp kazanmadığını kontrol etmeye devam eder:

`Eğer`{:class="block3control"} tekne, adanın rengine `değiyorsa`{:class="block3sensing"}, `2 saniyeliğine 'EVET!' demelisiniz.`{:class="block3looks"} ardından oyunu durdurmak için `tümünü durdur`{:class="block3control"} deyin.

--- /hint --- --- hint ---

İhtiyacınız olan kod blokları:

![tekne-kuklası](images/boat_resize.png)

```blocks3
say [EVET!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

--- /hint --- --- hint ---

Yeni kodunuz şöyle görünmelidir:

![tekne-kuklası](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [EVET!] for (2) seconds
stop [all v]
end
```

Bu yeni kodunuzun `sonsuz`{:class="block3control"} döngünüzün içinde olması gerektiğini unutmayın.

--- /hint ------ /hints --- --- /task ---