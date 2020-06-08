## टाइमर(timer) जोड़ना

अब आप अपने खेल में एक टाइमर जोड़ देंगे, ताकि खिलाड़ी को जल्द से जल्द द्वीप पर जाना पड़े।

--- task ---

`time`{:class="block3variables"} नामक एक नया वेरिएबल (variable) अपने प्रोजेक्ट में जोड़ें ।

![स्क्रीनशॉट](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

आप अपने टाइमर के लिए अपने नए चर को प्रदर्शित करने का तरीका बदल कर भी चुन सकते हैं।

--- /task ---

--- task ---

अब अपने स्टेज में कोड जोड़ें ताकि टाइमर नाव के रेगिस्तानीय द्वीप पर पहुँच जाने तक समय गिनता रहे।

--- hints ---
 --- hint ---

स्टेज पर, `when the green flag is clicked`{:class="block3control"}, `set the time to 0`{:class="block3variables"}। अपने `forever`{:class="block3control"} लूप के अंदर आपको पहले `wait 0.1 secs`{:class="block3control"}, फिर `change the time by 0.1`{:class="block3variables"}।

--- /hint --- --- hint ---

आपको इस कोड ब्लॉक की ज़रुरत पड़ेगी:

![मंच](images/stage.png)

```blocks3
change [time v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [time v] to [0]
```

--- /hint --- --- hint ---

आपका नया कोड कुछ ऐसा दिखना चाहिए:

![मंच](images/stage.png)

```blocks3
when flag clicked
set [time v] to [0]
forever
wait (0.1) seconds
change [time v] by (0.1)
end
```

--- /hint ------ /hints ---

--- /task ---

--- task ---

बस इतना ही! अपनी गेम का परीक्षण करें और देखें कि आप कितनी जल्द रेगिस्तान नाव को द्वीप पर पहुंचा सकते हैं!

![स्क्रीनशॉट](images/boat-variable-test.png)

--- /task ---