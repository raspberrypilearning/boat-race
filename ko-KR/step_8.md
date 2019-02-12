## Obstacles and boosters

Right now the game is **far** too easy, so you will add some things to make it more interesting.

First, you'll add some boosters to speed up the boat.

\--- task \---

Edit your Stage backdrop by adding in some white booster arrows.

![screenshot](images/boat-boost.png)

\--- /task \---

\--- task \---

Now add more code blocks to your boat's `forever`{:class="block3control"} loop so that the boat sprite moves three extra steps when it touches a white arrow. ![boat-sprite](images/boat_resize.png)

```blocks3
if <touching color [#FFFFFF] ?> then
move (3) steps
end
```

\--- /task \---

\--- task \---

Test your game to see whether your new booster arrows speed up the boat.

\--- /task \---

Next you'll add a spinning gate that the boat has to avoid.

\--- task \---

Add a new sprite that looks like this, and call it 'gate':

![스크린샷](images/boat-gate.png)

Make sure that the colour of the gate sprite is the same as the colour of the wooden barriers.

\--- /task \---

\--- task \---

Make sure that the centre of the gate sprite is positioned in the middle.

![스크린샷](images/boat-center.png)

\--- /task \---

\--- task \---

Add code to your gate sprite to make it spin slowly forever.

\--- hints \--- \--- hint \--- Add code blocks to the gate sprite so that it `turns 1 degree`{:class="block3motion"} `forever`{:class="block3control"}. \--- /hint \--- \--- hint \--- Here are the code blocks you need: ![gate](images/gate.png)

```blocks3
forever
end

turn cw (1) degrees

when flag clicked
```

\--- /hint \--- \--- hint \--- Here's what your new code should look like: ![gate](images/gate.png)

```blocks3
when flag clicked
forever
turn cw (1) degrees
end
```

\--- /hint \--- \--- /hints \---

\--- /task \---

\--- task \---

Test your game again. You should now have a spinning gate that you need to stir your boat around.

![스크린샷](images/boat-gate-test.png)

\--- /task \---