## ΠΡΟΣΩΠΙΚΑ ΣΤΟΙΧΕΙΑ:

### Αντρέας Παππούτας
### ΑΜ: Π2017148

| Εβδομάδα* | Παραδοτέο |
| --- | --- |
| <a href="#P">1</a> |<a href="#P">Φορκ του αποθετηρίου και δημιουργία της σελίδας της αναφοράς με τα προσωπικά στοιχεία σας, της σύνοψης με αυτόν τον πίνακα περιεχομένων, και συγγραφή της εισαγωγής με περιγραφή των αναγκών και των στόχων σας για το αντίστοιχο μάθημα* </a> |
| <a href="#P-1">2</a> |<a href="#P-1"> Άσκηση προγραμματισμού</a> |
| <a href="#P-2">3</a> |<a href="#P-2">  Άσκηση γραμμής εντολών</a> |
| <a href="#P-3">4<a href="#P-3"> |<a href="#P-3"> Άσκηση προγραμματισμού + αίτημα ενσωμάτωσης (CSCW, IV)<a href="#P-3"> |
| 5 | Άσκηση γραμμής εντολών |
| 6 | Άσκηση προγραμματισμού (HCI) ή γραμμής εντολών (SW)+ συμμετοχικό περιεχόμενο |
| 7 | Άσκηση γραμμής εντολών (SW) + αίτημα ενσωμάτωσης (CSCW, IV) |
| 8 | Άσκηση προγραμματισμού (HCI) ή γραμμής εντολών (SW) |
| 9 | Άσκηση γραμμής εντολών (SW) ή αίτημα ενσωμάτωσης (CSCW, IV) |
| 10 | συμμετοχικό περιεχόμενο |
| 11 | αίτημα ενσωμάτωσης (CSCW, IV) |
| 12 | Τελική αναφορά* |


## <a name="P">ΕΙΣΑΓΩΓΗ:</a>
Μέσο της οπτικοποίηση της πληροφορίας προσπαθούμε να δημιουργήσουμε μια διάδραση με τα δεδομένα που έχουμε έτσι ώστε να γίνουν πιο διακριτά. Έχω σαν στόχο να μάθω να οργανώνω με σωστό τρόπο τα δεδομένα σε ένα υψηλότερο επίπεδο. Σκοπός μου είναι να μάθω τεχνικές διαχείρισης τον διάφορων πληροφοριών(γραφικά , εικόνες , βίντεο κτλ) ενώ επίσης να αποκτήσω γνώση στις σύγχρονες τεχνολογίες που χρησιμοποιούνται για τη οπτικοποίηση τους.

---


## <a name="P-1">Παραδοτέο 1</a>
### Άσκηση: Τροποποιήστε τον κώδικα του παραδείγματος προσθέτοντας και οπτικοποιώντας στο ίδιο πλαίσιο περισσότερα από 2 σετ δεδομένων (datasets).


Επέλεξα για άσκηση προγραμματισμού να αλλάξω το visualization dataset. 
Στη άσκηση αυτή αρχικά δήλωσα στη javascript το νέο *"datasetC=[..]"* . 
Στη html δημιούργησα ένα κουμπί ίδιο τα με τα άλλα 2 για το datasetC και άλλαξα μόνο το *onclick* να πηγαίνει στο *triggerDatasetC*. 
Στη συνέχεια δημιούργησα ακριβώς το ίδιο function με αυτό που χρησιμοποιείτε για τα άλλα 2 όπου και το ονόμασα *triggerDatasetC*. 
Σε αυτό το νέο function η μόνη αλλαγή που χρειάζονταν ήτανε στη αρχή το *"var dataset = datasetC"*. 
Στο τέλος εφόσον είχα δηλωμένο ένα νέο datasetC με δικό του function και κουμπί που να πηγαίνει σε αυτό το function τότε μπορούσαμε να απεικονίσουμε 3 dataset.

