## Ras yn erbyn amser

Fe awn ati i ychwanegu cloc i dy gêm i annog y chwareuwr i gyrraedd yr ynys mor gyflym â phosib.

+ Ychwanega newidyn newydd o'r enw `amser`{:class="blockdata"} i dy lwyfan. Mae modd i ti hefyd newid sut mae dy newidyn newydd yn edrych. Os wyt ti eisiau cymorth, edrycha ar y prosiect 'Ghostbusters'.
    
    ![screenshot](images/boat-variable.png)

+ Ychwanega'r côd yma i dy **lwyfan**, fel fod y cloc yn cyfrif nes bod y cwch yn cyrraedd yr ynys:
    
    ```blocks
        pan fo ⚑ wedi ei glicio
        gosod [amser v] i [0]
        am byth
        aros (0.1) eiliad
        newid [amser v] gan (0.1)
        end
    ```

+ Dyna fe! Profa dy gêm i weld pa mor gyflym alli di gyrraedd yr ynys!
    
    ![screenshot](images/boat-variable-test.png)