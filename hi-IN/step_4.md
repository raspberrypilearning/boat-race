## दुर्घटनाग्रस्त होना!

फिलहाल, नाव sprite बस लकड़ी की बाधाओं के माध्यम से रवाना हो सकती है! अब आप इसे ठीक करने जा रहे हैं।

\--- task \---

आपको अपनी नाव के लिए दो पोशाक की आवश्यकता होगी, एक साधारण पोशाक, और दूसरी उस समय के लिए जब नाव की टक्कर हो जाती है। अपनी नाव की पोशाक की प्रतिलिपि(duplicate) बनाएं, और एक को 'normal' नाम दें और दूसरे को 'hit' नाम दें।

\--- /task \---

\--- task \---

अपनी 'hit' पोशाक पर क्लिक करें, और **Select** पोशाक के टुकड़ों को पकड़ने और नाव को मोड़ने के लिए उन्हें घुमाएं और घुमाएं जैसे कि यह टुकड़ों में दुर्घटनाग्रस्त हो गया है।

![स्क्रीनशॉट](images/boat-hit-costume-annotated.png)

\--- /task \---

\--- task \---

अब अपनी नाव में कोड जोड़ें ताकि यह किसी भी भूरी(brown) लकड़ी के टुकड़े से टकराने पर दुर्घटनाग्रस्त हो जाए और टूट जाए।

\--- hints \--- \--- hint \---

आपको अपने `forever`{"class="block3control"} लूप ताकि आपका कोड यह जाँचता रहे कि क्या नाव sprite दुर्घटनाग्रस्त हो गई है, और यदि यह दुर्घटनाग्रस्त हो गई, तो कोड को नाव sprite की स्थिति को रीसेट करने की आवश्यकता है।

`if`{:class="block3control"} नाव `touching`{:class="block3sensing"} लकड़ी का भूरा रंग, आपको हिट पोशाक के लिए `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, और फिर `switch back to the normal costume`{:class="block3looks"} | अंत में, आपको `point up`{:class="block3motion" और `go to the start position`{:class="block3motion"} |

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

आपको यह भी सुनिश्चित करना होगा कि आपकी नाव हमेशा 'सामान्य(normal)' स्थिति में स्टार्ट हो।

फिर से अपने कोड का परीक्षण करें। यदि आप नाव को लकड़ी की बाधा से पार करने की कोशिश करते हैं, तो नाव दुर्घटनाग्रस्त हो जाती है और फिर वापस अपनी प्रारंभिक स्थिति में आ जाती है।

![स्क्रीनशॉट](images/boat-crash.png)

\--- /task \---