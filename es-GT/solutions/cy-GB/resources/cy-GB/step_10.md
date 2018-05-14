\--- challenge \---

## Her: Mwy o gychod!

Wyt ti'n gallu troi dy gêm yn ras rhwng 2 chwareuwr?

+ Dyblyga'r cwch, ac ail-enwa fe'n 'Chwareuwr 2' a newid ei liw.

![screenshot](images/boat-p2.png)

+ Newida safle cychwyn Chwareuwr 2, wrth newid y côd yma:

```blocks
    mynd i x:(-190) y:(-150)
```

+ Dileua'r côd sydd yn defnyddio'r llygoden i reoli'r cwch:

```blocks
    os <(pellter at [pwyntydd llygoden v]) > [5]> wedyn
        pwyntio tuag at [pwyntydd llygoden v]
        symud (1) cam
    end
```

...a'i ailosod gyda côd sydd yn rheoli'r cwch yn defnyddio'r arwyddion ar y bysellfwrdd.

Dyma'r côd fydd angen arno ti i symud dy gwch ymlaen:

```blocks
    os <bysell [saeth i fyny v] wedi ei wasgu?> wedyn
   symud (1) cam
    end
```

Bydd hefyd angen i dy gôd `droi`{:class="blockmotion"} y cwch pan mae'r arwydd dde a chwith ar y bysellfwrdd wedi ei gwasgu.

\--- /challenge \---