### Zadatak

**Navedeni kod zadatka potrebno je postaviti na github repozitorij ili možete napraviti vlastiti fork (gumb gore) ovog repozitorija i unutar Vašeg forka riješiti zadatak u ovoj datoteci (lv-nadoknada/zadatak). Potrebno je napraviti SQL dump Vaše baze (Tablice) i postaviti unutar git-a.**

**Da bi se zadatak smatrao ispunjenim potrebno je redovito raditi git commitove kako bi se vidio proces rada prilikom rješavanja zadatka ( projekt koji se sastoji od par commitova neće se razmatrati prilikom ispravljanja). Osim postavljenog koda zadatka potrebno je podignuti rješenje zadatka na Heroku server ili na neki drugi od Cloud servisa (ili hostanog servera) po Vašoj volji.**

#### Opis zadatka

##### Aplikacija za umrežavanje ribiča - Ribogram

1. Potrebno je strukturirati elemente prema HTML5 standardu kao i upotrebu ARIA atributa za čitaće zaslona. Također na početnoj stranici potrebno je po vlastitoj želji postaviti link za korisničku registraciju

2. Na početnoj stranici aplikacije potrebno je prikazati korisničku prijavu. Validacija mora postojati u slučaju praznih polja.
    ![01](./docs/Mask%20Group.jpg)

3. Registracija od korisnika treba tražiti sljedeće:
   1. Korisničko ime
   2. Zaporku (koju je potrebno hashirati - ne smije biti u plain tekstu)
   3. Korisnički opis
   4. Slika (Koja se pohranjuje u bazu ili u direktorij poslužitelja - a zapis putanje ide u bazu) 
   5. Potrebna je validacija u smislu praznih inputa, krivih ispunjenih podataka itd.
   ![02](./docs/Mask%20Group-7.jpg)

4. Registracijom korisnik dolazi na početni zaslon aplikacije. Unutar aplikacije u gornjem desnom kutu korisnik vidi link na svoj profil i na svoje postavke. Na zaslonu također vidi slike ostalih korisnika koje su deklarirane kao javne. Na početnoj stranici potrebno je slučajnim odabirom prikazati najviše 9 slika (ako ih ima). Korisnik može mijenjati prikaz slika na početnoj stranici - postoji mogućnost slijednog prikaza slika (jedna ispod druge s username-om korisnika slike i opisom) ili može odabrati galerijski prikaz. Klikom na sliku (u oba prikaza) korisnika se vodi na profil koji je objavio javnu sliku.
   ![03](./docs/Mask%20Group-1.jpg)
   ![04](./docs/Mask%20Group-6.jpg)


5. Korisnik na korisničkom profilu može vidjeti ostale fotografije korisnika koje su javno objavljenje. Klikom na sliku otvara mu se modal prozor (slika u proširenoj rezoluciji). Klikom izvan prostora modala sliku je potrebno zatvoriti.
 ![05](./docs/Mask%20Group-4.jpg)
 ![06](./docs/Mask%20Group-5.jpg)

6. Ako se korisnik nalazi na svome profilu - potrebno je omogućiti gumb za dodavanje svojih slika.
    ![07](./docs/Mask%20Group-2.jpg)

 6. Klikom na upload gumb potrebno je odvesti korisnika u novi izbornik gdje može postaviti sliku, opis navedene slike te status prikaza slike koji može biti javan ili privatan. Ako je slika javna, drugi korisnici mogu je vidjeti na korisnikovom profilu kao i na početnoj stranici gdje se nalaze ostale javne slike. Ako je slika privatna, jedino je korisnik na svome profilu može vidjeti - drugim korisnicima je sakrivena.
   ![08](./docs/Mask%20Group-9.jpg)

6. Nakon što je korisnik dodao novu sliku, potrebno ga je vratiti na njegov profil gdje će slika biti prikazana u donjem dijelu njegovog profila. Svaki sliku korisnik može izmijeniti ili obrisati.
   ![09](./docs/Mask%20Group-3.jpg)

7. Na settings linku korisnik otvara svoje korisničke podatke koje može izmijeniti i ažurirati.
   ![10](./docs/Mask%20Group-8.jpg)