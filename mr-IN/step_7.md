## एक टाइमर जोडत आहे

आता आपण आपल्या गेममध्ये एक टाइमर जोडू शकता जेणेकरून खेळाडूला शक्य तितक्या लवकर बेटाकडे जाणे आवश्यक आहे.

\--- कार्य \---

आपल्या स्टेजवर `वेळ`{: class = "block3variables"} नावाचे एक नवीन चलन जोडा.

![स्क्रीनशॉट](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

आपण आपले नवीन व्हेरिएबल कसे प्रदर्शित केले आहे ते बदलून आपल्या टायमरची एक नक्कल निवडू शकता.

\--- / कार्य \---

\--- कार्य \---

आता आपल्या स्टेजवर कोड अवरोध जोडा जेणेकरून बेटी बेटावर पोचते तोपर्यंत टाइमर मोजा.

\--- hints \--- \--- hint \---

On the Stage, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}. Inside your `forever`{:class="block3control"} loop, you'll need to first `wait 0.1 secs`{:class="block3control"}, then `change the time by 0.1`{:class="block3variables"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you'll need:

![stage](images/stage.png)

```blocks3
बदला [वेळ v] by (0.1)

जेव्हा ध्वज

कायमचे क्लिक केले
अंत

प्रतीक्षा (0.1) सेकंद

सेट [वेळ v] ते [0]
```

\--- /hint \--- \--- hint \---

Here's what your new code should look like:

![stage](images/stage.png)

```blocks3
ध्वज
सेट [वेळ व्ही] ते [0]
क्लिक केले
प्रतिक्षा (0.1) सेकंद
बदल [वेळ व्ही] द्वारे (0.1)
समाप्ती
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test out your game and see how quickly you can get the boat to the island!

![screenshot](images/boat-variable-test.png)

\--- /task \---