![Alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a5/Flag_of_the_United_Kingdom_%281-2%29.svg/255px-Flag_of_the_United_Kingdom_%281-2%29.svg.png)

# Scenarios in CloudSim

For the requested Assignment, click the link:  
[Assignment](Assignment/)

For the Source Code, click the link:  
[Code](cloudsim-cloudsim-4.0/)

For the detailed Documentation, click the link:  
[Documentation](Documentation/)

## Overview

This project involves the implementation of a cloud computing simulation using CloudSim. The application models a theater reservation system where clients can reserve seats for performances at Theater X. The simulation includes various components such as data centers, hosts, virtual machines (VMs), and cloudlets.

## Course Information

- **Course**: [Cloud Computing and Services](https://ice.uniwa.gr/education/undergraduate/courses/cloud-services/)
- **Semester**: 8
- **Program of Study**: [UNIWA](https://www.uniwa.gr/)
- **Department**: [Informatics and Computer Engineering](https://ice.uniwa.gr/)
- **Theory Instructors**: [Mamalis Vasileios](https://ice.uniwa.gr/emd_person/17361/)-[Kallergis Dimitrios](https://ice.uniwa.gr/emd_person/20878/)
- **Academic Season**: 2023-2024

## Student Information

- **Name**: Athanasiou Vasileios Evangelos
- **Student ID**: 19390005
- **Status**: Undergraduate

## Table of Contents

- [Theoretical Part](#theoretical-part)
  - [1. Data Centers and Hosts](#1-data-centers-and-hosts)
  - [2. Host Features](#2-host-features)
  - [3. Data Center Characteristics](#3-data-center-characteristics)
  - [4. Virtual Machines](#4-virtual-machines)
  - [5. VM Accommodation Parameters](#5-vm-accommodation-parameters)
  - [6. VM Execution Analysis](#6-vm-execution-analysis)
  - [7. Cloudlets](#7-cloudlets)
  - [8. Cloudlet Allocation](#8-cloudlet-allocation)
  - [9. Routing Policies](#9-routing-policies)
  - [10. Output Analysis](#10-output-analysis)

- [Practical Part](#practical-part)
  - [A. Testing Different Sharing Policies](#a-testing-different-sharing-policies)
  - [B. Infrastructure Changes](#b-infrastructure-changes)
  - [C. Code Modifications](#c-code-modifications)

## Theoretical Part

### 1. Data Centers and Hosts
Discussion on the creation of data centers and the number of hosts within each data center.

### 2. Host Features
Examination of the processors (PEs) in each host along with their specifications such as MIPS and memory.

### 3. Data Center Characteristics
Overview of the additional characteristics of each data center and their representation in the code.

### 4. Virtual Machines
Details on the number of VMs created and their specific characteristics.

### 5. VM Accommodation Parameters
Parameters that determine the number of VMs each host can accommodate and the allocation algorithm used.

### 6. VM Execution Analysis
Analysis of the execution of VMs, including the reasons some VMs may not be assigned to any host.

### 7. Cloudlets
Details on the creation of cloudlets and their characteristics.

### 8. Cloudlet Allocation
Discussion on the allocation of cloudlets to VMs and the factors influencing this decision.

### 9. Routing Policies
Examination of the routing policies used for assigning cloudlets to VMs and VMs to PEs.

### 10. Output Analysis
Detailed explanation of the output results, including the significance of start and end times of cloudlets.

## Practical Part

### A. Testing Different Sharing Policies
Experimentation with different space/time sharing policies for cloudlet and VM routing.

### B. Infrastructure Changes
Modification of the infrastructure to ensure all VMs can run without over-subscription, presented in three different approaches.

### C. Code Modifications
Discussion on the code changes required to implement alternative allocation policies and their potential effects on the simulation.

## Requirements

- **CloudSim Framework**: Ensure the [CloudSim 4.0 framework](https://github.com/Cloudslab/cloudsim/releases) is installed and configured.
- **Java Development Kit (JDK)**: A compatible version of JDK (8 or higher) is required.
- **IDE**: An integrated development environment (IDE) for Java development.

## Installation & Usage

### 1. Clone the Repository
Download the repository to your local machine:
```
git clone https://github.com/Cloud-Computing-and-Services/CloudSim.git
```
### 2. Open Project in IDE
Open the project in IDE for Java Development such as Eclipse

### 3. Run the example
From package `/cloudsim-examples/src/main/java/org/cloudbus/cloudsim/examples/` run `CloudSimExample6.java` to see the simulation

![Alt text](https://upload.wikimedia.org/wikipedia/commons/thumb/5/5c/Flag_of_Greece.svg/255px-Flag_of_Greece.svg.png)

# Σενάρια στο CloudSim

Για την αιτούμενη εργασία, κάντε κλικ στον σύνδεσμο:  
[Εργασία](Assignment/)

Για τον πηγαίο κώδικα, κάντε κλικ στον σύνδεσμο:  
[Κώδικας](cloudsim-cloudsim-4.0/)

Για την αναλυτική τεκμηρίωση, κάντε κλικ στον σύνδεσμο:  
[Τεκμηρίωση](Documentation/)

## Επισκόπηση

Αυτό το έργο περιλαμβάνει την υλοποίηση μιας προσομοίωσης υπολογιστικού νέφους χρησιμοποιώντας το CloudSim. Η εφαρμογή μοντελοποιεί ένα σύστημα κρατήσεων θέσεων για παραστάσεις στο Θέατρο X. Η προσομοίωση περιλαμβάνει διάφορα στοιχεία όπως κέντρα δεδομένων, κεντρικούς υπολογιστές, εικονικές μηχανές (VMs) και cloudlets.

## Πληροφορίες Μαθήματος

- **Μάθημα**: [Υπολογιστική Νέφους και Υπηρεσίες](https://ice.uniwa.gr/education/undergraduate/courses/cloud-services/)
- **Εξάμηνο**: 8
- **Πρόγραμμα Σπουδών**: [ΠΑΔΑ](https://www.uniwa.gr/)
- **Τμήμα**: [Μηχανικών Πληροφορικής και Υπολογιστών](https://ice.uniwa.gr/)
- **Διδάσκοντες Θεωρίας**: [Μαμάλης Βασίλειος](https://ice.uniwa.gr/emd_person/17361/) - [Καλλέργης Δημήτριος](https://ice.uniwa.gr/emd_person/20878/)
- **Ακαδημαϊκή Χρονιά**: 2023-2024

## Πληροφορίες Φοιτητή

- **Όνομα**: Αθανασίου Βασίλειος Ευάγγελος
- **Αριθμός Φοιτητή**: 19390005
- **Κατάσταση**: Προπτυχιακός

## Πίνακας Περιεχομένων

- [Θεωρητικό Μέρος](#θεωρητικό-μέρος)
  - [1. Κέντρα Δεδομένων και Κεντρικοί Υπολογιστές](#1-κέντρα-δεδομένων-και-κεντρικοί-υπολογιστές)
  - [2. Χαρακτηριστικά Κεντρικών Υπολογιστών](#2-χαρακτηριστικά-κεντρικών-υπολογιστών)
  - [3. Χαρακτηριστικά Κέντρου Δεδομένων](#3-χαρακτηριστικά-κέντρου-δεδομένων)
  - [4. Εικονικές Μηχανές](#4-εικονικές-μηχανές)
  - [5. Παράμετροι Φιλοξενίας VM](#5-παράμετροι-φιλοξενίας-vm)
  - [6. Ανάλυση Εκτέλεσης VM](#6-ανάλυση-εκτέλεσης-vm)
  - [7. Cloudlets](#7-cloudlets)
  - [8. Κατανομή Cloudlet](#8-κατανομή-cloudlet)
  - [9. Πολιτικές Δρομολόγησης](#9-πολιτικές-δρομολόγησης)
  - [10. Ανάλυση Εξόδου](#10-ανάλυση-εξόδου)

- [Πρακτικό Μέρος](#πρακτικό-μέρος)
  - [A. Δοκιμή Διαφορετικών Πολιτικών Κοινοχρησίας](#a-δοκιμή-διαφορετικών-πολιτικών-κοινοχρησίας)
  - [B. Αλλαγές Υποδομής](#b-αλλαγές-υποδομής)
  - [C. Τροποποιήσεις Κώδικα](#c-τροποποιήσεις-κώδικα)

## Θεωρητικό Μέρος

### 1. Κέντρα Δεδομένων και Κεντρικοί Υπολογιστές
Συζήτηση σχετικά με τη δημιουργία κέντρων δεδομένων και τον αριθμό των κεντρικών υπολογιστών σε κάθε κέντρο δεδομένων.

### 2. Χαρακτηριστικά Κεντρικών Υπολογιστών
Εξέταση των επεξεργαστών (PEs) σε κάθε κεντρικό υπολογιστή, μαζί με τις προδιαγραφές τους, όπως MIPS και μνήμη.

### 3. Χαρακτηριστικά Κέντρου Δεδομένων
Επισκόπηση των επιπλέον χαρακτηριστικών κάθε κέντρου δεδομένων και της αναπαράστασής τους στον κώδικα.

### 4. Εικονικές Μηχανές
Λεπτομέρειες σχετικά με τον αριθμό των VMs που δημιουργούνται και τα συγκεκριμένα χαρακτηριστικά τους.

### 5. Παράμετροι Φιλοξενίας VM
Παράμετροι που καθορίζουν τον αριθμό των VMs που μπορεί να φιλοξενήσει κάθε κεντρικός υπολογιστής και ο αλγόριθμος κατανομής που χρησιμοποιείται.

### 6. Ανάλυση Εκτέλεσης VM
Ανάλυση της εκτέλεσης των VMs, συμπεριλαμβανομένων των λόγων για τους οποίους ορισμένα VMs μπορεί να μην έχουν ανατεθεί σε κανένα κεντρικό υπολογιστή.

### 7. Cloudlets
Λεπτομέρειες σχετικά με τη δημιουργία cloudlets και τα χαρακτηριστικά τους.

### 8. Κατανομή Cloudlet
Συζήτηση σχετικά με την κατανομή cloudlets σε VMs και τους παράγοντες που επηρεάζουν αυτήν την απόφαση.

### 9. Πολιτικές Δρομολόγησης
Εξέταση των πολιτικών δρομολόγησης που χρησιμοποιούνται για την ανάθεση cloudlets σε VMs και VMs σε PEs.

### 10. Ανάλυση Εξόδου
Λεπτομερής εξήγηση των αποτελεσμάτων εξόδου, συμπεριλαμβανομένης της σημασίας των χρόνων έναρξης και λήξης των cloudlets.

## Πρακτικό Μέρος

### A. Δοκιμή Διαφορετικών Πολιτικών Κοινοχρησίας
Πειραματισμός με διαφορετικές πολιτικές κοινοχρησίας χώρου/χρόνου για τη δρομολόγηση cloudlet και VM.

### B. Αλλαγές Υποδομής
Τροποποίηση της υποδομής ώστε να εξασφαλιστεί ότι όλα τα VMs μπορούν να τρέξουν χωρίς υπερκάλυψη, παρουσιασμένες σε τρεις διαφορετικές προσεγγίσεις.

### C. Τροποποιήσεις Κώδικα
Συζήτηση σχετικά με τις τροποποιήσεις κώδικα που απαιτούνται για την υλοποίηση εναλλακτικών πολιτικών κατανομής και τις πιθανές επιδράσεις τους στην προσομοίωση.

## Απαιτήσεις

- **Framework CloudSim**: Βεβαιωθείτε ότι το [CloudSim 4.0 framework](https://github.com/Cloudslab/cloudsim/releases) είναι εγκατεστημένο και ρυθμισμένο.
- **Java Development Kit (JDK)**: Απαιτείται μια συμβατή έκδοση του JDK (8 ή υψηλότερη).
- **IDE**: Ένα ολοκληρωμένο περιβάλλον ανάπτυξης (IDE) για την ανάπτυξη Java.

## Εγκατάσταση & Χρήση

### 1. Κλωνοποιήστε το Αποθετήριο
Κατεβάστε το αποθετήριο στον τοπικό σας υπολογιστή:
```
git clone https://github.com/Cloud-Computing-and-Services/CloudSim.git
```
### 2. Ανοίξτε το Έργο σε IDE
Ανοίξτε το έργο σε IDE για Ανάπτυξη Java όπως το Eclipse.
### 3. Εκτελέστε το παράδειγμα
Από το πακέτο `/cloudsim-examples/src/main/java/org/cloudbus/cloudsim/examples/` εκτελέστε το `CloudSimExample6.java` για να δείτε την προσομοίωση.
