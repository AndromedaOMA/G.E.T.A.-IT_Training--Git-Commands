## Structura ghidului de comenzi GIT:
* [PART 1: Comenzi destinate initializarii lucrului cu GIT](#part-1)
* [PART 2: Comenzi destinate lucrului cu repository-ul local](#part-2) 
* [PART 3: Comenzi destinate lucrului cu repository-ul remote](#part-3)

--------------------------------------------------------------------------------
## PART 1:

✨Aceste comenzi le vei executa o singura data✨

⭐Initializezare git:
```bash
git init
```
* Explicatie: Prin initializare Git ne referim la crearea unui fisier special pentru a lucra mai departe cu Git si pentru stocarea istoricului, practic numai asa vei putea scrie urmatoarele comenzi, aceste informatii/comenzi sunt retinute in acest fisier.



⭐Pentru a transfera/clona/duplica datele de pe remote repsitory/GitHub pe local repository/laptop-ul tau:
```bash
git clone LINK
```
* Unde "LINK" va fi inlocuit cu link-ul SSH al proiectului pe care doresti sa il copiezi pe local repository/laptop-ul tau.

* Explicatie: (ATENTIE!) A nu se confunda cu comanda "git pull". Comanda "git clone" practic iti instaleaza proiectul, deja existent pe remote repsitory/GitHub, pe local repository/laptop-ul tau.

---------------------------------------------------------------------------------------------------

🥳FELICITARI!

Ai reusit sa initiezi tot ce este nevoie pentru a continua modificarea proiectului.

Acum trebuie doar sa incepi sa modifici ce vrei sa modifici, apoi vei reveni la command prompt cu urmatoarele comenzi pentru lucrul cu repository-ul local:

---------------------------------------------------------------------------------------------------

* [Structura ghidului de comenzi GIT](#structura-ghidului-de-comenzi-git)

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

* Explicatie: Faci commit la modificarile tale, adica creezi o eticheta schimbarilor prin care specifici ce ai schimbat prin mesajul aflat intre ghinimele.

 

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

---------------------------------------------------------------------------------------------------

🥳FELICITARI!

Ai reusit sa realizez toate modificarile necesare functionalitatii proiectului tau!

Acum vom trece la treburi putinmai serioase: lucrul cu repsitory-ul remote/GitHub. Astfel, mai departe vom folosi urmatoarele comenzi pentru lucrul cu remository-ul remote:

---------------------------------------------------------------------------------------------------

* [Structura ghidului de comenzi GIT](#structura-ghidului-de-comenzi-git)

## PART 3:


⭐Asociem un nume (deseori "origin") repositry-ului remote:
```bash
git remote add origin LINK
```
* Unde "LINK" va fi inlocuit cu link-ul SSH al proiectului tau.

* Explicatie: Ii asociezi repo-ului de pe GitHub o denumire mai accesibila, aceasta fiind "origin".


⭐Pentru redenumirea ramurii curente in "main":
```bash
git branch -M main
```
* Explicatie: Utilizând această comandă, se va redenumi ramura curentă a repo-ului la "main" și se va face ca toate commit-urile anterioare să aparțină de această nouă ramură principală. Acest lucru poate fi util dacă doriți să urmați practicile recomandate pentru a elimina utilizarea termenilor potențial ofensatori din proiectele tale Git.


⭐Pentru impingerea proiectului si usurarea lucrului cu "git push":
```bash
git push -u origin main
```
* Explicatie: Comanda "git push -u origin main" este utilizată pentru a împinge ramura curentă (în acest caz, ramura "main") în repo-ul Git remote (în acest caz, numit "origin"). Opțiunea "-u" setează ramura de urmărire pentru ramura curentă, ceea ce înseamnă că următoarele comenzi "git push" pot fi folosite fără a specifica destinația și ramura în mod explicit.



⭐Pentru a verifica daca exista diferente intre proiectul de pe repository-ul local si cel de pe repository-ul remote:
```bash
git fetch
```
* Explicatie: Dupa apelarea acestei comenzi vom afla daca exista diferente intre proiectul de pe repository-ul local si cel de pe repository-ul remote. Daca exista modificari/diferente, atunci se vor afisa o multitudine de informatii. Nu este nevoie sa descifrati aceste informatii, afisarea lor evidentieaza faptul ca exista diferente intre proiectul de pe repository-ul local si cel de pe repository-ul remote. Altfel, daca nu se afiseaza nimic, atunci proiectul de pe repository-ul local este acelasi cu cel de pe repository-ul remote.

* ATENTIE! Exista posibilitatea ca dupa actualizarea proiectului tau pe repository-ul local, prin comanda "git pull", sa primiti o eroare de "conflicts", impreuna cu locatia/fisierul unde se afla conflictul. Aceasta eroare se poate rezolva prin deschiderea fisierului respectiv si remedierea situatiei prin simpla editare de cod.

  Exemplul urmator este destul de amplu. Pentru buna intelegere a conceptului de "cofnlicts", va sfatuiesc sa urmariti cu atentie exemplul/ situatia urmatoare: Avem un fisier numit "lista_de_cumparaturi.txt" aflata in repository-ul local si remote numit "LISTA", initial goala. Persoana care detine repository-ul remote "LISTA" doreste sa populeze lista, din repository-ul local, prin adaugarea unor fructe (Banane, Mere si Pere), timp in care o alta persoana, care are acces la repository-ul remote, prin intermediul GitHub, populeaza lista prin adaugarea unor legume (Rosii, Ardei si Morcovi). ATENTIE: Ambele liste sunt independente una de cealalta! Adica prima lista, cea de fructe, inca nu a fost impinsa pe repository-ul remote, iar cea de-a doua lista a fost adaugata direct pe repository-ul remote. Asrfel, utilizatorul care detine repository-ul "LISTA" nu va avea posibilitatea de a impinge modificarile sale (prin comanda "git push") si va fi nevoit sa traga informatiile noi din repository-ul remote (prin comanda "git push"). In acest moment, proiectul sau contine atat lista sa de fructe, cat si cea de legume, dar evidentiate ca fiind in conflict. Pentru rezolvarea conflictului, tot ce va mai trebui sa faca acesta este sa pastreze ce modificari doreste, de exemplu sa renunte la lista lui de fructe si sa o pastreze pe cea de legume, considerand ca nu mai are nevoie de cea cu fructe, prin stergerea acesteia, si in final sa stearga si liniile ce ajuta la evidentierea conflictului (acestea sunt marcate prin: "<<<<<<<<HEAD" , "========" si ">>>>>>>> 1231ubhbeh123b1i3b123i21", la final se genereaza un cod random, deci nu va bateti capul cu el). Acum conflictul este rezolvat, deci utilizatorul principal poate impinge noile modificari (prin prin comanda "git push").
  
  * [Structura ghidului de comenzi GIT](#structura-ghidului-de-comenzi-git)

