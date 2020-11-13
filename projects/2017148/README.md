## ΠΡΟΣΩΠΙΚΑ ΣΤΟΙΧΕΙΑ:

### Αντρέας Παππούτας
### ΑΜ: Π2017148

| Εβδομάδα* | Παραδοτέο |
| --- | --- |
| <a href="#P">1</a> |<a href="#P">Φορκ του αποθετηρίου και δημιουργία της σελίδας της αναφοράς με τα προσωπικά στοιχεία σας, της σύνοψης με αυτόν τον πίνακα περιεχομένων, και συγγραφή της εισαγωγής με περιγραφή των αναγκών και των στόχων σας για το αντίστοιχο μάθημα* </a> |
| <a href="#P-1">2</a> |<a href="#P-1"> Άσκηση προγραμματισμού</a> |
| <a href="#P-2">3</a> |<a href="#P-2">  Άσκηση γραμμής εντολών</a> |
| <a href="#P-3">4</a> |<a href="#P-3"> Άσκηση προγραμματισμού + αίτημα ενσωμάτωσης (CSCW, IV)</a> |
|  <a href="#P-4">5 </a> |<a href="#P-4"> Άσκηση γραμμής εντολών</a> |
| <a href="#P-5">6 </a>|<a href="#P-5"> συμμετοχικό περιεχόμενο</a> + <a href="#P-5-1"> Άσκηση προγραμματισμού 3</a> |
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
Για να γίνει αυτό έφτιαξα 2 shell script.
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


## <a name="P-4">Παραδοτέο 4</a>
## Άσκηση: generate plots	create plots for your data from some other course or project
Χρήση δεδομένων από covid-19
COVID-19 Data Repository by the Center for Systems Science and Engineering (CSSE) at Johns Hopkins University
https://github.com/CSSEGISandData/COVID-19
# [Asciinema MatPlotLib](https://asciinema.org/a/370795)
Έγινε χρήση shell scripting, pipelining και python. Μέσο του shell script κατεβάζω τα δεδομένα από το github. Μέσο του python φτιάχνω το plot. Εφόσον τα δεδομένα είναι πολλά το περισσότερο pipelining έγινε μέσα στο πρόγραμμα.
Οι 2 εντολές χρησιμοποιούνται όπως παρακάτω. Ο χρήστης δίνει τη χώρα που θέλει στο bash script και στο python script δίνει το όνομα για το plot του.
```
bash covid.sh COUNTRY_NAME

python covid.py CHART_NAME
```

Για υλοποίηση αυτής της άσκησης εγκατέστησα το MatPlotLib με τη παρακάτω εντολή.
```
python -m pip install -U matplotlib
```

