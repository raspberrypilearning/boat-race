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

**Poznámka:** V současné době je v aplikaci Scratch chyba, může se stát, že se tvoje loď nemusí pohybovat směrem k ukazateli myši. If this happens, click the arrow on the `point towards` block and re-select `mouse-pointer`.

![screenshot](images/boat-bug.png) \--- /collapse \---

+ What happens if the boat reaches the mouse pointer? Try it.

+ To stop this from happening, you'll need to add an `if` block to your code, so that the boat only moves if it is more than 5 pixels away from the mouse.

\--- hints \--- \--- hint \--- The boat should only point towards the mouse pointer and move `if` the `distance to the mouse pointer` is `greater than 5 pixels`. \--- /hint \--- \--- hint \--- Here are the code blocks you'll need to add to the code for the boat: ![screenshot](images/boat-pointer-blocks.png) \--- /hint \--- \--- hint \--- This is what your code should look like: ![screenshot](images/boat-pointer-code.png) \--- /hint \--- \--- /hints \---

+ Test out your boat again to check whether the problem has been fixed.