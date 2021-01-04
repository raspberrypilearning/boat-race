## ಗೆಲ್ಲುವ ವಿಧಾನ!

--- task ---

ಈಗ ಮತ್ತೊಂದು `if`{:class="block3control"} ನಿಮ್ಮ ದೋಣಿ sprite ಇ‌ನ ಕೋಡ್‌ಗೆ ಸೇರಿಸಿದರಿಂದ ದೋಣಿ ಹಳದಿ ದ್ವೀಪಕ್ಕೆ ಬರುವಂತೆ ಮಾಡಿ ಆಟಗಾರರನ್ನು ಗೆಲ್ಲುವುದಕ್ಕೆ ಸಾಧ್ಯವಾಗುತ್ತದೆ.

ದೋಣಿ ದ್ವೀಪಕ್ಕೆ ಬಂದಾಗ, ಆಟವು 'YEAH!' ಎಂದು ಹೇಳಬೇಕು, ಮತ್ತು ನಂತರ ಅದು ಕೊನೆಗೊಳ್ಳಬೇಕು.

--- hints ---
 --- hint ---

ಹೆಚ್ಚಿನ `forever`{:class="block3control"}ಕೋಡ್ ಬ್ಲಾಕ್ಗಳ ‌ಲೂಪ್ ಅನ್ನು ನೀವು ಶಾಶ್ವತವಾಗಿ ಸೇರಿಸುವ ಅಗತ್ಯವಿದೆ, ಅದರಿಂದ ಆಟಗಾರನು ಗೆದ್ದಿದ್ದಾನೆಯೇ ಎಂದು ನಿಮ್ಮ ಕೋಡ್ ಪರಿಶೀಲಿಸುತ್ತದೆ:

`if`{:class="block3control"} ದೋಣಿ `touching`{:class="block3sensing"} ದ್ವೀಪದ ಕಂದು ಬಣ್ಣ ಕಾಣುತ್ತಿದ್ದರೆ, ನೀವು `say 'YEAH!' for 2 seconds`{:class="block3looks"} ಮತ್ತು `stop all`{:class="block3control"} ಎಂದು ಆಟ ನಿಲ್ಲಿಸಲು ಹೇಳಿ.

--- /hint --- --- hint ---

ನಿಮಗೆ ಅಗತ್ಯವಿರುವ ಕೋಡ್ ಬ್ಲಾಕ್‌ಗಳು ಇಲ್ಲಿವೆ:

![ದೋಣಿ -sprite](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

--- /hint --- --- hint ---

ನಿಮ್ಮ ಹೊಸ ಕೋಡ್ ಹೀಗಿರಬೇಕು:

![ದೋಣಿ-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

ಈ ಹೊಸ ಕೋಡ್ `forever`{:class="block3control"} ಲೂಪ್ ಒಳಗೆ ಇರಬೇಕು ಎಂಬುದನ್ನು ಮರೆಯಬೇಡಿ.

--- /hint ------ /hints --- --- /task ---