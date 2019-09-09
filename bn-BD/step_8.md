## বাধা এবং boosters

এই মুহুর্তে খেলাটি **পর্যন্ত** খুব সহজ, তাই আপনি আরো আকর্ষণীয় করতে কিছু জিনিস যুক্ত করুন।

প্রথম, আপনি নৌকা গতিতে কিছু boosters যোগ করব।

\--- কাজ \---

কিছু সাদা সহায়তাকারী তীর যোগ করে আপনার স্টেজ ব্যাকড্রপ সম্পাদনা করুন।

![screenshot](images/boat-boost.png)

\--- /কাজ \---

\--- কাজ \---

এখন আপনার নৌকাটির `চিরকালের জন্য আরও কোড ব্লক যুক্ত করুন`{: class = "block3control"} লুপ যাতে নৌকাটি একটি সাদা তীর স্পর্শ করে তিনটি অতিরিক্ত ধাপে চলে যায়। ![নৌকা-পরী](images/boat_resize.png)

```blocks3
যদি <touching color [#FFFFFF] ?> তারপর
পদক্ষেপ (3) পদক্ষেপ
শেষ
```

\--- /কাজ \---

\--- কাজ \---

আপনার নতুন বুস্টার তীর বোট গতি বাড়া কিনা দেখতে আপনার খেলা পরীক্ষা করুন।

\--- /কাজ \---

পরবর্তী আপনি একটি কাটিয়া গেট যুক্ত হবে যে নৌকা এড়াতে হবে।

\--- কাজ \---

এটির মতো একটি নতুন স্প্রাইট যোগ করুন এবং এটি 'গেট' কল করুন:

![screenshot](images/boat-gate.png)

গেট স্প্রাইটের রঙটি কাঠের বাধাগুলির রঙের মতোই নিশ্চিত।

![screenshot](images/brown-hsv.png)

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![screenshot](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![গেট](images/gate.png)

```blocks3
সর্বদা
শেষ

বিন্দু CW (1) ডিগ্রী

যখন পতাকা ক্লিক করা হয়
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
যখন পতাকা
চিরকালের জন্য ক্লিক করুন

 সিউ (1) ডিগ্রী
শেষ
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![screenshot](images/boat-gate-test.png)

\--- /task \---