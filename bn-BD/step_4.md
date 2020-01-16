## বিপর্যয়!

এ মুহূর্তে, নৌকোড়াটি কেবল কাঠের বাধা দিয়ে পালাতে পারে! আপনি এখন যে ঠিক করতে যাচ্ছি।

\--- কাজ \---

আপনি আপনার নৌকা স্প্রাইট জন্য দুটি পোশাক প্রয়োজন: একটি স্বাভাবিক পরিচ্ছদ, এবং নৌকা ক্র্যাশ জন্য এক। আপনার নৌকা স্প্রাইটের পোশাকটি নকল করুন, এবং একটি পোষাক 'স্বাভাবিক' নাম দিন এবং অন্যটি হিট করুন।

\--- /কাজ \---

\--- কাজ \---

আপনার 'হিট' পরিচ্ছদটিতে ক্লিক করুন এবং পরিচ্ছদ টুকরা টেনে আনতে **নির্বাচন করুন** টুল ব্যবহার করুন এবং নৌকাটি টুকরো টুকরো করে ক্র্যাশ করে তুলতে তাদেরকে ঘুরে ঘুরুন।

![screenshot](images/boat-hit-costume-annotated.png)

\--- /কাজ \---

\--- কাজ \---

এখন আপনার নৌকাতে কোড যুক্ত করুন যাতে এটি কোনও বাদামী কাঠের বাধাগুলি স্পর্শ করে ক্র্যাশ এবং বিরতি দেয়।

\--- hints \--- \--- hint \---

You need to add code blocks inside your `forever`{:class="block3control"} loop so that your code keeps checking if the boat sprite has crashed, and if it has crashed, the code needs to reset the boat sprite's position.

`if`{:class="block3control"} the boat is `touching`{:class="block3sensing"} the brown colour of the wood, you need to `switch to the hit costume`{:class="block3looks"}, `say Noooo! for 2 seconds`{:class="block3looks"}, and then `switch back to the normal costume`{:class="block3looks"}. Finally, you'll need to `point up`{:class="block3motion"} and `go to the start position`{:class="block3motion"}.

\--- /hint \--- \--- hint \---

Here are the code blocks you need:

![boat-sprite](images/boat_resize.png)

```blocks3
যদি <touching color [ ] ?> তারপর
শেষ

x তে যান: (-190) y: (-150)

সুইচ পরিচ্ছদ (হিট ভ) দিকের

পয়েন্টে (0)

সুইচ পরিচ্ছদ (স্বাভাবিক v)

বলুন [Noooooo!] এর জন্য (২ সেকেন্ড
```

\--- /hint \--- \--- hint \---

Here's what your code should look like:

![boat-sprite](images/boat_resize.png)

```blocks3
যখন পতাকা
পয়েন্টে 
 পয়েন্টে ক্লিক করে (0)
x তে যান (-190) y: (-150)
চিরতরে
হলে <(দূরত্ব (মাউস-পয়েন্টার v) থেকে) > [5]> তারপর
পয়েন্ট দিকে (মাউস- পয়েন্টার v)
পদক্ষেপ (1) পদক্ষেপ
শেষ
হলে <touching color [#663b00] ?>
পোষাকের পোশাক (হিট বনাম)
বলবে [Noooooo!] (2) সেকেন্ডে
সুইচ পরিচ্ছদ (স্বাভাবিক v) দিকের
পয়েন্টে (0)
এক্স এ যান: (-190) Y: (-150)
শেষ
```

\--- /hint \--- \--- /hints \---

\--- /কাজ \---

\--- task \---

You should also add code to make sure that your boat sprite always starts out looking 'normal'.

Test your code again. If you try to sail the boat through a wooden barrier now, the boat should crash and then move back to its starting position.

![screenshot](images/boat-crash.png)

\--- /task \---