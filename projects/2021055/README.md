# Οπτικοποίηση της Πληροφορίας

### ΟΝΟΜΑΤΕΠΟΝΥΜΟ: AΧΙΛΛΕΑΣ ΖΕΡΒΟΣ

### ΑΡΙΘΜΟΣ ΜΗΤΡΩΟΥ: INF2021055

### Η ΟΜΑΔΑ ΜΟΥ: [OMADA11](https://github.com/orgs/OMADA11/repositories)

| Εβδομάδα | [Όλα τα παραδοτέα βρίσκονται στην ίδια σελίδα της τελικής αναφοράς](https://epidrome.github.io/teaching/deliverables/) με τα προσωπικά στοιχεία σας (Όνομα, ΑΜ, github profile) και μαζί με αυτόν εδώ τον πίνακα περιεχομένων | Σύνδεσμος στην [εβδομαδιαία παρουσίαση προόδου στις συζητήσεις](https://github.com/courses-ionio/iv/discussions/categories/show-and-tell) | Αυτοαξιολόγηση σύμφωνα με τα κριτήρια της αντίστοιχης άσκησης |
| --- | --- | --- | --- |
| 1 |  [Φορκ και δημιουργία σελίδας τελικής αναφοράς](https://courses-ionio.github.io/help/guide/), [προσθήκη πίνακα περιεχομένων](https://raw.githubusercontent.com/courses-ionio/iv/master/README.md), [συγγραφή της εισαγωγής](https://epidrome.github.io/teaching/intro/), αποστολή της εισαγωγής για σχολιασμό στην συζήτηση και καταγραφή του συνδέσμου συζήτησης δίπλα --> |https://github.com/courses-ionio/iv/discussions/15 | |
| 2 | Άσκηση γραμμής εντολών (archlinux+wm) | https://github.com/courses-ionio/iv/discussions/24
| 3 | Εναλλακτικό σύστημα | https://github.com/courses-ionio/iv/discussions/25
| 4 | Άσκηση γραμμής εντολών (custom wm) | https://github.com/courses-ionio/iv/discussions/26
| 5 | Αίτημα ενσωμάτωσης |
| 6 | Άσκηση γραμμής εντολών (cli data analysis) |
| 7 | Εναλλακτικό σύστημα |
| 8 | Άσκηση γραμμής εντολών (cli data analysis) |
| 9 | Αίτημα ενσωμάτωσης |
| 10 | Τελική αναφορά |

# ΠΑΡΑΔΟΤΕΟ 1 - Εισαγωγή

Στο μάθημα οπτικοποίηση της πληροφορίας, ευελπιστώ να μάθω να χρησιμοποιώ νέα εργαλεία και ταυτόχρονος να εξοικειωθώ ακόμη περισσότερο με τα ήδη υπάρχοντα που έχω μάθει. Στόχος μου αποτελεί, η μάθηση νέων γνώσεων και η εφαρμογή τους σε πρακτικές καταστάσεις, όπως η ανάλυση δεδομένων και η δημιουργία window manager μέσω του arch linux. Τέλος, η βελτιστοποίηση της συνεργασίας και επικοινωνίας με τα υπόλοιπα μέλη της ομάδας μου αποτελεί ακόμη ένα σημαντικό στόχο για εμένα.

# ΠΑΡΑΔΟΤΕΟ 2 - Άσκηση γραμμής εντολών (archlinux+wm) 

Το πρώτο πρόβλημα που συνάντησα ήταν το wiki του arch linux, προσωπικά με δυσκόλεψε πολύ και με έκανε να καταφύγω σε αυτό το [tutorial](https://www.youtube.com/watch?v=yaThYGr37DI). Στην συνεχεία, το arch κατά την εγκατάσταση δεν έχει την δυνατότητα σύνδεσης με wifi πράγμα το οποίο με ανάγκασε να προσπαθήσω ανεπιτυχώς να εγκαταστήσω το `iwctl` και να συμβιβαστώ με ένα ethernet cable. Τέλος, το command `install-grub` δεν μου δούλευε με αποτέλεσμα να ψάχνω σε διάφορα forums για εναλλακτικά commands.


## ΤΡΟΠΟΣ ΕΓΚΑΤΑΣΤΑΣΗΣ ΒΗΜΑ-ΒΗΜΑ(ARCHLINUX)
Αρχικά, για την εγκατάσταση, έπρεπε να μετατρέψω το usb stick μου σε bootable, αυτό επιτεύχθηκε με την βοήθεια του [rufus](https://rufus.ie/en/), έπειτα κατέβασα από το [wiki](https://archlinux.org/download/) του arch το απαραίτητο iso και το πέρασα στο usb stick.

Αφού πραγματοποίησα το boot μέσω του usb stick στον υπολογιστή μου, πρόσθεσα άλλο ένα άδειο usb stick στο οποίο χρησιμοποιήθηκε για την εγκατάσταση του arch-linux. Στη συνέχεια, το usb έπρεπε να χωριστεί σε partitions για την εγκατάσταση του arch linux. Με την βοήθεια του `gdisk /dev/sda` δημιούργησα 2 partitions, ένα για το boot και ένα με τον υπόλοιπο διαθέσιμο χώρο για λειτουργικό σύστημα, μετέπειτα και τα δύο partitions έγιναν `mount`.

Έπειτα από αυτό, έκανα εγκατάσταση το πρώτο μεγάλο πακέτο(`pacstrap /mnt base base-devel linux-linux firmware vim`). Με την εντολή `arch-chroot /mnt` μπήκα σε root profile με σκοπό την εγκατάσταση του grub. Στην συνέχεια με την εντολή `timedatectl list-timezones | "enter the time zone"` πρόσθεσα την ώρα και την ημερομηνία της πόλης μου με σκοπό το σύστημα μου να είναι σωστά ενημερωμένο. Τέλος, με την εντολή `pacman -S grub` εγκατέστησα το grub και με την εντολή `pacman -S netowrkmanager`
του απαραίτητους drivers για το δίκτυο στο σύστημα μου.

Πριν κάνω reboot και τελειώσω το installation, φρόντισα να δημιουργήσω ένα προφίλ με την εντολή `vim /etc/hostname` και προσωπικό κωδικό με την εντολή `passwd`. Μετά την εκτέλεση αυτών των 2, βγήκα από το root profile με την εντολή `exit` και με την εντολή `reboot` πραγματοποίησα επανεκκίνηση στο σύστημα μου.

### ASCIINEMA VIDEOS
* [`neofetch-journalctl`](https://asciinema.org/a/zgjfOm0K8xKFlJdwyMhj8Jhtg)

## ΕΓΚΑΤΑΣΤΑΣΗ I3
Η εγκατάσταση του `WM` i3 ήταν πολύ απλή, χρησιμοποίησα την εντολή `sudo pacman -S i3` για να εγκαταστήσω τον i3. Στην συνέχεια, με την εντολή `nano -w .xinitrc` άνοιξά το αρχείο xinitrc και έγραψα την εντολή `exec i3` με σκοπό να ενεργοποιήσω στο X Window System τον i3, έπειτα έκανα reboot το σύστημα μου και για να εκκινήσω τον i3 χρησιμοποίησα την εντολή `startx`.

# ΠΑΡΑΔΟΤΕΟ 3 - Εναλλακτικό σύστημα
Για το παραδοτέο 3 επέλεξα να ασχοληθώ με το uxn varvara. To uxn varvara είναι μια εικονική μηχανή η οποία έχει το δικό της λογισμικό, τρέχει δικιά της γλώσσα προγραμματισμού και διαβάζει αρχεία `.rom`.

### Εγκατάσταση και εκτέλεση
Για να εγκαταστήσω τον εξομοιωτή, κατέβασα από το επίσημο site του uxn varvara, την έκδοση για linux και στην συνέχεια, έκανα unzip το αρχείο με την εντολή `tar xzf όνομα_αρχείου.tar.gz`. Επιπλέον χρειάστηκε να κατεβάσω και το πακέτο `libsdl2-2.0-0` για να λειτουργήσει ο εξομοιωτής.

Μετά την διαδικασία εγκατάστασης του, άνοιξα τον φάκελο με όνομα uxn με την εντολή `cd`. Ο φάκελος αυτός, πέραν του εκτελέσιμου αρχείου του εξομοιωτή, είχε και αρκετά εκτελέσιμα προγράμματα. Προσωπικά, δοκίμασα τα `calc.rom` και `nasu.rom`. Οποιδήποτε πρόγραμμα στο uxn varvara εκτελείται με την εντολή `./uxn αρχείο.rom`

![Screenshot from 2023-11-06 10-35-19](https://github.com/Axileaszervos/iv/assets/115211756/b613c7f3-fed8-411f-a70f-491c0b8d236f)

![Screenshot from 2023-11-06 10-35-37](https://github.com/Axileaszervos/iv/assets/115211756/8622bbf1-f6aa-4e96-8f48-d0df99b387ed)

# ΠΑΡΑΔΟΤΕΟ 4 - Άσκηση γραμμής εντολών (custom wm)

Για window manager επέλεξα τον `i3` και παρακάτω θα παρουσιάσω όλα τα assignments όλα τα assignments που επέλεξα για την παραμετροποίηση του window manager.

### Wallpaper
Για να αλλάξω το μαύρο φόντο που υπάρχει εξ αρχής στην επιφάνεια του i3, χρειάστηκε να εγκαταστήσω το πακέτο `feh` με το οποίο είναι εφικτή η προβολή εικόνων. Στην συνέχεια κατέβασα από το διαδίκτυο μια εικόνα της αρεσκείας μου και για να την προβάλω στην επιφάνεια του i3, χρειάστηκε να ανοίξω το αρχείο `.config/i3/config` και να προσθέσω μια νέα κατηγορία με όνομα `DISPLAY`, στην οποία τρέχω την εντολή `exec_always feh --bg-fill /home/Axileas/Downloads/Arch.jpg`.
![wallpaper](https://github.com/Axileaszervos/iv/assets/115211756/13989031-3a7c-44de-8fe2-8b56cce4b555)

### Bar
Για `status-bar` επέλεξα ένα έτοιμο theme ένα repository στο github. Πιο συγκεκριμένα, επισκέφτηκα το repository με [όνομα](https://github.com/tobi-wan-kenobi/bumblebee-status), έκανα `git clone` στον δίσκο μου το αποθετήριο με τα διαθέσιμα themes. Στην συνέχεια, άνοιξα το αρχέιο `.config/i3/config` και δημιούργησα ένα block κώδικα, στο οποίο αντέγραψα τον έτοιμο κώδικα που είχε το repository και τον προσάρμοσα στις δικές μου απαιτήσεις(αλλαγή θέσης του bar, προβολή δικών μου δεδομένων).
![status-bar](https://github.com/Axileaszervos/iv/assets/115211756/f507c068-6ae1-4be3-9192-c8f02fc9dcb3)

### Notification
Για notification manager επέλεξα τον dunst, με την εντολή `sudo pacman -S dunst` τον εγκατέστησα και με την εντολή `notify-send` μπορώ να γράψω κάτι και να το λάβω σαν ειδοποίηση. Όπως φαίνεται και στην εικόνα, όταν ενεργοποιώ τον dunst, μου εμφανίζει την κατάσταση της σύνδεσης μου.
![dunst](https://github.com/Axileaszervos/iv/assets/115211756/e7abde6b-2ebd-4d75-a871-5869f94240f7)

# ΠΑΡΑΔΟΤΕΟ 5 - Αίτημα ενσωμάτωσης
Σε αυτό το παραδοτέο, χρειάστηκε η συνεισφορά μας στην ανεπίσημη [ιστοσελίδα](https://epic-hamilton-da9ac8.netlify.app/) του ιονίου πανεπιστημίου με σκοπό, την διόρθωση των περιεχομένων της ιστοσελίδας.

## Δήλωση θέματος - [issue#1](https://github.com/ioniodi/guide/issues/1)
Αρχικά, έπρεπε να ανοίξω ένα issue στην σχετική κατηγορία του [](), με σκοπό την δήλωση της αλλαγής που επρόκειτο να πραγματοποιήσω. Στην συνέχεια, για την υλοποίηση του issue έπρεπε, ένας καθηγητής να δώσει `green light` στο issue που έχει ανοίξει.

## Η συνεισφορά μου
Στο κομμάτι της συνεισφοράς, επέλεξα να αλλάξω την κατηγόρια(RANK) του καθηγητή Εμμανουήλ Μάγκου από "Αναπληρωτή Καθηγητή" σε "Καθηγητή". Πιο συγκεκριμένα, επέλεξα να κάνω `git clone` στον υπολογιστή μου το repository με όνομα [all_collections](https://github.com/ioniodi/all_collections/tree/ea9cfa267a6879165aabc645dd5ff5fd65344d81) και έπειτα επέλεξα φάκελο `people`. Μέσα σε αυτόν, επέλεξα το αρχέιο `emagkos.md` και άλλαξα την κατηγορία rank απο 2(Αναπληρωτές Καθηγητές) σε 1(Καθηγητές).

## Pull request
Έπειτα απ το `green light`, προχώρησα σε [pull request](https://github.com/ioniodi/all_collections/pull/74), το οποίο περιείχε την αλλαγή που είχα πραγματοποιήσει.

# ΠΑΡΑΔΟΤΕΟ 6 - Άσκηση γραμμής εντολών (cli data analysis)
Για το 6ο παραδοτέο, επέλεξα να ασχοληθώ με το [pastel](https://github.com/sharkdp/pastel), το οποίο επιλέχθηκε μέσα από την πληθώρα επιλογών που είχε ο πίνακας [visualization](https://github.com/epidrome/dokey#:~:text=OpenSSH%20Cloud%20Stack-,visualization,-assignments). Το pastel είναι ένα εργαλείο για τον χρωματισμό κειμένου και δεδομένων στο τερματικό, προσφέρoντας διάφορες δυνατότητες χρωματισμού στον χρήστη, όσον αναφορά το κείμενο.

Δημιούργησα αυτό το `shell script`


    #!/bin/bash

    # define colors
    GREEN=$(tput setaf 2)
    CYAN=$(tput setaf 6)
    RESET=$(tput sgr0)

    #function print_color_message
    
    print_color_text() {
    local color="$1"       # define variables
    local message="$2"
    echo "${color}${message}${RESET}" # print the color message and reset the colors
    }

    # print the welcome message
    
    print_color_text "$CYAN" "-----------------------------------------"
    print_color_text "$CYAN" "        Welcome to My Awesome Script     "
    print_color_text "$CYAN" "-----------------------------------------"

    # print the starting messsage
    print_color_text "$GREEN" "The script is starting now..."

    sleep 3 # freeze time for 3 seconds

    echo "Hello World!"

    # print the final color message
    
    print_color_text "$CYAN" "-----------------------------------------"
    print_color_text "$CYAN" "          Script Completed!              "
    print_color_text "$CYAN" "-----------------------------------------"
    
Στο οποίο αρχικά, δηλώνω τα χρώματα που θέλω να χρησιμοποιήσω με την εντολή tput setaf colorname. Το `tput` είναι ένα εργαλείο του Unix που χρησιμοποιείται για τη διαχείριση γραφικών ρυθμίσεων στο τερματικό, όπου σε συνδυασμό με την εντολή `setaf` και την επιλογή του αριθμού χρώματος που επιλέγει ο χρήστης, δημιουργείται το εκάστοτε χρώμα. Στην συνέχεια, δημιουργείται μια συνάρτηση `print_color_text()` στην οποία δηλώνονται δύο μεταβλητές(χρώματος και κειμένου) και έπειτα, εκτυπώνονται με την εντολή `echo` και με την μεταβλητή `Reset` τα χρώματα στο τερματικό επαναφέρονται στην αρχική τους κατάσταση. Τέλος, με την εντολή `sleep`  το shellscript παγώνει για 3 δευτερόλεπτα, με σκοπό να δείχνει το script ότι κάτι φορτώνεται σε αυτό και έπειτα εκτυπώνεται το τελικό αποτέλεσμα μαζί με ένα χρωματιστό μήνυμα ολοκλήρωσης του shellscript.

* [ASCIINEMA_VIDEO]()




# ΠΑΡΑΔΟΤΕΟ 8 - Άσκηση γραμμής εντολών (cli data analysis)
Στα πλαίσια του όγδοου παραδοτέου, επιλέχθηκε απο τον πίνακα με τα διαθέσιμα shellscripts η δημιουργία ένος script το οποίο θα εμφανίζει όλα τα commits που έχουν πραγματοποιηθεί σε ένα αποθετήριο.
Πιο συγκεκρινένα, δημιούργησα αυτο το `shell script`

     #!/bin/bash

    # Set the folder path
    folder_path="/home/axileas/Desktop/iv"

    # Define the name of the file to store the results
    output_file="git_bars_output.txt"

    # Check if the folder exists
    if [ -d "$folder_path" ]; then
    echo "Folder found: $folder_path"
    
    # Change to the folder
    cd "$folder_path"
    
    # Execute git-bars and save the results to a file
    if git-bars | tee "$output_file"; then
        echo "Successful execution of git-bars."
        cat "$output_file"
    else
        echo "Error during the execution of git-bars"
      fi
    else
       echo "Folder does not exist: $folder_path"
    fi

# ΠΑΡΑΔΟΤΕΟ 9 - Αίτημα ενσωμάτωσης
