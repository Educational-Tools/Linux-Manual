# Live USB

Αν και τα περισσότερα λειτουργικά συστήματα διατίθενται σε μορφή .iso, 
συνηθίζεται πλέον να γράφονται σε USB sticks για λόγους ταχύτητας και 
ευκολίας, αλλά και επειδή πολλοί υπολογιστές δεν έχουν πια μονάδα CD-ROM.

Υπάρχουν πολλά προγράμματα που μπορούν να δημιουργήσουν live USB sticks 
από ένα .iso image. Ακολουθήστε τις οδηγίες των σελίδων τους για να τα 
δημιουργήσετε.

## Με Ventoy (Προτείνεται)

Το [Ventoy](https://ventoy.net) είναι μία από τις καλύτερες επιλογές και 
υποστηρίζει Windows, Linux ή και MacOS. Έχει το πλεονέκτημα ότι αφού δημιουργήσετε 
ένα USB stick, στη συνέχεια μπορείτε να προσθέτετε ή να αφαιρείτε .iso αρχεία 
τοποθετώντας τα σε έναν υποφάκελο, χωρίς να χρειαστεί να ξαναφορμάρετε το stick.

([Πώς να Εγκαταστήσω το Ventoy;](https://www.pcsteps.gr/99966-multiboot-usb-%CE%BC%CE%B5-%CE%BB%CE%B5%CE%B9%CF%84%CE%BF%CF%85%CF%81%CE%B3%CE%B9%CE%BA%CE%AC-%CF%83%CF%85%CF%83%CF%84%CE%AE%CE%BC%CE%B1%CF%84%CE%B1/))

## Από Windows

Η παρακάτω επιλογή υποστηρίζεται μόνο σε Windows.

[Rufus](https://rufus.ie/)
([Σχετικό Tutorial για Οποιοδήποτε Τύπο .iso](https://www.pcsteps.gr/14678-%CE%B4%CE%B7%CE%BC%CE%B9%CE%BF%CF%85%CF%81%CE%B3%CE%AF%CE%B1-boot-usb/))

## Από Linux (Δεν Προτείνεται για Αρχάριους)

Τα παρακάτω λογισμικά εκτελούνται σε Linux και μπορούν να δημιουργήσουν live 
USB sticks για οποιοδήποτε λειτουργικό:

- [Startup Disk Creator](https://ubuntu.com/tutorials/tutorial-create-a-usb-stick-on-ubuntu)
- [Unetbootin](https://fossbytes.com/create-bootable-usb-media-from-iso-ubuntu/)
- [dd](https://fossbytes.com/create-bootable-usb-media-from-iso-ubuntu/)

## LiveUSB

Το <https://github.com/alkisg/liveusb> προηγήθηκε του ventoy και υποστηρίζει κι
αυτό προσθήκη .iso με αντιγραφή/επικόλληση. Όμως δεν έχει γραφικό interface και
δεν προτείνεται η χρήση του παρά μόνο σε λίγες περιπτώσεις που οι άλλες μέθοδοι
δεν δουλεύουν, για παράδειγμα εάν θέλουμε να ξεκινήσουμε το
[ubuntu-mate-18.04.5-desktop-i386.iso](https://cdimage.ubuntu.com/ubuntu-mate/releases/18.04/release/ubuntu-mate-18.04.5-desktop-i386.iso)
σε υπολογιστή με UEFI.
