## Structura ghidului de comenzi GIT:
* [PART 1: Comenzi destinate inițializării lucrului cu GIT](#part-1)
* [PART 2: Comenzi destinate lucrului cu repository-ul local](#part-2) 
* [PART 3: Comenzi destinate lucrului cu repository-ul remote](#part-3)
 <!--- Made by MJ: https://github.com/AndromedaOMA --->
--------------------------------------------------------------------------------
## PART 1:

✨Aceste comenzi le vei executa o singura dată✨

⭐Inițializezare git:
```bash
git init
```
* Explicație: Prin inițializare Git ne referim la crearea unui fișier special pentru a lucra mai departe cu Git și pentru stocarea istoricului, practic numai așa vei putea scrie următoarele comenzi, aceste informații/comenzi sunt reținute în acest fișier.



⭐Pentru a transfera/clona/duplica datele de pe remote repository/GitHub pe local repository/laptop-ul tău:
```bash
git clone LINK
```
* Unde "LINK" va fi înlocuit cu link-ul SSH al proiectului pe care dorești să-l copiezi pe local repository/laptop-ul tău.

* Explicație: (ATENȚIE!) A nu se confunda cu comanda "git pull". Comanda "git clone" practic îți instalează proiectul, deja existent pe remote repository/GitHub, pe local repository/laptop-ul tău.

---------------------------------------------------------------------------------------------------

🥳FELICITĂRI!

Ai reușit să inițiezi tot ce este nevoie pentru a continua modificarea proiectului.

Acum trebuie doar să începi să modifici ce vrei să modifici, apoi vei reveni la command prompt cu următoarele comenzi pentru lucrul cu repository-ul local:
 <!--- Made by MJ: https://github.com/AndromedaOMA --->
---------------------------------------------------------------------------------------------------

 * [Structura ghidului de comenzi GIT](#structura-ghidului-de-comenzi-git)

## PART 2:

⭐Pentru verificarea statusului curent:
```bash
git status
```
* Explicație: Prin intermediul acestei comenzi vei putea accesa diverse informații despre starea actuală de lucru, dacă proiectul este sau nu actualizat sau pe ce branch te afli. De asemenea, verifici dacă sunt schimbări în local repository, adică dacă există modificări la nivelul proiectului, față de starea sa inițială. Dacă ai modificări în proiect, îți vor apărea fișierele modificate/noi cu roșu pe ecran, dacă nu, toate fișierele vor fi colorate cu verde, semn că totul e ok.



⭐Pentru adăugarea/inregistrarea modificarilor noi de-a lungul timpului:
```bash
git add .
```
* Unde "." face referire la absolut toate fișierele noi/adaugate.

SAU
```bash
git add NUME_FISIER
```
* Unde "NUME_FISIER" este numele fișierului pe care dorim să îi înregistram modificările.

* Explicatie: Mereu cand vei face o nouă modificare, vei fi nevoit să o înregistrezi lui git pentru a putea lucra mai departe. Practic vei adăuga toate modificările făcute de tine.



⭐Pentru reținerea modificărilor făcute în istoric:
```bash
git commit -m "MESAJ"
```
* Unde "MESAJ" va fi înlocuit cu un o descriere a modificării tale. De exemplu: "Am adaugat logo-ul site-ului pe pagina principala", descriere sugestivă pentru modificarea făcută anterior.

* Explicație: Faci commit la modificările tale, adică creezi o etichetă schimbărilor prin care specifici ce ai schimbat prin mesajul aflat între ghinimele.

 

⭐Pentru vizualizarea commit-urilor:
```bash
git log
```
* Explicație: Această comandă iți va oferi o listă cu toate commit-urile realizate anterior.


⭐Pentru restaura/recupera fișierele șterse anterior (din greseală):
```bash
git restore .
```
* Unde "." face referire la absolut toate fișierele șterse.

SAU
```bash
git restore NUME_FISIER
```
* Unde "NUME_FISIER" este numele fișierului pe care dorim să îl restaurăm.

* Explicație: Această comandă este utilă pentru a recupera diverse fișiere pe care le-am șters (din greseală).

--------------------------------------------------------


⭐Pentru vizualizarea listei de branch-uri:
```bash
git branch
```
* Explicație: Această comandă iți va oferi o listă cu toate branch-urile create anterior si îți va evidenția pe ce branch te afli în momentul respectiv.


⭐Pentru crearea unui branch nou:
```bash
git branch NUME
```
* Unde "NUME" este numele noului branch.

* Explicație: Această comandă îți va crea un nou branch cu numele "NUME".

* OBS: Odată cu crearea unui branch nou, vom transfera datele de pe branch-ul vechi in cel nou!


⭐Pentru transferarea de la un branch la altul:
```bash
git checkout NUME
```
* Unde "NUME" este numele branch-ului destinație.

* Explicație: Această comandă te va transfera pe branch-ul cu numele "NUME".


⭐Pentru crearea ȘI transferarea de la un branch la altul nou:
```bash
git checkout -b NUME
```
* Unde "NUME" este numele branch-ului destinație/nou.

* Explicație: Această comandă va crea un branch nou cu numele "NUME" si te va transfera pe branch-ul respectiv. Practic creem o clonă a branch-ului curent, dar cu un alt nume.

* OBS: Odată cu crearea unui branch nou, vom transfera datele de pe branch-ul vechi in cel nou!



⭐Pentru "lipirea" a două branch-uri:
```bash
git merge NUME
```
* Unde "NUME" este numele branch-ului de la care dorim sa preluăm informațiile și să le adăugăm la cel curent.

* Explicație: Această comandă va lipi/concatena/adăuga informațiile noi din branch-ul "NUME" la cel curent.



⭐Pentru ștergerea unui branch:
```bash
git branch -d NUME
```
* Unde "NUME" este numele branch-ului pe care dorim să-l ștergem.

* Explicație: Această comandă pur si simplu va sterge branch-ul "NUME", împreuna cu toata informația acestuia.

---------------------------------------------------------------------------------------------------

🥳FELICITĂRI!

Ai reusit sa realizezi toate modificările necesare funcționalității proiectului tău!

Acum vom trece la treburi puțin mai serioase: lucrul cu repsitory-ul remote/GitHub. Astfel, mai departe vom folosi urmatoarele comenzi pentru lucrul cu remository-ul remote:
 <!--- Made by MJ: https://github.com/AndromedaOMA --->
---------------------------------------------------------------------------------------------------

 * [Structura ghidului de comenzi GIT](#structura-ghidului-de-comenzi-git)

## PART 3:


⭐Asociem un nume (deseori "origin") repositry-ului remote:
```bash
git remote add origin LINK
```
* Unde "LINK" va fi inlocuit cu link-ul SSH al proiectului tău.

* Explicație: Ii asociezi repo-ului de pe GitHub o denumire mai accesibilă, aceasta fiind "origin". Acest nume va fi reținut numai local, de catre repository-ul local.


⭐Pentru redenumirea ramurii curente în "main":
```bash
git branch -M main
```
* Explicație: Utilizând această comandă, se va redenumi ramura curentă a repo-ului la "main" și se va face ca toate commit-urile anterioare să aparțină de această nouă ramură principală. Acest lucru poate fi util dacă doriți să urmați practicile recomandate pentru a elimina utilizarea termenilor potențial ofensatori din proiectele tale Git.


⭐Pentru "împingerea" proiectului și ușurarea lucrului cu "git push":
```bash
git push -u origin main
```
* Explicație: Comanda "git push -u origin main" este utilizată pentru a împinge ramura curentă (în acest caz, ramura "main") în repo-ul Git remote (în acest caz, numit "origin"). Opțiunea "-u" setează ramura de urmărire pentru ramura curentă, ceea ce înseamnă că următoarele comenzi "git push" pot fi folosite fără a specifica destinația și ramura în mod explicit.



⭐Pentru a verifica dacă există diferențe între proiectul de pe repository-ul local si cel de pe repository-ul remote:
```bash
git fetch
```
* Explicație: După apelarea acestei comenzi vom afla dacă există diferențe între proiectul de pe repository-ul local si cel de pe repository-ul remote. Dacă există modificări/diferențe, atunci se vor afișa o multitudine de informații. Nu este nevoie să descifrati aceste informații, afișarea lor evidentieaza faptul că există diferențe între proiectul de pe repository-ul local si cel de pe repository-ul remote. Altfel, dacă nu se afișează nimic, atunci proiectul de pe repository-ul local este același cu cel de pe repository-ul remote.

* ATENȚIE! Există posibilitatea ca după actualizarea proiectului tău pe repository-ul local, prin comanda "git pull", să primiți o eroare de "conflicts", împreună cu locația/fișierul unde se află conflictul. Această eroare se poate rezolva prin deschiderea fișierului respectiv și remedierea situatiei prin simpla editare de cod.

  Exemplul urmator este destul de amplu. Pentru buna înțelegere a conceptului de "cofnlicts", vă sfătuiesc să urmariți cu atentie exemplul/situația următoare: Avem un fișier numit "lista_de_cumparaturi.txt" aflată în repository-ul local si remote numit "LISTA", initial goală. Persoana care deține repository-ul remote "LISTA" dorește să populeze lista, din repository-ul local, prin adaugărea unor fructe (Banane, Mere si Pere), timp în care o alta persoană, care are acces la repository-ul remote "LISTA", prin intermediul GitHub, populează lista prin adăugarea unor legume (Roșii, Ardei si Morcovi). ATENȚIE: Ambele liste sunt independente una de cealaltă! Adică prima listă, cea de fructe, incă nu a fost "împinsă" pe repository-ul remote, iar cea de-a doua listă a fost adăugată direct pe repository-ul remote. Astfel, utilizatorul care deține repository-ul "LISTA" nu va avea posibilitatea de a împinge modificările sale (prin comanda "git push") și va fi nevoit să tragă informatiile noi din repository-ul remote (prin comanda "git push"). În acest moment, proiectul său conține atât lista sa de fructe, cat și cea de legume, dar evidențiate ca fiind în conflict. Pentru rezolvarea conflictului, tot ce va mai trebui să facă acesta este să păstreze ce modificări dorește, de exemplu să renunțe la lista lui de fructe și să o păstreze pe cea de legume, considerand că nu mai are nevoie de cea cu fructe, prin stergerea acesteia, și în final să șteargă și liniile ce ajută la evidențierea conflictului (acestea sunt marcate prin: "<<<<<<<<HEAD" , "========" si ">>>>>>>> 1231ubhbeh123b1i3b123i21", la final se genereaza un cod random, deci nu vă bateti capul cu el). Acum conflictul este rezolvat, deci utilizatorul principal poate împinge noile modificări (prin comanda "git push").
  
  * [Structura ghidului de comenzi GIT](#structura-ghidului-de-comenzi-git)
  
 <!--- Made by MJ: https://github.com/AndromedaOMA --->
