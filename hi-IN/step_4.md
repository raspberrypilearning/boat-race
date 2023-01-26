## टकरा जाना!

फिलहाल, नाव स्प्राइट केवल लकड़ी के अवरोधों से होकर जा सकता है! आप इसे अभी ठीक करने जा रहे हैं।

\--- task \---

आपको अपनी नाव स्प्राइट के लिए दो पोशाकों की आवश्यकता होगी, एक साधारण पोशाक, और दूसरी उस समय के लिए जब नाव टकरा जाती है। अपनी नाव स्प्राइट की पोशाक की कॉपी बनाएं, और एक को 'normal' नाम दें और दूसरे को 'hit' नाम दें।

\--- /task \---

\--- task \---

अपनी 'hit' पोशाक पर क्लिक करें, और पोशाक के **Select** टूल का उपयोग करें और नाव को ऐसा बनाने के लिए घुमाएँ और घुमाएँ जैसे कि यह टुकड़ों में दुर्घटनाग्रस्त हो गई है।

![स्क्रीनशॉट](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

अब अपनी नाव में कोड जोड़ें ताकि यह किसी भी भूरी लकड़ी के टुकड़े से टकराने पर दुर्घटनाग्रस्त हो जाए और टूट जाए।

\--- hints \--- \--- hint \---

आपको अपने `forever`{:class="block3control"} लूप के अंदर कोड ब्लॉक जोड़ने की जरूरत है ताकि आपका कोड जांचता रहे कि क्या नाव स्प्राइट दुर्घटनाग्रस्त हो गई है, और यदि यह दुर्घटनाग्रस्त हो गई है, तो कोड को नाव स्प्राइट की स्थिति को रीसेट करने की आवश्यकता है।

`if`{:class="block3control"} नाव `touching`{:class="block3sensing"} लकड़ी का भूरा रंग, आपको हिट पोशाक के लिए `switch to the hit costume`{:class="block3looks"}, `Noooo<0> कहते हैं! for 2 seconds`{:class="block3looks"}, और फिर `switch back to the normal costume`{:class="block3looks"} | अंत में, आपको `point up`{:class="block3motion" और `go to the start position`{:class="block3motion"} |

\--- /hint \--- \--- hint \---

आपको इन कोड ब्लॉक्स की ज़रुरत पड़ेगी:

![नाव स्प्राइट](images/boat_resize.png)

```blocks3
if <touching color [ ] ?> then
end

go to x: (-190) y: (-150)

switch costume to (hit v)

point in direction (0)

switch costume to (normal v)

say [Noooooo!] for (2) seconds
```

\--- /hint \--- \--- hint \---

आपका कोड ऐसा दिखना चाहिए:

![नाव स्प्राइट](images/boat_resize.png)

```blocks3
when flag clicked
point in direction (0)
go to x: (-190) y: (-150)
forever
if <(distance to (mouse-pointer v)) > [5]> then
point towards (mouse-pointer v)
move (1) steps
end
if <touching color [#663b00] ?> then
switch costume to (hit v)
say [Noooooo!] for (2) seconds
switch costume to (normal v)
point in direction (0)
go to x: (-190) y: (-150)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

आपको यह सुनिश्चित करने के लिए कोड भी जोड़ना चाहिए कि आपकी नाव स्प्राइट हमेशा 'normal' स्तिथि में शुरू हो।

अपने कोड का फिर से परीक्षण करें। यदि आप अब लकड़ी की बाधा से नाव को पार करने की कोशिश करते हैं, तो नाव दुर्घटनाग्रस्त हो जानी चाहिए और फिर वापस अपनी प्रारंभिक स्थिति में आ जानी चाहिए।

![स्क्रीनशॉट](images/boat-crash.png)

\--- /task \---