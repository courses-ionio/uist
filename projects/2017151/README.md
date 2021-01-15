## :point_right: ΠΡΟΣΩΠΙΚΑ ΣΤΟΙΧΕΙΑ:

- - - -
### *Θεοδούλου Χαράλαμπος*
### *Π2017151*
### *p17theo3@ionio.gr*

- - - -


| Εβδομάδα* | Παραδοτέο |
| --- | --- |
| <a href="#Paradoteo0">1</a> |<a href="#Paradoteo0">Φορκ του αποθετηρίου και δημιουργία της σελίδας της αναφοράς με τα προσωπικά στοιχεία σας, της σύνοψης με αυτόν τον πίνακα περιεχομένων, και συγγραφή της εισαγωγής με περιγραφή των αναγκών και των στόχων σας για το αντίστοιχο μάθημα* </a> |
|<a href="#Paradoteo1"> 2</a> | <a href="#Paradoteo1">Άσκηση προγραμματισμού </a>|
| <a href="#Paradoteo2"> 3</a>  |<a href="#Paradoteo2"> Άσκηση γραμμής εντολών </a>|
| <a href="#Paradoteo3"> 4</a>  |<a href="#Paradoteo3"> Άσκηση προγραμματισμού </a>|
| <a href="#Paradoteo4"> 5</a>  |<a href="#Paradoteo4"> Γραμμή εντολών </a>|
| <a href="#Paradoteo5"> 5</a>  |<a href="#Paradoteo5">συμμετοχικό περιεχόμενο </a>|
| <a href="#Paradoteo6"> 5</a>  |<a href="#Paradoteo6">αιτημα ενσωμάτωσης</a>|
| 8 | Άσκηση προγραμματισμού (HCI) ή γραμμής εντολών (SW) |
| 9 | Άσκηση γραμμής εντολών (SW) ή αίτημα ενσωμάτωσης (CSCW, IV) |
| 10 | συμμετοχικό περιεχόμενο |
| 11 | αίτημα ενσωμάτωσης (CSCW, IV) |
| 12 | Τελική αναφορά* |



## <a name="Paradoteo0">:point_right: *Εισαγωγή*</a>

Οπτικοποίηση της πληροφορίας είναι η μετατροπή των γεγονότων και της πληροφορίας σε μορφή η οποία να είναι πιο κατανοητή και πιο εύκολα ερμηνεύσιμη. Στόχος μου είναι να καταφέρω  επιτυχώς να μάθω καλά  το πώς  φτάνουμε από τα δεδομένα στην πληροφορία και τους  τρόπους της οπτικής αναπαράστασης οι οποίοι δίνουν την δυνατότητα στον άνθρωπο να την κατανοεί πιο εύκολα , επίσης  θέλω να μάθω να αναγνωρίζω ποια είναι η σωστή τεχνική για κάθε περίπτωση (με βάση το είδος της πληροφορίας και το κοινό που θα την αξιοποίηση.)
- - - -




## <a name="Paradoteo1">:point_right: *Πρώτο Παραδοτέο*</a>
*Άσκηση: Τροποποιήστε τον κώδικα του παραδείγματος προσθέτοντας και οπτικοποιώντας στο ίδιο πλαίσιο περισσότερα από 2 σετ δεδομένων (datasets).*

Για την εκπόνηση της πρώτης εργασίας , έτσι ώστε να τροποποιήσω το visualazastion πρόσθεσα  ένα ακόμα   DataSet C κουμπί στο html κομμάτι , το οποίο να πηγαίνει στο function triggerDatasetC. Ακολούθως στo JS κομμάτι δήλωσα το dataset C με διαφορετικούς αριθμούς έτσι ώστε να έχω διαφορετικά αποτελέσματα.  Έπειτα δημιούργησα ένα νέο function το οποίο λέγετε triggerDatasetC το οποίο είναι ουσιαστικά ίδιο με τα αλλά δυο με την μονή διαφορά  η γραμμή κώδικα να είναι "var dataset = datasetC" ετσι ώστε να μπορεσω να εμφανίσω και τα 3 κουμπιά 