## Το αρχείο covid.sh
```
#!/bin/bash

echo "" > ~/CovidResults/results.csv

cd ~ && cd ~/repositories/COVID-19/csse_covid_19_data/csse_covid_19_daily_reports && git pull

lista=`cd ~ && ls repositories/COVID-19/csse_covid_19_data/csse_covid_19_daily_reports/*.csv`

for KatheFile in $lista

do

count=0

	cd ~ && cat $KatheFile|while IFS=, read -r col1 col2 col3 col4 col5 col6 col7 col8 col9 col10 col11 col13 col14

	do

    		if [[ $col4 == $1 ]]; then

			count=$((count+1))

			cd ~ && echo -n $(echo "$KatheFile" | cut -b 70-79 ) "," >> ~/CovidResults/results.csv && awk 'NR=='$count'' $KatheFile | cut -d ',' -f 8 >> ~/CovidResults/results.csv 

			break;

		else

			count=$((count+1))

		fi

	done

done
```
## Το αρχείο covid.py
```
#!/usr/bin/python
import csv
import datetime as dt
from matplotlib import pyplot as plt                                            
from matplotlib import style                                                    
import numpy as np
import sys                                                             
                                                                                
style.use('ggplot')    
x = []   
y = []

with open('results.csv') as csvfile:
    readCSV = csv.reader(csvfile, delimiter=',')
    next(readCSV)
    for row in readCSV:
	x.append(row[0])
	y.append(row[1])
                                                         
                                                          
test = [dt.datetime.strptime(d,'%m-%d-%Y ').date() for d in x]
arr = np.array(y)
arr2 = arr.astype(np.float)
                                                                          
plt.plot(test,arr2)                                                                                                                       
 
#plt.plot_date(test, arr2)
                                                                               
plt.title(sys.argv[1])                                                              
plt.ylabel("Confirmed")                                                            
plt.xlabel("Time")                                                                      
                                                                                
plt.show()                                                                      
                                                                                
plt.savefig('plot.pdf')                                                         
plt.savefig('plot.svg')                                                         
plt.savefig('plot.png')   
```

## Το results.csv θα είναι στο τέλος της παρακάτω μορφής
```
03-22-2020 ,624
03-23-2020 ,695
03-24-2020 ,743
03-25-2020 ,821
03-26-2020 ,892
03-27-2020 ,966
03-28-2020 ,1061
03-29-2020 ,1156
03-30-2020 ,1212
03-31-2020 ,1314
...
```


Αρχικά στο shell script αδειάζω το αρχείο results.csv για να το χρησιμοποιήσω για τα νέα δεδομένα.
```
echo "" > ~/CovidResults/results.csv
```
Μετά ελέγχω αν βγήκαν καινούργια δεδομένα στο github όπου είναι τα δεδομένα.
```
cd ~ && cd ~/repositories/COVID-19/csse_covid_19_data/csse_covid_19_daily_reports && git pull
```
Ακολούθως μπαίνω στο cloned repository και παίρνω λίστα με όλα τα αρχεία που τελειώνουν σε csv.
```
lista=`cd ~ && ls repositories/COVID-19/csse_covid_19_data/csse_covid_19_daily_reports/*.csv`
```

Πιάνω ένα ένα τα αρχεία απο αυτή τη λιστα και μηδενίζω το counter για καθένα από αυτά στη αρχή έτσι ώστε να μην έχω προβλήματα.
```
for KatheFile in $lista

do

count=0
```
 Μετά στο κάθε αρχείο πιάνω ένα ένα τα column μέσα σε ένα while, οπού βάζω ότι χωρίζεται με ερωτηματικό.
 ```
 cd ~ && cat $KatheFile|while IFS=, read -r col1 col2 col3 col4 col5 col6 col7 col8 col9 col10 col11 col13 col14

	do
```
Τέλος συγκρίνω το όνομα του κάθε column της 4ης σειράς όπου στο κάθε αρχείο είναι το όνομα της χώρας και αν είναι ίδιο με αυτό που δίνει ο χρήστης τότε γράφω στο αρχείο results.csv . Αρχικά γράφω τη ημερομηνία όπου και είναι το όνομα του αρχείου έτσι κόβω αναλόγως τα byte(αυτό αλλάζει αναλόγος που είναι cloned το repository με δεδομένα). Μετά μέσο του awk και του counter που έχω κόβω στη γραμμή όπου είναι η χώρα. Τέλος μέσω cut πιάνω το αριθμό των confirmed που είναι στη 8η γραμμή. Αυτός ο έλενχως γίνεται για όλα τα file που υπάρχουν, έτσι το results.csv θα έχει γραμμές όσα file βρέθηκε η χώρα.
```
if [[ $col4 == $1 ]]; then

			count=$((count+1))

			cd ~ && echo -n $(echo "$KatheFile" | cut -b 70-79 ) "," >> ~/CovidResults/results.csv && awk 'NR=='$count'' $KatheFile | cut -d ',' -f 8 >> ~/CovidResults/results.csv 

			break;

		else

			count=$((count+1))

		fi
```

Στο covid.py αρχίζω με άνοιγμα του αρχείου csv όπου και αναθέτω τη κάθε γραμμή σε ένα πίνακα.
```
with open('results.csv') as csvfile:
    readCSV = csv.reader(csvfile, delimiter=',')
    next(readCSV)
    for row in readCSV:
	x.append(row[0])
	y.append(row[1])
```

Ακολούθως κάνω το y αριθμούς float και το x σε μορφή date.
```
test = [dt.datetime.strptime(d,'%m-%d-%Y ').date() for d in x]
arr = np.array(y)
arr2 = arr.astype(np.float)
```

Στο τέλος αυτού του αρχείου βάζω τίτλο αυτό που έδωσε ο χρήστης, δείχνω το plot και το κάνω export.
```
plt.title(sys.argv[1])                                                              
plt.ylabel("Confirmed")                                                            
plt.xlabel("Time")                                                                      
                                                                                
plt.show()                                                                      
                                                                                
plt.savefig('plot.pdf')                                                         
plt.savefig('plot.svg')                                                         
plt.savefig('plot.png')
```

Στο τελικό αποτέλεσμα μπορείς να δεις ακριβώς σε κάθε ημερομηνία πόσα κρούσματα υπάρχουν.

Το αποτέλεσμα σε εικόνα png:
![plott](https://user-images.githubusercontent.com/44147982/98317544-5b05a300-1fe5-11eb-8056-ed39240d22c1.png)



## <a name="P-5">Παραδοτέο 5</a>
## Συμμετοχικό εκπαιδευτικό υλικό
Εφτιαξα 3 καινούργια δικά μου εργαλεία στο codepen. Το πρωτο δειχνη πως λειτουργουν τα keyframe animations. Το δευτερο δειχνει οπτικοποιηση δεδομένων μέσο google charts. Τελος στο τρίτο έφτιαξα ένα απλό εργαλείο pen.
Τα βήματα και ο κώδικας για τη διμιουργία του κάθε εργαλείου βρίσκονται πιο κάτω.

### Css Animation:
[Link σελίδας αποτελέσματος](https://andreaspappoutas.netlify.app/remix/keyframes_animation/)</br>
[Codepen Link](https://codepen.io/andreaspappoutas/pen/dyXQxbb)</br>
[Link αρχείου md](https://github.com/andreaspappoutas/site/blob/master/_remix/Keyframes_Animation.md)</br>




### Google Charts:
[Link σελίδας αποτελέσματος](https://andreaspappoutas.netlify.app/remix/google-charts/)</br>
[Codepen Link](https://codepen.io/andreaspappoutas/pen/ExyOJZz)</br>
[Link αρχείου md](https://github.com/andreaspappoutas/site/blob/master/_remix/google-charts.md)</br>




### Pen Tool:
[Link σελίδας αποτελέσματος](https://andreaspappoutas.netlify.app/remix/pen-tool/)</br>
[Codepen Link](https://codepen.io/andreaspappoutas/pen/VwjqMgX)</br>
[Link αρχείου md](https://github.com/andreaspappoutas/site/blob/master/_remix/pen-tool.md)</br>





### CSS animation
Στο css animation αρχικά δημιούργησα ένα κύκλο div.
```
<div id="mycircle" class="circle"></div>

.circle {
  height: 50px;
  width: 50px;
  background-color: black;
  border-radius: 50%;
}
```

Στο κομμάτι του javascript έπιασα το div με όνομα circle ενώ επίσης έφτιαξα eventlisteners για αν μετακινηθεί το ποντίκι ή εάν γίνει κλικ.
```
var circle = document.getElementById("mycircle");
document.addEventListener("mousemove", Thesi); 
document.body.addEventListener('click', RunAnimation); 
```

Στο function Thesi παίρνω το χ και το ψ του ποντικιού και ακολούθως βάζω το κύκλο εκεί.
```
function Thesi(){
  x = event.x-20; //-20 gia na einai kentron
  y = event.y-20;//-20 gia na einia kentron
  circle.style.position = "absolute";
  circle.style.left = x + 'px';
  circle.style.top = y + 'px';
}
```

Στο function RunAnimation βάζω να τρέξει το animation και εφόσον τρέξει μέσο timout το αδειάζω έτσι ώστε να μπορεί να τρέξει αυτόματος ξανά στο κλικ.
```
function RunAnimation(){
  circle.style.animation="MyAnimation 4s ease-in-out";
  setTimeout('circle.style.animation=""', 4000)
}
```

Το keyframes MyAnimation
```
@keyframes MyAnimation {
  0% {
    
    transform: scale(1);
  }

  33% {
    background-color: blue;
    opacity: 0.5;
    transform: scale(0);
  }
  66% {
    opacity: 0.8;
    transform: scale(2);
  }
	100% {
    opacity: 1;
    transform: scale(1);
  }
```
  
  
### Google Charts
Αρχικά έβαλα όλα τα κατάλληλα που χρειάζονται για google charts μαζί με το div όπου θα μπει το chart.
```
<div id="Google_paradeigma" style="width: 700px; height: 400px"></div>

document.getElementById('Google_paradeigma')
google.charts.load('current', {'packages':['corechart']});
google.charts.setOnLoadCallback(drawChart);
```
Έβαλα το data και options για κάθε παράδειγμα.
```
var data = google.visualization.arrayToDataTable([
['Year', 'Cyprus', 'Greece'],
['1955', 529972, 8011124],
['1960', 572930, 8273629],
...
var options = {
          title: 'Country Population',
...
```

Έφτιαξα ένα dropdown μενού που καλεί τη function των google charts που λέγεται drawChart και μέσα βάζω μια μεταβλητή αναλόγως ποιο γράφημα θέλω.
```
<div class="dropdown">
  <button class="button">Datasets</button>
  <div class="list">
     <a onclick="drawChart(0)">Population</a>
    <a onclick="drawChart(1)">GDP per capita</a>
    
  </div>
</div>
```

Τέλος μέσο ενός switch μέσα στο drawChart εμφανίζω τα chart που θέλω.
```
switch(p){
          case 0:
            chart.clearChart() //oxi anagkastiko
            chart.draw(data, options);
            break;
          case 1:
            chart.clearChart() //oxi anagkastiko
            chart.draw(data2, options2);
            
        }
```

### Pen Tool
Ξεκίνησα φτιάχνοντας το canvas και περνώντας το αυτό μαζί με το context του στο κομμάτι του javascript
```
<canvas id="toCanvas" width="600" height="300"></canvas>

var canvas = document.getElementById("toCanvas");
var ctx = canvas.getContext("2d");
```

Στο επόμενο κομμάτι δήλωσα ένα control variable που θα χρησιμοποιήσω για να ξέρω τη κατάσταση του πλήκτρου space ενώ επίσης έθεσα τα χ, ψ και πάχος γραμμής
var control= false;
```
let x =0;
let y= 0;
ctx.lineWidth = 5;
```

Εδώ έβαλα αρχικά eventlistener εάν πατήσω κλικ και μετά ένα για αν πατήσω κάποιο πλήκτρο
```
document.body.addEventListener('mousedown', e => {
  document.body.onkeyup = function(e){
```  
  
Αν πατηθεί το space τότε αντιστρέφω το control και αναλόγως αλλάζω το χρώμα των γραμμάτων κάτω από το canvas. Επίσης θέτω τα χ και ψ στο offset του event κάτι που λειτουργεί σαν reset για αυτά.
```
if(e.keyCode == 32){
        control = !control
        if(control==false){
          document.getElementById("space").style.color="black";
        }else{
          document.getElementById("space").style.color="green";
        }
        
        x = e.offsetX
        y = e.offsetY
    }
```

Αν το control είναι θετικό τότε πατήθηκε το space. Οι συντεταγμένες που θα πάρει θα είναι από το eventlistener για κλικ εφόσον δεν θα περάσει από το πιο πάνω if. Τέλος εδώ δημιουργούμε το σχέδιο μέσο του moveTo και lineTo.   
```
if(control==true){
        const newX = e.offsetX;
        const newY = e.offsetY;
        ctx.beginPath();
        ctx.moveTo( x, y ); //apo p na 3ekina
        ctx.lineTo( newX, newY ); //pou na pigeni
        ctx.stroke();
  }
```

Eventlistener για να βρίσκουμε που να προχωρά η γραμμή.
```
window.addEventListener('mouseup', e => {
  x = e.offsetX
  y = e.offsetY
```

Έφτιαξα επίσης ένα κουμπί που κάνει clear το canvas.
```
<button onclick="clearCanvas()">clear</button>

function clearCanvas(){
  ctx.clearRect(0, 0, canvas.width, canvas.height);
}
```

Επίσης ένα slider όπου επιλέγει μέγεθος. Επίσης αλλάζει πιο πάνω το innerHTML και δείχνω τι μέγεθος έχουμε.
```
<input type="range" min="1" max="10" value="5" id="LineWidth">
<h3>Width:</h3><h4 id="h4txt">5</h4>

var valueTXT = document.getElementById("h4txt");
lineWidth.oninput = function() {
  valueTXT.innerHTML = this.value;
  ctx.lineWidth = this.value
}
```

Τέλος έβαλα και την επιλογή να αλλάζει το χρώμα ο χρήστης.
```
<input id="color" type="color" value="#000000" onchange="color()">

function color(){
   ctx.strokeStyle = document.getElementById("color").value;
  
}
```

### <a name="P-5-1"> Άσκηση Προγραμματισμού 3: </a>
### Άσκηση: Τροποποιήστε το παράδειγμα χρησιμοποιώντας φίλτρα εικόνας και συνδυασμούς αυτών. Παραδείγματα φίλτρων βρίσκονται ως σχόλια στην ενότητα με τον CSS κώδικα του παραδείγματος.

Αρχικά έφτιαξα ένα dropdown menu όπου το κάθε κουμπί πάει σε ένα function με διαφορετικό αριθμό ενώ επίσης να αλλάζει το χρώμα του background.
```
<div class="dropdown">
  <button class="button">Filters</button>
  <div class="list">
     <a onclick="changeStyle(0);document.body.style.backgroundColor = '#4B4F4F';">grayscale</a>
 ...
```
Έβαλα και να γίνονται αλλαγές όταν γίνετε hover το κουμπί.
```
.dropdown:hover .button {
  background-color: #333636;
}
```

Στο κομμάτι του javascript αρχικά δημιουργώ style τύπου css όπου θα αλλάζω αργότερα.
```
var style = document.createElement('style');
    style.type = 'text/css';
```
Μετά φτιάχνω το function που καλούν τα κουμπιά και ένα case αναλόγως με τι αριθμό έχει το κάθε κουμπί.
```
function changeStyle(p){
  switch (p){
```

Εδώ θα δείξω 2 παραδείγματα case αλλά και τα υπόλοιπα έχουν το ίδιο σκεπτικό. Πιάνω το innerHTML του style που έφτιαξα και έβαλα πιο πάνω και εφόσον βάλω το στυλ που θέλω το κάνω append στο <head>, δηλαδή το βάζω μέσα στο html.

Με grayscale
```
case 0:
      style.innerHTML = "img:hover{filter:grayscale(1);}";
      document.getElementsByTagName("head")[0].appendChild(style);
      break;
```

Συνδυασμός
```
case 8:
      style.innerHTML = "img:hover{filter:hue-rotate(90deg) sepia(1) brightness(.15);}";
      document.getElementsByTagName("head")[0].appendChild( style );
```
[Codepen Link](https://codepen.io/andreaspappoutas/pen/LYZmzKN)

[Link Κώδικα](https://github.com/andreaspappoutas/site/blob/master/_remix/image-filter.md)

[Link σελίδας αποτελέσματος](https://andreaspappoutas.netlify.app/remix/image-filter/)
