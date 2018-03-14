## Ovládání lodi

+ Loď budeš ovládat myší. Přidej k lodi vlastní kód tak, aby startovala z levého dolního rohu, směřovala nahoru a následovala ukazatel myši. **Otestuj svůj kód** aby ses ujistil, že dělá to, co má.

\--- hints \--- \--- hint \--- `Po kliknutí na zelený praporek`, by loď měla `skočit na výchozí pozici` a `nastavit směr` přídí vzhůru. Dále se musí `natočit k ukazateli myši` a přesunout se `dopředu o 1 krok`. Tyto kroky by měla opakovat `stále`.

\--- /hint \--- \--- hint \--- Zde jsou bloky, které budeš potřebovat: ![screenshot](images/boat-move-blocks.png) \--- /hint \--- \--- hint \--- Takto by měl vypadat tvůj kód: ![screenshot](images/boat-move-code.png) \--- /hint \--- \--- /hints \---

+ Otestuj svou loď kliknutím na zelený praporek a pohybuj myší. Pohybuje se loď směrem k myši?
    
    ![screenshot](images/boat-mouse.png)
    
    ![screenshot](images/boat-pointer-test-anim.gif)

## \--- collapse \---

title: Pokud máš problémy ...

## image: images/image.png

**Poznámka:** V současné době je v aplikaci Scratch chyba, může se stát, že se tvoje loď nemusí pohybovat směrem k ukazateli myši. Pokud k tomu dojde, klikni na šipku v bloku `natoč se k` a znovu vyber `ukazatel myši`.

![screenshot](images/boat-bug.png) \--- /collapse \---

+ Co se stane, když loď dosáhne ukazatelem myši? Zkus to.

+ Chceš-li této situaci zabránit, musíš ke kódu přidat blok `když` tak, aby se člun pohyboval pouze v případě, že je více než 5 pixelů od myši.

\--- hints \--- \--- hint \--- Loď by se měla pohybovat a orientovat se, jen tehdy, `když` je dále `než 5 pixelů` od `ukazatele myši.`. \--- /hint \--- \--- hint \--- Zde jsou bloky, které potřebuješ přidat ke kódu lodi: ![screenshot](images/boat-pointer-blocks.png) \--- /hint \--- \--- hint \--- Takto by měl vypadat tvůj kód: ![screenshot](images/boat-pointer-code.png) \--- /hint \--- \--- /hints \---

+ Otestuj znovu svou loď, abys zkontroloval, zda byl problém vyřešen.