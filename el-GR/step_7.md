## Προσθέτοντας ένα χρονόμετρο

Τώρα θα προσθέσεις ένα χρονόμετρο στο παιχνίδι σου, έτσι ώστε ο παίκτης να πρέπει να φτάσει στο νησί το συντομότερο δυνατόν.

--- task ---

Πρόσθεσε μια νέα μεταβλητή με το όνομα `χρόνος`{:class="block3variables"} στο Σκηνικό σου.

![screenshot](images/boat-variable-annotated.png)

[[[generic-scratch3-add-variable]]]

Μπορείς επίσης να επιλέξεις μια εμφάνιση του χρονομέτρου σου αλλάζοντας τον τρόπο απεικόνισής του στην οθόνη.

--- /task ---

--- task ---

Τώρα πρόσθεσε κώδικα στο Σκηνικό σου έτσι ώστε το χρονόμετρο να μετρά τον χρόνο μέχρι η βάρκα να φτάσει στο νησί.

--- hints ---
--- hint ---

Στο Σκηνικό, `όταν στην πράσινη σημαία γίνει κλικ`{:class="block3control"}, `όρισε τη μεταβλητή χρόνος σε 0`{:class="block3variables"}. Μέσα στην δομή επανάληψης `για πάντα`{:class="block3control"}, θα πρέπει πρώτα να `περιμένεις 0.1 δευτερόλεπτα`{:class="block3control"}, και μετά `άλλαξε την τιμή της μεταβλητής χρόνος κατά 0.1`{:class="block3variables"}.

--- /hint ---
--- hint ---
Εδώ είναι τα μπλοκ εντολών που θα χρειαστείς:

![φάση](images/stage.png)

```blocks3
change [χρόνος v] by (0.1)

when flag clicked

forever
end

wait (0.1) seconds

set [χρόνος v] to [0]
```

--- /hint ---
--- hint ---

Έτσι πρέπει να είναι ο κώδικάς σου:

![φάση](images/stage.png)

```blocks3
when flag clicked
set [χρόνος v] to [0]
forever
wait (0.1) seconds
change [χρόνος v] by (0.1)
end
```

--- /hint ---
--- /hints ---

--- /task ---

--- task ---

Αυτό είναι! Δοκίμασε το παιχνίδι σου και δες πόσο γρήγορα μπορείς να φτάσεις στο έρημο νησί!

![screenshot](images/boat-variable-test.png)

--- /task ---