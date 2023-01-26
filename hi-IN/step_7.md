## टाइमर जोड़ना

अब आप अपने खेल में एक टाइमर जोड़ेंगे, जिससे खिलाड़ी को जल्द से जल्द द्वीप पर पहुंचना होगा।

\--- task \---

`time`{:class="block3variables"} नामक एक नया वेरिएबल अपने स्टेज में जोड़ें |

![स्क्रीनशॉट](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

आप अपने नए वेरिएबल के प्रदर्शित होने के तरीके को बदलकर अपने टाइमर के लिए एक लुक भी चुन सकते हैं।

\--- /task \---

\--- task \---

अब अपने स्टेज में कोड ब्लॉक्स जोड़ें ताकि टाइमर की गिनती तब तक हो जब तक नाव द्वीप पर न पहुंच जाए।

\--- hints \--- \--- hint \---

स्टेज पर, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}। अपने `forever`{:class="block3control"} लूप के अंदर आपको पहले `wait 0.1 secs`{:class="block3control"}, फिर `change the time by 0.1`{:class="block3variables"}।

\--- /hint \--- \--- hint \---

आपको इन कोड ब्लॉक्स की ज़रुरत पड़ेगी:

![स्टेज](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

\--- /hint \--- \--- hint \---

आपका नया कोड कुछ ऐसा दिखना चाहिए:

![स्टेज](images/stage.png)

```blocks3
when flag clicked
set [time v] to [0]
forever
wait (0.1) seconds
change [time v] by (0.1)
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

अपने खेल का परीक्षण करें और देखें कि आप कितनी जल्दी नाव को द्वीप तक पहुंचा सकते हैं!

![स्क्रीनशॉट](images/boat-variable-test.png)

\--- /task \---