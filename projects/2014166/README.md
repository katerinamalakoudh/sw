
# Pacman
Θέμα εργασίας: Pacman 

Ονοματεπώνυμο: Παπαοικονόμου Νίκος

ΑΜ: Π2014166

Προσωπικό Αποθετηρίο: https://github.com/nikous/pacman

Εκτελέσιμο: https://nikous.github.io/pacman/  

# Σύνοψη
Η εργασία που μου κέντρισε το ενδιαφέρον και με την οποία ασχολήθηκα είναι το παιχνίδι Pacman. Μέσα από την συγκεκριμένη εργασία έμαθα Html5 καθώς και μια πολύ χρήσιμη και βολική βιβλιοθήκη το Phaser που σίγουρα θα την ξαναχρησιμοποιήσω για τα projects μου. Στη συνέχεια θα δούμε κάποιες αλλαγές στον αρχικό κώδικα καθώς και πως λειτουργούν πολλά από αυτά.

# Εισαγωγή 
Το αρχικό παιχνίδι ήταν το απλό pacman που όλοι ξέρουμε αλλά με τις αλλαγές που έγιναν δεν θυμίζει πλέον αυτό. Αρχικά άλλαξα την πίστα με το πρόγραμμα titled  και στην συνέχεια το παίχτη. Πρόσθεσα pokeballs αντί για νομίσματα ,έβαλα εχθρούς που σε κυνηγάνε και σε τρώνε. Έβαλα σκορ ,ζωές καθώς και έκανα το παίχτη να πυροβολεί και να τηλεμεταφέρεται. Τέλος έβαλα κάποιο ήχο να παίζει και κάποια απλά εφέ. 

# Επιλογή εργαλείων
Τα εργαλεία που χρησιμοποίησα είναι τα εξής αρχικά την βιβλιοθήκη Phaser γιατί σου προσφέρει όλα τα απαραίτητα για να φτιάξεις ένα παιχνίδι πιο εύκολα στη συνέχεια το πρόγραμμα titled για να φτιάξω τον χάρτη. Επίσης τον κώδικα τον έτρεχα τοπικά στον υπολογιστή μου με το mongoose και για το debugging χρησιμοποίησα το firebug( extension του Mozilla Firefox). Τέλος χρησιμοποίησα και το photoshop για την επεξεργασία κάποιων sprite/spritesheet.

# Διαδικασία Ανάπτυξης 
Στην αρχή ξεκίνησα με τη αλλαγή του χάρτη χρησιμοποιώντας κάποια έτοιμα tilemaps και έφτιαξα τον δικό μου. Μετά έφτιαξα έναν νέο χαρακτήρα(player) χρησιμοποιώντας κάποια spritesheet που βρήκα. Άλλαξα τα νομίσματα που μαζεύει ο χαρακτήρας και έβαλα 2 pokeballs να απλώνονται σε όλο το χάρτη. 'Έβαλα το σκορ το οποίο ανανεώνεται συνεχώς ανάλογα με τι τρώει ο χαρακτήρας και άμα σκοτώνει κάποιον εχθρό. 

![2](https://cloud.githubusercontent.com/assets/12613497/26833560/7c3ebef4-4adb-11e7-9267-96a825766245.png)

Στη συνέχεια πρόσθεσα τον εχθρό ο οποίος είναι ένας αλλά σε ακολουθάει αρκετά γρήγορα σε όλη τη διαδρομή σου .Το μοτίβο που ακολουθεί είναι πολύ απλό για αυτό και καμιά φόρα κολλάει για λίγο πάνω σε κάποιο εμπόδιο στο χάρτη. Δοκίμασα και το easy star που  είναι ενας πιο απλός Α* αλγόριθμος για pathfinding αλλά δεν τα κατάφερα. 
 
 ![1](https://cloud.githubusercontent.com/assets/12613497/26833599/963fbede-4adb-11e7-9aa4-47b606474b35.png)
 
 Στη συνέχεια έβαλα το παίχτη να χάνει ζωή και τελικά να πεθαίνει όταν τον ακουμπάει ο εχθρός
 
 ![3](https://cloud.githubusercontent.com/assets/12613497/26833604/9c6e7d2c-4adb-11e7-8036-9d9bdfb86beb.png)
 
 Όταν με ακουμπάει ο εχθρός μέσο του overlap χάνω και από μία ζωή. Μέχρι που θα χάσω και τις 3 και θα τελειώσει το παιχνίδι όπου τότε θα έχω τη δυνατότητα να κάνω restart άμα θέλω. Έβαλα και ένα μικρό εφέ μια έκρηξη για όταν πεθαίνω.
 
 ![4](https://cloud.githubusercontent.com/assets/12613497/26833628/b1d34558-4adb-11e7-83b7-b459e4e786c5.png)
 
 Τα πάντα μηδενίζουν στο restart  οι ζωές γίνονται ξανά 3 και γεμίζει ο χάρτης με pokeballs
  
![5](https://cloud.githubusercontent.com/assets/12613497/26833639/ba7199b2-4adb-11e7-940d-78b3afa549e7.png)

Στη συνέχεια έκανα τον παίχτη μου να επιτίθεται στον εχθρό άμα θέλει πατώντας το spacebar και να τον σκοτώνει παίρνοντας πόντους. Ο εχθρός βέβαια αναγεννιέται πάλι μέσα σε λίγα δευτερόλεπτα

![6](https://cloud.githubusercontent.com/assets/12613497/26833662/c786fc50-4adb-11e7-8fc0-162b106ba01c.png)

Τέλος πατώντας το κουμπί Ε στο πληκτρολόγιο ο παίχτης έχει τη δυνατότητα να διαλέξει με το ποντίκι που θα τηλεμεταφερθει εμφανίζοντας ένα μαύρο πλαίσιο που σου δείχνει ακριβώς σε πιο tile θα πας.

![7](https://cloud.githubusercontent.com/assets/12613497/26833665/c8f8c56e-4adb-11e7-8569-7441c810618f.png)


# Συμπεράσματα
Με διευκόλυνε πάρα πολύ το Phaser στην κατασκευή του παχνιδιού καθώς έχει πάρα πολλά tutorials και documentation που σε βοηθούν αρκετά. Κάποια από αυτά που είδα και με βοήθησαν είναι: 
https://phaser.io/examples/v2/arcade-physics/one-way-collision 
https://phaser.io/examples/v2/time/basic-looped-event 
https://phaser.io/examples/v2/groups/add-a-sprite-to-group 
https://phaser.io/examples/v2/category/games
