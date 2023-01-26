## जीतना!

\--- task \---

अब एक और `if`{:class="block3control"} स्टेटमेंट को अपनी नाव स्प्राइट कोड में जोड़ें ताकि खिलाड़ी जब बोट को पीले द्वीप पर पहुंचाए तो जीत जाए।

जब नाव द्वीप पर पहुँचती है, तो खेल को 'YEAH!' कहना चाहिए, और फिर इसे समाप्त हो जाना चाहिए।

\--- hints \--- \--- hint \---

आपको अपने `forever`{:class="block3control"} लूप के अंदर और कोड ब्लॉक्स जोड़ने होंगे ताकि आपका कोड यह जांचता रहे कि क्या खिलाड़ी जीता है:

`if`{:class="block3control"} नाव `touching`{:class="block3sensing"} है, तो आपको `say 'YEAH!' for 2 seconds`{:class="block3looks"} जोड़ना होगा और फिर गेम समाप्त करने के लिए `stop all`{:class="block3control"} जोड़ना होगा।

\--- /hint \--- \--- hint \---

आपको इन कोड ब्लॉक्स की ज़रुरत पड़ेगी:

![नाव स्प्राइट](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \---

आपका नया कोड कुछ ऐसा दिखना चाहिए:

![नाव स्प्राइट](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

यह न भूलें कि यह नया कोड `forever`{:class="block3control"} लूप के अंदर होना चाहिए।

\--- /hint \--- \--- /hints \--- \--- /task \---