[Codepen Link](https://codepen.io/andreaspappoutas/pen/ZEOQLvm)

[Link Κώδικα](https://github.com/andreaspappoutas/site/blob/master/_remix/visualization-dataset.md)

[Link σελίδας αποτελέσματος](https://andreaspappoutas.netlify.app/remix/visualization-dataset)


## <a name="P-2">Παραδοτέο 2</a>
### Άσκηση: visualize your data |	demo with your git commits history and percipation data per day for the last month from your city.

[Asciinema-Spark](https://asciinema.org/a/367160)

Ξεκίνησα τη πρώτη άσκηση γραμμής εντολών με τη οπτικοποίηση των commits μου στο IV μέσο του εργαλείου spark.
Άρχισα αυτή τη άσκηση με τη εγκατάσταση του spark:
```
sudo sh -c "curl https://raw.githubusercontent.com/holman/spark/master/spark -o /usr/local/bin/spark && chmod +x /usr/local/bin/spark"
```
Έτρεξα μια απλή εντολή για οπτικοποίηση μιας ακολουθίας αριθμών.
```
spark 0 2 4 6 8 10 12
```
Ακολούθως με τη παρακάτω εντολή έκανα εγκατάσταση του git spark ένα εργαλείο με το οποίο μπορούμε να οπτικοποιήσουμε πληροφορίες για το github.

```
curl -L http://cpanmin.us | perl - --sudo App::cpanminus
cpanm App::Git::Spark
```

Έφτιαξα ένα νέο φάκελο όπου και έβαλα μέσα το repository iv και έτρεξα τη παρακάτω εντολή για να δείξω πόσα commits έκανα τις τελευταίες 15 μέρες.
```
git spark --days 15 andreaspappoutas
```


## Βελτίωση άσκησης με χρήση pipelining και shell scripting

### Έφτιαξα 2 διαφορετικούς τρόπους για χρήση shell scripting και pipelining. Στο πρώτο τρόπο κάνω spark από ένα οποιοδήποτε αρχείο csv τη στήλη που θέλω. Στο δεύτερο τρόπο κάνω spark τα commits οποιουδήποτε συγγραφέα θέλω.

### [Asciinema-Spark Shell&PipeliningCSV](https://asciinema.org/a/368965)
 Για το παράδειγμα έκανα χρήση των δεδομένων: [Πίνακας πλήθους Ελλήνων εκλογέων ανά εκλογικό διαμέρισμα (Δημοτικές - Περιφερειακές εκλογές 2010)](https://geodata.gov.gr/en/dataset/plethos-ellenon-eklogeon-ana-eklogiko-diamerisma-demotikes--periphereiakes-ekloges-2010/resource/b67372da-aa78-4de1-ba76-9bb792c179c1)


### [Asciinema-Spark Shell&Pipelining Git Commits](https://asciinema.org/a/369127)
Έκανα χρήση του d3 σε αυτό το παράδειγμα εφόσον είχε περισσότερα commits.






### CSV Spark:
Μέσο shell scripting και pipelining πιάνω ένα αρχείο csv, δίνω όνομα της στήλης που θα ήθελα να κάνω σε γράφημα και εμφανίζετε στο τέλος μέσο της εντολής spark.
Για να γίνει αυτό έφτιξα 2 shell script.
Η τελική εντολή είναι η παρακάτω:
```
bash Script1.sh https://WEBSITE.COM/OURFILE.csv | xargs -t bash Script2.sh "COLUMN_TO_SPARK" | xargs -t cut -d ',' -f | sed "s/[^0-9]//g" | spark
```
#### Script1.sh :
```
#!/bin/bash

curl -o output.csv $1
echo output.csv
```
#### Script2.sh
```
#!/bin/bash

colnames=$(head -n 1 < $2)
colnames2=$( echo -e "$colnames" | tr  ' ' '_'  )
arr=(${colnames2//,/ })


for item in ${arr[@]}; do
	etoimo=$(echo "$item" | tr -d '"')
	count=$((count+1))
   if [ "${etoimo}" == "${1}" ]; then
     echo "$count"
   fi
done
echo "$2"
```
Η ιδέα είναι μέσο του ονόματος της στήλης που θέλω από ένα csv να εμφανίζονται τα αποτελέσματα.
Στο Script1.sh μέσο του cURL κατεβάζω το πρώτο argument που δίνει ο χρήστης εφόσον είναι σύνδεσμος και το αποθηκεύω σαν output.csv. Έτσι το Script.1 χρησιμοποιείτε όπως παρακάτω:
```
bash Script1.sh https://WEBSITE.COM/OURFILE.csv 
```
Στο Script2 το πρώτο argument που θα δίνετε θα είναι το όνομα της στήλης που θέλουμε να φτιάξουμε το γραφημά μας άπο τα δεδομένα της και το δεύτερο θα είναι το όνομα του αρχείου. Έτσι ξέρω ότι $1 = όνομα στήλης και $2 = αρχείο. Το Script1 δεν είναι απαραίτητο αν έχεις ήδη κατεβασμένο το αρχείο csv.
Αρχικά παίρνω τους τίτλους της κάθε στήλης. Αντικαθιστώ οποιοδήποτε κενό με το χαρακτήρα "_" εφόσον μου δημιουργούσε προβλήματα. Τέλος το χωρίζω ανά κόμμα μέσα σε ένα πινάκα.
```
colnames=$(head -n 1 < $2)
colnames2=$( echo -e "$colnames" | tr  ' ' '_'  )
arr=(${colnames2//,/ })
```

Ακολούθως μέσο ενός for loop βλέπω το κάθε τίτλο ξεχωριστά σαν ένα item. Φεύγω το χαρακτήρα " για ευκολία στη σύγκριση στο if και δημιουργώ ένα counter για να ξέρω σε ποια στήλη είμαι.
```
etoimo=$(echo "$item" | tr -d '"')
	count=$((count+1))
```

Στο if ελένχω αν έχω τη στήλη που δόθηκε. Αν το argument 1, δηλαδή το όνομα της σειράς που δίνετε, είναι ίδιο με οποιοδήποτε από τους τίτλους μέσα στο πίνακα τότε το τυπώνουμε το αριθμό της για να το χρησιμοποιήσουμε στο επόμενο πρόγραμμα του pipe.
```
if [ "${etoimo}" == "${1}" ]; then
     echo "$count"
   fi
```

Τελειώνοντας με το αρχείο αυτό τυπώνω το όνομα του csv εφόσον θα είναι χρήσιμο για τα επόμενα προγράμματα.
```
echo "$2"
```
Χρήση του Script2. Χρήση xargs για περισσότερο έλενχο.
```
xargs -t bash Script2.sh "COLUMN_TO_SPARK"
```
Μετά μεσώ του cut έφυγα όλα τα δεδομένα εκτός της σειράς που επιλέξαμε:

```
xargs -t cut -d ',' -f
```
*Αμέσως μετά το -f θα ακολούθηση ο αριθμός της σειράς που τυπώσαμε πιο πάνω εάν βρέθηκε και το όνομα του αρχείου.*


Τέλος μέσο του sed φέυγω όλα τα γράμματα και αφήνω μόνο τους αριθμούς. Τρέχω τα αποτέλεσμα μέσο pipelining στο spark.
```
 sed "s/[^0-9]//g" | spark
```
  
<br/>
<br/>
<br/>
  
### Github Commits Spark:
Έφτιαξα 2 script. Το πρώτο φέρνει το log.csv ενώ το δεύτερο βρίσκει τη συχνότητα commits κάθε μέρας για το συγγραφέα που θα δώσουμε.
Το τελικό command:
```
bash log.sh "repository" "siggrafeas" | awk '{print $3,$4,$6}' log.csv > log2.csv | bash deutero.sh | 
sed "s/[^0-9]//g" | spark
```

#### log.sh:
```
#!/bin/bash

cd ~ && cd repositories && cd $1 && git log --pretty=format:'%h;%an;%ad;%s' --author=$2 > ~/sparkTouGithub/log.csv
```
#### deutero.sh
```
#!/bin/bash

tr -s ' ' '_' < log2.csv > log3.csv
tr -s ' ' '\n' < log3.csv | uniq -c -d | cut -b 1-7
```

Αρχικά στο log.sh μέσο του cd πάω στο φάκελο με τα git clones. Το πρώτο argument που έχουμε θα είναι το όνομα του repository έτσι και θα μπούμε στο φάκελο αυτού.
```
cd ~ && cd repositories && cd $1
```

Μετά μέσο του git log περνούμε τα commits σε μορφή csv και αποθηκεύουμε το αρχείο στο φάκελο που έχουμε τα 2 shell scripts. Ξέρουμε οτι το δεύτερο argument που θα δοθεί θα είναι το όνομα του συγγραφέα.
```
git log --pretty=format:'%h;%an;%ad;%s' --author=$2 > ~/sparkTouGithub/log.csv
```

Ακολούθως με το awk παίρνω τη τρίτη,τέταρτη και έκτη στήλη εφόσον αυτές δείχνουν την ημερομηνία commit που μας ενδιαφέρει. Το αποτέλεσμα το στέλνω στο αρχείο log2.csv.
```
awk '{print $3,$4,$6}' log.csv
```

Στο deutero.sh ξεκινώ με αντικατάσταση των κενών με το χαρακτήρα "_" εφόσον θα χρειαστεί να βρούμε duplicates.
```
tr -s ' ' '_' < log2.csv > log3.csv
```

Βρίσκουμε τη συχνότητα της κάθε ημερομηνίας έτσι ώστε να χρησιμοποιηθεί πιο μετά για δημιουργία γραφήματος μέσο του spark.
```
tr -s ' ' '\n' < log3.csv | uniq -c -d
```

Τελειώνοντας με το script αυτό κάνουμε cut τα πρώτα 7 bytes. Το αποτέλεσμα του command tr πιο πάνω μας έδινε δίπλα από της συχνότητες και τη ημερομηνία κάτι που δεν χρειαζόμαστε για το spark.
```
cut -b 1-7
```

Τέλος κρατώ μόνο τους αριθμούς μέσο του sed και τρέχω τα αποτελέσματα μέσω pipelining στο προγραμμα spark.
```
sed "s/[^0-9]//g" | spark
```

## <a name="P-3">Παραδοτέο 3</a>
### Άσκηση 1: Τροποποιήστε το παράδειγμα έτσι ώστε όταν το αυτοκίνητο κινείται όπισθεν να έχει μικρότερη (τη μισή) ταχύτητα από το όταν κινείται έμπροσθεν.
### Άσκηση 2: Δημιουργείστε περιμετρικά όρια έτσι ώστε το αυτοκίνητο να μη βγαίνει ποτέ έξω από την πίστα.

Για τη άσκηση 1 βρήκα στο κώδικα javascript το "onkeydown" όπου και βλέπουμε ανά πόσα pixels αλλάζει το αυτοκίνητο όταν το κάθε κουμπί είναι πιεσμένο. Τα κουμπιά είναι γραμμένα με το κωδικό τους κάτι που μπορεί να βρεθεί εύκολα από αυτή τη [σελίδα](https://keycode.info).
```
if (key == 37) dx=-4; else if (key == 38) dy=-4; else if (key == 39) dx=4; else if (key == 40) dy=4;
```
Η όπισθεν είναι το κουμπί με το αριθμό 40 έτσι το αλλάζουμε να σε 2.
```
if (key == 40) dy=4
```

Στη άσκηση 2 αρχικά πρέπει να φτιάξουμε ένα function για το κάθε άξονα που θα ελέγχει αν το αυτοκίνητο είναι μέσα στα όρια του canvas.
```
function testX(x){
  if((x<1000) && (x>0)){
    return true;
  }
  else return false;
}

function testY(y){
  if((y<800) && (y>0)){
    return true;
  }
  else return false;
}
```
Αν είναι μέσα στα όρια επιστρέφει true αλλιώς false
Μέσο του ίδιου σκεπτικού φτιάχνουμε function για όταν το αυτοκίνητο είναι εκτός ορίων.
}
```
function AllagiX(x){
  if(x>=1000){
    x=x-1;
    //x=1; diaforetiko
    return x;
  }
  else if(x<=0){
    x=x+1;
    //x=999;
    return x;
  }
}
function AllagiY(y){
  if(y>=800){
    y=y-1;
    return y;
  }
  else if(y<=0){
    y=y+1;
    return y;
  }
}
}
```
Αν βγει εκτός ορίων αριστερά η πάνω από το canvas του προσθέτουμε ενώ αντίθετα αν είναι δεξιά ή κάτω του αφαιρούμε.
Τέλος συνδυάζουμε αυτά τα 2 functions με 2 απλά if όπου εφόσον έχουμε true δεν χρειάζεται να γίνει αλλαγή στη τοποθεσία του αυτοκινήτου έτσι δεν καλούνται οι function για αλλαγή.
```
if(testX(x)){
    x = x - dy * Math.cos(angle * Math.PI / 180);
  }
    else{
      x = AllagiX(x);
    }
    
  if(testY(y)){
    y = y - dy * Math.sin(angle * Math.PI / 180);
  }
    else{
      y = AllagiY(y);
    }
```
[Codepen Link](https://codepen.io/andreaspappoutas/pen/YzWwgMW)

[Link Κώδικα](https://github.com/andreaspappoutas/site/blob/master/_remix/keyboard-input.md)

[Link σελίδας αποτελέσματος](https://andreaspappoutas.netlify.app/remix/keyboard-input/)