[Codepen Link](https://codepen.io/p17theo3/pen/NWrrNWe)

[Link Κώδικα](https://github.com/p17theo3/site/blob/master/_remix/visualization-dataset.md)

[Link σελίδας αποτελέσματος](https://p17theo3.netlify.app/remix/visualization-dataset/)
  
- - - -



## <a name="Paradoteo2">:point_right: *Δεύτερο Παραδοτέο*</a>
*Άσκηση: visualize your data | demo with your git commits history and percipation data per day for the last month from your city.*

Για την εκπόνηση της δεύτερης  εργασίας εγινε χρήση του spark και του git spark τα οποία εγκατέστησα με τα παρακάτω commands:

## Spark
```
sudo sh -c "curl https://raw.githubusercontent.com/holman/spark/master/spark -o /usr/local/bin/spark && chmod +x /usr/local/bin/spark
```

## Git spark
```
curl -L http://cpanmin.us | perl - --sudo App::cpanminus
cpanm App::Git::Spark
```

Εφόσον έκανα την εγκατάσταση τον παραπάνω έκανα clone το hci έτσι ώστε σε αυτό να μπορώ να δείξω τα commits μου. Επίσης μέσω του spark έδειξα ένα απλό γράφημα. Για commit διάλεξα να δείξω τα τελευταία τρία χρονιά.



*Για το πρώτο γράφημα έκανα χρήση του παρακάτω command*
```
spark 1 2 3 4 5 6 7 8 9 10
```








*Για να δείξω τα τελευταία τρία χρόνια του hci έκανα χρήση του παρακάτω command*

```
git spark --years 3 p17theo3
```


[asciinema url](https://asciinema.org/a/367741)


## <a name="Paradoteo3">:point_right: *Τρίτο Παραδοτέο*</a>
*Άσκηση: Τροποποιήστε το παράδειγμα χρησιμοποιώντας φίλτρα εικόνας από το προηγούμενο παράδειγμα. Συνδυάστε τα φίλτρα εικόνας και τη χρήση zoom κατά τη λειτουργία hover (κίνηση του ποντικιού πάνω από την εικόνα).*


*για την πραγματοποίηση της εργασίας αρχικά έβαλα ενα id wraptest για να μπορώ να πιάσω μετά το element στο js κομμάτι*
```
<div id="wrapTest" class="wrap">
  ```
*στη συνέχεια έβαλα ενα div me id entotext οπού λέγετε zoomin το οποίο μετά θα το έκρυβα κάνοντας την χρήση του hover*
```
id="entotext">Zoom In</div></div>
```
*στη συνέχεια στο css  στο hover κομμάτι έβαλα τα filter* **- greyscale - salurate - sepia **
```
filter: grayscale(1);
filter: saturate(50%);
filter: sepia(80%);
```
*ακόμη μια αλλαγή που σκεφτικά είναι το cursor στο zoomin να αλλάζει και επίσης έφυγα το background position και background zise*
```
cursor: zoom-in;
```
~~background-potition:100%;~~
~~background-size:100%;~~

*στο js κομμάτι test1 έπιασα το wrap  μέσο του jquery οπού είναι μέσα η εικόνα*
```
var test1 = document.querySelector("#wrapTest");
```
*στην συνέχεια επιασα το zoomin και έβαλα στο wrap eventlistenet οπου γίνεται το function mouseover να γίνεται run το function testtozoomi*
```
var textt = document.getElementById("entotext");
test1.addEventListener("mouseover", testTozoomi);
```

*ακολούθος μεσα στο function testtozoomi εκανα το visibility το textZoomin να είναι hidden*
```
function testTozoomi(){
textt.style.visibility = "hidden";
```
 *εφόσον ξέρω ότι ήδη ο χρήστης έχει το  mouse το πάνω από την εικόνα τότε από το eventlistener που έχουμε πιο πάνω (mouse over) τότε έβαλα ενα νέο eventlistener που ελέγχει αν μετακινείτε το mouse του.*
```
test1.addEventListener("mousemove", (e)
```

*το offset κανει τα pixel της εικονας (px)  να πηγαινει αντίθετα με το mouse*
```
test1.addEventListener("mousemove", (e) =>
{
test1.style.backgroundPositionX = -e.offsetX + "px";
tes
```


*τέλος όταν κάνει load η σελίδα έβαλα ενα απλό μήνυμα να εμφανίζεται στην οθόνη*
```
window.addEventListener('load',
function()
{
alert('δοκίμασε να κάνεις ζούμ!!!!');
}
);
```




[Codepen Link](https://codepen.io/p17theo3/pen/oNLdZRO)

[Link Κώδικα](https://github.com/p17theo3/site/blob/master/_remix/image-zoom.md)

[Link σελίδας αποτελέσματος](https://p17theo3.netlify.app/remix/image-zoom/)
  
- - - -




## <a name="Paradoteo4">:point_right: *Τέταρτο Παραδοτέο*</a>

*Άσκηση: visualize git commits display your commits from a previous course, eg hci.*
```
#!/bin/bash

if [[ -n $3 ]]; then
cd ~ && cd Desktop/myrepos/$1/ && git-bars -p $2 -u $3
else
cd ~ && cd Desktop/myrepos/$1/ && git-bars -p $2
fi
```

*μέσω αφού του κώδικα ο χρήστης δίνει τρία  arguments , το πρώτο είναι το όνομα του repository , το δεύτερο η διάρκεια και το τρίτο ο συγγραφέας. Αν δεν δώσει τρίτο argument όμως πάλι λειτουργά.*

Παράδειγμα:
```

Bash barrues.sh mm day p17theo3 
```

*αρχικά στον κώδικα έλεγχο αν υπάρχει το τρίτα argument και αν ναι τρέχω το πρόγραμμα με συγγραφέα.*
```

if [[ -n $3 ]]; then
cd ~ && cd Desktop/myrepos/$1/ && git-bars -p $2 -u $3
```

*ακολούθως αν δεν υπάρχει απλά το πρόγραμμα τρέχει χωρίς συγγραφέα *
```
else
cd ~ && cd Desktop/myrepos/$1/ && git-bars -p $2
fi
```

[Link αποτελέσματος](https://asciinema.org/a/370970)

## <a name="Paradoteo5">:point_right: *Πέμπτο Παραδοτέο*</a>

*Άσκηση: Συμετοχικό  περιεχόμενο*

*Αρχικά έκανα  ένα visualization του covid οπού βρήκα  τα στοιχεία από το worldometer* 


[Link αποτελέσματος](https://p17theo3.netlify.app/remix/worldometer/) </br>
*Σαν άσκηση έβαλα να πρέπει να αλλάξουν την γραμματοσειρά και τα χρώματα  του γραφήματος* 

*Σαν δεύτερο παράδειγμα  έβαλα ένα  generator κωδικού μέσο js* 

[Link αποτελέσματος](https://p17theo3.netlify.app/remix/password)

*Σαν άσκηση έβαλα να πρέπει να αλλάξουν των κώδικα έτσι ώστε να μπορεί να γίνετε χρήση ελληνικών χαρακτήρων*

## <a name="Paradoteo6">:point_right: *Έκτο Παραδοτέο*</a>
Αιτημα ενσωματωσης - Εχω επιλεξη να ενημερωσω το προγραμμα σπουδων

Αλλαγες - 
-Μετακίνηση μαθήματος επιλογής Ζ' εξαμήνου «Ειδικά θέματα Διδακτικής της Πληροφορικής» ως μάθημα επιλογής στο Η’ εξάμηνο

-Μετακίνηση μαθήματος επιλογής Ζ' εξαμήνου «Διαχείριση Έργων Πληροφορικής» στο Η’ εξάμηνο

-Αλλαγή καθηγητή στο μάθημα Εισαγωγή στον Προγραμματισμό

[link sto issue](https://github.com/ioniodi/sitegr/issues/10)
[link sto pull request](https://github.com/ioniodi/sitegr/pull/19)


























