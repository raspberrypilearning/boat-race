## जीतना!

\--- task \---

अब एक और जोड़ें `if`{:class="block3control"}स्टेटमेंट जोड़ें ताकि खिलाड़ी जीत जाए जब वे नाव को पीले द्वीप पर पहुंचे।

जब नाव द्वीप पर पहुंच जाती है, तो खेल को 'YEAH!' कहना चाहिए, और फिर इसे समाप्त होना चाहिए।

\--- hints \--- \--- hint \---

आपको अपने `forever`{:class="block3control"} लूप के अंदर और कोड्स जोड़ने होंगे ताकि आपका कोड यह जांचता रहे कि क्या खिलाड़ी जीता है:

`if`{:class="block3control"} नाव द्वीप को `touching`{:class="block3sensing"} लेती है, तो आपको `say 'YEAH!' for 2 seconds`{:class="block3looks"} जोड़ना होगा और फिर गेम समाप्त करने के लिए `stop all`{:class="block3control"} जोड़ना होगा।

\--- /hint \--- \--- hint \---

आपको इस कोड ब्लॉक की ज़रुरत पड़ेगी:

![नाव sprite](images/boat_resize.png)

```blocks3
say [YEAH!] for (2) seconds

if <touching color [#FFFF99] ?> then
end

stop [all v]

```

\--- /hint \--- \--- hint \---

आपका कोड ऐसा दिखना चाहिए:

![नाव sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFF99] ?> then
say [YEAH!] for (2) seconds
stop [all v]
end
```

यह मत भूलो कि इस नए कोड को हमेशा के लिए `forever`{:class="block3control"} लूप के अंदर होना चाहिए।

\--- /hint \--- \--- /hints \--- \--- /task \---