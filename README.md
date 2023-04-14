## PART 1:

## Aceste comenzi le vei executa o singura data:

⭐Pentru a transfera/clona/duplica datele de pe remote repsitory/GitHub pe local repository/laptop-ul tau:
```bash
git clone LINK
```
* Unde "LINK" va fi inlocuit cu link-ul SSH al proiectului pe care doresti sa il copiezi pe local repository/laptop-ul tau.

* Explicatie: (ATENTIE!) A nu se confunda cu comanda "git pull". Comanda "git clone" practic iti instaleaza proiectul, deja existent pe remote repsitory/GitHub, pe local repository/laptop-ul tau.

* OBS: In cazul de fata, totul va fi pregatit pentru lucrul cu proiectul, deci poti sari la comenzile din a doua parte a fisierului!



⭐Initializezare git:
```bash
git init
```
* Explicatie: Prin initializare Git ne referim la crearea unui fisier special pentru a lucra mai departe cu Git si pentru stocarea istoricului, practic numai asa vei putea scrie urmatoarele comenzi, aceste informatii/comenzi sunt retinute in acest fisier.


⭐Initializezare git:
```bash
git remote add origin LINK
```
* Unde "LINK" va fi inlocuit cu link-ul SSH al proiectului tau.

* Explicatie: Ii asociezi repo-ului de pe GitHub o denumire mai accesibila, aceasta fiind "origin".

---------------------------------------------------------------------------------------------------

🥳FELICITARI!
Ai reusit sa initiezi tot ce este nevoie pentru a continua modificarea proiectului.
Acum trebuie doar sa incepi sa modifici ce vrei sa modifici, apoi vei reveni la command prompt cu urmatoarele comenzi:

---------------------------------------------------------------------------------------------------

## PART 2:

⭐Pentru verificarea statusului curent:
```bash
git status
```
* Explicatie: Prin intermediul acestei comenzi vei putea accesa diverse informatii depsre starea actuala de lucru, daca proiecul este sau nu actualizat sau pe ce branch te aflii. De asemenea verifici daca sunt schimbari in local repository, adica daca exista modificari la nivelul proiectului, fata de starea sa initiala. Daca ai modificari in proiect, iti vor aparea fisierele modificate/noi cu rosu pe ecran, daca nu, toate fisierele vor fi colorate cu verde, semn ca totul e ok.



⭐Pentru adaugarea/inregistrarea modificarilor noi de-a lungul timpului:
```bash
git add .
```
* Unde "." face referire la absolut toate fisierele noi/adaugate.

SAU
```bash
git add NUME_FISIER
```
* Unde "NUME_FISIER" este numele fisierului pe car dorim sa ii inregistram modificarile.

* Explicatie: Mereu cand vei face o noua modificare, vei fi nevoit sa o inregistrezi lui git pentru a putea lucra mai departe. Practic vei adauga toate modificarile facute de tine.



⭐Pentru retinerea modificarilor facute in istoric:
```bash
git commit -m "MESAJ"
```
* Unde "MESAJ" va fi inlocuit cu un o descriere a modificarii tale. De exemplu: "Am adaugat logo-ul site-ului pe pagina principala", descriere sugestiva pentru modificarea facuta anterior.

* Explicatie: Faci commit la modificarile tale, adica creezi o eticheta schimbarilor prin care specifici ce ai schimbat prin mesajul aflat intre ghinimele, in loc de NUME vei scrie numele activitatii unde ai facut schimbarea, pentru o recunoastere mai usoara a schimbarilor

 

⭐Pentru vizualizarea commit-urilor:
```bash
git log
```
* Explicatie: Aceasta comanda iti va oferi o lista cu toate commit-urile realizate anterior.


⭐Pentru restaura/recupera fisierele sterse anterior din greseala:
```bash
git restore .
```
* Unde "." face referire la absolut toate fisierele sterse.

SAU
```bash
git restore NUME_FISIER
```
* Unde "NUME_FISIER" este numele fisierului pe car dorim sa ii restauram.

* Explicatie: Aceasta comanda este utila pentru a recupera diverse fisiere pe care le-am sters din greseala.

--------------------------------------------------------


⭐Pentru vizualizarea listei de branch-uri:
```bash
git branch
```
* Explicatie: Aceasta comanda iti va oferi o lista cu toate branch-urile create anterior si iti va evidentia pe ce branch te aflii in momentul respectiv.


⭐Pentru crearea unui branch nou:
```bash
git branch NUME
```
* Unde "NUME" este numele noului branch.

* Explicatie: Aceasta comanda iti va crea un nou branch cu numele "NUME".

* OBS: Odata cu crearea unui branch nou, vom transfera datele de pe branch-ul vechi in cel nou!


⭐Pentru transferarea de la un branch la altul:
```bash
git checkout NUME
```
* Unde "NUME" este numele branch-ului destinatie.

* Explicatie: Aceasta comanda te va transfera pe branch-ul cu numele "NUME".


⭐Pentru crearea si transferarea de la un branch la altul nou:
```bash
git checkout -b NUME
```
* Unde "NUME" este numele branch-ului destinatie/nou.

* Explicatie: Aceasta comanda va crea un branch nou cu numele "NUME" si te va transfera pe branch-ul respectiv. Practic creem o clona a branch-ului curent, dar cu un alt nume.q  

* OBS: Odata cu crearea unui branch nou, vom transfera datele de pe branch-ul vechi in cel nou!



⭐Pentru "lipirea a doua branch-uri:
```bash
git merge NUME
```
* Unde "NUME" este numele branch-ului de la care dorim sa preluam informatiile si sa le adaugam la cel curent.

* Explicatie: Aceasta comanda va lipi/concatena/adauga informatiile noi din branch-ul "NUME" la cel curent.



⭐Pentru stergerea unui branch:
```bash
git branch -d NUME
```
* Unde "NUME" este numele branch-ului pe care dorim sa-l stergem.

* Explicatie: Aceasta comanda pur si simplu va sterge branch-ul "NUME", impreuna cu toata informatia acestuia.


