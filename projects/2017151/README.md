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
| 5 | Άσκηση γραμμής εντολών |
| 6 | Άσκηση προγραμματισμού (HCI) ή γραμμής εντολών (SW)+ συμμετοχικό περιεχόμενο |
| 7 | Άσκηση γραμμής εντολών (SW) + αίτημα ενσωμάτωσης (CSCW, IV) |
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






