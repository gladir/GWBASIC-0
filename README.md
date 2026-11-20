# GWBASIC-0
Clone GWBASIC du DOS écrit en Pascal  (Turbo Pascal ou Free Pascal).

![image](https://github.com/user-attachments/assets/75df72ff-a337-4f71-9678-99eeea4c16b6)

<h2>Quoi de neuf</h2>

<h4>Version 0.83</h4>
<ul>
  <li>Ajout de l'instruction ENVIRON.</li>
  <li>Ajout du manuel d'utilisation (exemples, tableaux des instructions et des fonctions) dans ce fichier.</li>
</ul>

<h4>Version 0.82</h4>
<ul>
  <li>Ajout des fonctions VARPTR (y compris VARPTR(#n)) et VARPTR$.</li>
  <li>DRAW et PLAY acceptent les sous-chaînes « X »+VARPTR$(a$) et les paramètres « =variable; » ou « = »+VARPTR$(v).</li>
  <li>Ajout de DEF USR[n] et de la fonction USR[n] (Turbo Pascal seulement).</li>
  <li>Ajout de EXTERR, STICK et STRIG (services du DOS et du BIOS sous Turbo Pascal) et de IOCTL$.</li>
  <li>Ajout des fonctions LTRIM$, RTRIM$ et TRIM$ (extensions du clone).</li>
  <li>INPUT$(0) provoque maintenant « Appel de fonction illégal » comme le GW-BASIC.</li>
</ul>

<h4>Version 0.81</h4>
<ul>
  <li>Ajout des fichiers à accès direct : OPEN "R" / FOR RANDOM ... LEN=, FIELD, GET #, PUT #, LSET, RSET, LOC, LOF et EOF.</li>
  <li>Ajout de GET et PUT graphiques (format de tableau du GW-BASIC, actions PSET, PRESET, AND, OR, XOR).</li>
  <li>Ajout de VIEW, VIEW SCREEN, VIEW PRINT, WINDOW, WINDOW SCREEN, de la fonction PMAP et de POINT(n).</li>
  <li>Ajout de PALETTE et PALETTE USING.</li>
  <li>Ajout de BLOAD et BSAVE (sous Free Pascal, PEEK/POKE/BLOAD/BSAVE utilisent un segment de 64 Ko simulé).</li>
  <li>Ajout de CALL et CALLS (Turbo Pascal seulement, appel d'une routine en langage machine à DEF SEG:adresse).</li>
  <li>Ajout de COMMON ; CHAIN supporte MERGE, ALL et DELETE.</li>
  <li>Ajout de l'interception des événements : ON KEY(n), ON TIMER(n), ON COM(n), ON PEN, ON PLAY(n), ON STRIG(n) ... GOSUB, avec KEY(n), TIMER, COM(n), PEN, PLAY et STRIG ON/OFF/STOP.</li>
  <li>Ajout de WAIT ; LOCK, UNLOCK, PCOPY et LCOPY sont acceptés.</li>
  <li>Ajout des commandes CAT (comme FILES) et CLR (comme CLEAR).</li>
</ul>

<h4>Version 0.80</h4>
<ul>
  <li>Réécriture de l'évaluateur d'expressions : priorité des opérateurs conforme au GW-BASIC (^, négation, * /, \, MOD, + -, relationnels, NOT, AND, OR, XOR, EQV, IMP), types entier (%), simple (!) et double (#) précision, chaînes.</li>
  <li>Affichage des nombres identique au GW-BASIC (7 chiffres en simple précision, 16 en double, notation E/D, espace de signe).</li>
  <li>Correction du IF ... THEN ... ELSE (ELSE imbriqués, numéro de ligne après THEN/ELSE, IF ... GOTO).</li>
  <li>Support complet de DIM et des tableaux (plusieurs dimensions, dimension implicite de 10, OPTION BASE, ERASE, « Indice hors limites », « Définition en double »).</li>
  <li>Les lignes sont converties en jetons comme le GW-BASIC (LIST affiche les mots réservés en majuscules).</li>
  <li>Ajout de FOR/NEXT avec STEP, WHILE/WEND, ON ... GOTO/GOSUB, DATA/READ/RESTORE, INPUT, LINE INPUT, DEF FN, DEFINT/DEFSNG/DEFDBL/DEFSTR, SWAP, MID$ en affectation, ON ERROR GOTO, RESUME, ERROR, ERR, ERL, STOP/CONT, RENUM, DELETE, MERGE, CHAIN, PRINT USING, WRITE, fichiers séquentiels (OPEN, CLOSE, PRINT #, WRITE #, INPUT #, LINE INPUT #, EOF), RANDOMIZE et RND (même suite que le GW-BASIC), PSET, PRESET, PAINT, PLAY, SOUND.</li>
  <li>Ajout des fonctions manquantes (LEFT$, RIGHT$, MID$, STR$, STRING$, SPACE$, HEX$, OCT$, INSTR, INKEY$, INPUT$, CINT, CSNG, CDBL, SGN, TIMER, DATE$, TIME$, MKI$/CVI, MKS$/CVS, MKD$/CVD, ...).</li>
  <li>Messages d'erreur numérotés comme ceux du GW-BASIC (ERR) avec le numéro de ligne.</li>
</ul>

<h4>Version 0.73</h4>
<ul>
  <li>Ajout du support de la commande EDIT.</li>
  <li>Corrige le bogue pour n'écrasant pas une ligne existante si elle le même numéro.</li>
  <li>Ajout des raccourcis clavier de Alt+A (AUTO), Alt+B (NEXT), Alt+P (PRINT),...</li>
</ul>

<h4>Version 0.72</h4>
<ul>
  <li>Ajout du support de la commande DRAW.</li>
  <li>Ajout du support de l'opérateur d'exposant.</li>
  <li>Fixe le bogue effectant une variable LongInt plutôt qu'une variable réel, lorsque le nombre est à virgule flottante.</li>
  <li>Fixe le bogue que le ne change pas de type de données les variantes lorsqu'on fixe une nouvelle valeurs.</li>
  <li>Fixe le bogue des pertes de décimales pour les variables # et !.</li>
</ul>

<h4>Version 0.71</h4>
<ul>
  <li>Ajout du support de la commande AUTO avec son arrêt par Ctrl+C.</li>
  <li>Ajout du support de la commande KILL et NAME.</li>
  <li>Ajout du support de la commande LPRINT.</li>
  <li>Ajout du support de la commande CLEAR.</li>
  <li>Fixe le bogue n'effacant pas les anciennes variables lorsqu'il lance la commande RUN.</li>
  <li>Fixe le bogue qu'il perd l'affichage des touches de fonctions lors de l'utilisation de la commande CLS.</li>
</ul>

<h4>Version 0.70</h4>
<ul>
  <li>Ajout du paramètre --version.</li>
  <li>Ajout du support du chargement du format compressé du GW-BASIC (encodage avec jetons).</li>
  <li>Ajout du support de la suppression d'une ligne de code source en tapant son numéro.</li>
  <li>Ajout des commandes SCREEN, CIRCLE et LINE.</li>
  <li>Amélioration des paramètres de la commande LIST et LLIST pour supporter les intervalles.</li>
</ul>


<h2>Manuel d'utilisation</h2>

<h3>Démarrage</h3>

Pour lancer l'interpréteur, tapez simplement :

```
GWBASIC
```

Pour charger et exécuter directement un programme BASIC (l'extension `.BAS` est ajoutée si elle est absente) :

```
GWBASIC JEU.BAS
```

L'écran affiche alors le message d'accueil suivi de l'invite `Ok`. La dernière ligne de l'écran rappelle le rôle des touches de fonction (`KEY OFF` la fait disparaître). Pour quitter l'interpréteur, tapez `SYSTEM`.

<h3>Mode direct et mode programme</h3>

Une ligne tapée **sans numéro** est exécutée immédiatement (mode direct). C'est pratique pour faire des calculs ou essayer une instruction :

```
PRINT "Bonjour"
Bonjour
Ok
PRINT 2+3*4, 10/3, 2^10
 14            3.333333      1024
Ok
A$="GW":PRINT A$+"-BASIC";LEN(A$)
GW-BASIC 2
Ok
```

Une ligne tapée **avec un numéro** (0 à 65529) n'est pas exécutée : elle est rangée dans le programme en mémoire, triée selon son numéro. On exécute ensuite le programme avec `RUN` et on l'affiche avec `LIST` :

```
10 REM Table de multiplication
20 INPUT "Quelle table";N
30 FOR I=1 TO 5
40 PRINT N;"x";I;"=";N*I
50 NEXT I
RUN
Quelle table? 7
 7 x 1 = 7
 7 x 2 = 14
 7 x 3 = 21
 7 x 4 = 28
 7 x 5 = 35
Ok
```

Comme dans le GW-BASIC, les mots réservés et les noms de variables peuvent être tapés en minuscules : `LIST` les affiche en majuscules. Plusieurs instructions peuvent être écrites sur une même ligne en les séparant par `:`. Le point d'interrogation `?` est un raccourci pour `PRINT`. Les mots réservés doivent être séparés des noms de variables par un espace ou un symbole (`FOR I=1 TO 10` et non `FORI=1TO10`).

<h3>Modifier un programme</h3>

* Pour **remplacer** une ligne, retapez-la avec le même numéro.
* Pour **supprimer** une ligne, tapez seulement son numéro ; `DELETE 100-200` supprime un intervalle.
* `EDIT 30` affiche la ligne 30 pour la corriger. Après une erreur de syntaxe dans un programme, la ligne fautive est aussi affichée automatiquement pour être corrigée.
* `AUTO 100,10` numérote automatiquement les lignes tapées (100, 110, 120...). Appuyez sur **Ctrl+C** pour arrêter.
* `RENUM` renumérote le programme de 10 en 10 et met à jour les `GOTO`, `GOSUB`, `THEN`, `ELSE`, `RESTORE`, `RESUME` et `RUN`.
* `NEW` efface le programme et toutes les variables.

```
AUTO 100,10
100 PRINT "UN"
110 PRINT "DEUX"
120 PRINT "TROIS"
130                      <- Ctrl+C
110 PRINT "2"
LIST
100 PRINT "UN"
110 PRINT "2"
120 PRINT "TROIS"
Ok
RENUM
Ok
DELETE 30
Ok
LIST
10 PRINT "UN"
20 PRINT "2"
Ok
```

Touches de l'éditeur de ligne :

| Touche | Action |
|--------|--------|
| ← → Début Fin | Déplacer le curseur dans la ligne |
| Retour arrière, Suppr | Effacer le caractère avant ou sous le curseur |
| Inser | Basculer entre le mode remplacement (par défaut) et le mode insertion |
| Échap | Effacer toute la ligne |
| F1 à F10 | Insérer le texte de la touche (`LIST`, `RUN`, `LOAD"`, `SAVE"`, `CONT`, ...), modifiable par `KEY n,chaîne$` |
| Alt+lettre | Insérer un mot réservé (Alt+P = `PRINT`, Alt+F = `FOR`, Alt+G = `GOTO`, Alt+I = `INPUT`, ...) |
| Ctrl+C | Interrompre la saisie, `AUTO` ou le programme en cours (`CONT` permet de reprendre) |

<h3>Sauvegarder et charger</h3>

```
SAVE "CHAINES"
Ok
NEW
Ok
LOAD "CHAINES"
Ok
RUN "CHAINES"
```

`SAVE` écrit toujours le programme en texte (ASCII), lisible avec n'importe quel éditeur. `LOAD`, `RUN`, `MERGE` et `CHAIN` acceptent les fichiers texte ainsi que les fichiers `.BAS` sauvegardés en format binaire (jetons) par le vrai GW-BASIC. `FILES` affiche la liste des fichiers.

<h3>Exemples commentés</h3>

Chacun de ces exemples peut être tapé tel quel ; la sortie affichée est celle produite par l'interpréteur.

**1. Conditions avec `IF ... THEN ... ELSE`**

```
10 FOR I=1 TO 4
20 IF I MOD 2=0 THEN PRINT I;"est pair" ELSE PRINT I;"est impair"
30 NEXT I
RUN
 1 est impair
 2 est pair
 3 est impair
 4 est pair
```

Les nombres positifs sont précédés d'un espace (réservé au signe) et suivis d'un espace, exactement comme dans le GW-BASIC.

**2. Tableaux, `READ`/`DATA` et `PRINT USING`**

```
10 DIM NOTE(4)
20 FOR I=0 TO 4
30 READ NOTE(I):S=S+NOTE(I)
40 IF NOTE(I)>M THEN M=NOTE(I)
50 NEXT I
60 PRINT "Moyenne :";S/5
70 PRINT USING "Meilleure note : ##.#";M
80 DATA 12,15.5,9,18,14
RUN
Moyenne : 13.7
Meilleure note : 18.0
```

`DIM NOTE(4)` crée un tableau de 5 éléments (indices 0 à 4, ou 1 à 4 après `OPTION BASE 1`). Un tableau utilisé sans `DIM` est créé automatiquement avec 11 éléments (indices 0 à 10).

**3. Sous-programme (`GOSUB`) et fonction utilisateur (`DEF FN`)**

```
10 DEF FNC(F)=(F-32)*5/9
20 FOR F=32 TO 212 STEP 60
30 GOSUB 100
40 NEXT F
50 END
100 PRINT USING "### F = ###.# C";F;FNC(F)
110 RETURN
RUN
 32 F =   0.0 C
 92 F =  33.3 C
152 F =  66.7 C
212 F = 100.0 C
```

**4. Chaînes de caractères**

```
10 S$="BONJOUR LE MONDE"
20 PRINT LEFT$(S$,7);"|";MID$(S$,9,2);"|";RIGHT$(S$,5)
30 PRINT INSTR(S$,"LE");LEN(S$);ASC(S$);CHR$(65);STR$(3.5);VAL("12")+1
RUN
BONJOUR|LE|MONDE
 9  16  66 A 3.5 13
```

**5. Fichiers**

```
10 OPEN "O",#1,"AMIS.TXT"
20 WRITE #1,"Paul",34
30 WRITE #1,"Marie",29
40 CLOSE #1
50 OPEN "I",#1,"AMIS.TXT"
60 WHILE NOT EOF(1)
70 INPUT #1,N$,A
80 PRINT N$;" a";A;"ans"
90 WEND
100 CLOSE #1
RUN
Paul a 34 ans
Marie a 29 ans
```

Le fichier `AMIS.TXT` contient alors `"Paul",34` et `"Marie",29`. Les fichiers à accès direct s'utilisent avec `OPEN "R"`, `FIELD`, `LSET`/`RSET`, `PUT` et `GET`.

**6. Interception des erreurs**

```
10 ON ERROR GOTO 100
20 INPUT "Nombre";X
30 R=SQR(X)
40 PRINT "Racine :";R
50 END
100 PRINT "Erreur";ERR;"a la ligne";ERL
110 RESUME 20
RUN
Nombre? -4
Erreur 5 a la ligne 30
Nombre? 16
Racine : 4
```

Sans `ON ERROR`, le programme s'arrête et affiche le message, par exemple `Appel de fonction illégal à la ligne 30`. Comme dans le GW-BASIC, la division par zéro et le dépassement de capacité en virgule flottante affichent seulement un avertissement et l'exécution continue :

```
10 PRINT "Debut"
20 PRINT 10/0
30 PRINT "Suite"
RUN
Debut
Division par zéro
 1.701412E+38
Suite
```

**7. Graphiques**

```
10 SCREEN 1
20 LINE (10,10)-(310,190),3,B
30 CIRCLE (160,100),50,1
40 PAINT (160,100),2,1
50 DRAW "BM200,150 C3 U20 R20 D20 L20"
60 IF INKEY$="" THEN 60
70 SCREEN 0
```

Ce programme passe en mode graphique 320×200, trace un cadre, un cercle rempli et un carré, puis attend une touche avant de revenir en mode texte. Les coordonnées sont celles du mode GW-BASIC choisi (`SCREEN 1` : 320×200, `SCREEN 2` : 640×200, `SCREEN 9` : 640×350) ; elles sont mises à l'échelle de l'écran VGA. Sous Turbo Pascal, le fichier `EGAVGA.BGI` doit se trouver dans le répertoire courant.

<h3>Types de données et opérateurs</h3>

| Suffixe | Type | Exemple |
|---------|------|---------|
| `%` | Entier (-32768 à 32767) | `A%=5` |
| `!` | Simple précision (7 chiffres, par défaut) | `A!=1.5` ou `A=1.5` |
| `#` | Double précision (16 chiffres) | `A#=1/3#` |
| `$` | Chaîne de caractères (255 caractères au maximum) | `A$="BONJOUR"` |

Le type par défaut d'une variable sans suffixe peut être changé avec `DEFINT`, `DEFSNG`, `DEFDBL` et `DEFSTR`. Les constantes peuvent aussi s'écrire en hexadécimal (`&HFF`) ou en octal (`&O17`).

Les opérateurs sont évalués dans l'ordre de priorité suivant (du plus prioritaire au moins prioritaire) :

| Priorité | Opérateurs |
|----------|------------|
| 1 | `^` (puissance) |
| 2 | `-` (négation) |
| 3 | `*` `/` |
| 4 | `\` (division entière) |
| 5 | `MOD` |
| 6 | `+` `-` (et `+` pour concaténer des chaînes) |
| 7 | `=` `<>` `<` `>` `<=` `>=` (vrai = -1, faux = 0) |
| 8 | `NOT` |
| 9 | `AND` |
| 10 | `OR` |
| 11 | `XOR` |
| 12 | `EQV` |
| 13 | `IMP` |

Ainsi `-2^2` vaut -4 et `2^3^2` vaut 64, comme dans le GW-BASIC.

<h3>Messages d'erreur</h3>

Les erreurs portent les mêmes numéros que dans le GW-BASIC (valeur de `ERR`) ; les messages sont en français. Les plus courants :

| Code | Message |
|------|---------|
| 1 | NEXT sans FOR |
| 2 | Erreur de syntaxe |
| 3 | RETURN sans GOSUB |
| 4 | Plus de DATA |
| 5 | Appel de fonction illégal |
| 6 | Dépassement de capacité |
| 7 | Mémoire insuffisante |
| 8 | Numéro de ligne indéfini |
| 9 | Indice hors limites |
| 10 | Définition en double |
| 11 | Division par zéro |
| 13 | Types incompatibles |
| 15 | Chaîne trop longue |
| 18 | Fonction utilisateur non définie |
| 26 | FOR sans NEXT |
| 29 | WHILE sans WEND |
| 30 | WEND sans WHILE |
| 52 | Mauvais numéro de fichier |
| 53 | Fichier introuvable |
| 54 | Mauvais mode de fichier |
| 62 | Lecture au-delà de la fin |

<h3>Instructions et commandes</h3>

Notation : les éléments entre crochets `[ ]` sont facultatifs, `{A|B}` signifie A ou B.

| Syntaxe | Description |
|---------|-------------|
| `AUTO [ligne][,incrément]` | Cette procédure permet de numéroter automatiquement les lignes tapées au clavier (Ctrl+C pour arrêter). |
| `BEEP` | Cette procédure permet d'émettre un bip sonore. |
| `BLOAD fichier$[,déplacement]` | Cette procédure permet de charger en mémoire, au segment défini par `DEF SEG`, une image sauvegardée par `BSAVE`. |
| `BSAVE fichier$,déplacement,longueur` | Cette procédure permet de sauvegarder une zone de mémoire dans un fichier. |
| `CALL variable[(argument,...)]` | Cette procédure permet d'appeler une routine en langage machine située à l'adresse `DEF SEG`:variable, en lui passant le déplacement de chaque argument (Turbo Pascal seulement). |
| `CALLS variable[(argument,...)]` | Cette procédure permet d'appeler une routine en langage machine en lui passant l'adresse complète (segment et déplacement) de chaque argument (Turbo Pascal seulement). |
| `CAT` | Cette procédure permet d'afficher la liste des fichiers, comme `FILES` (extension du clone). |
| `CHAIN [MERGE] fichier$[,[ligne][,[ALL][,DELETE début-fin]]]` | Cette procédure permet de charger et d'exécuter un autre programme en lui transmettant les variables déclarées par `COMMON` (toutes avec `ALL`) ; `MERGE` ajoute le programme à celui en mémoire. |
| `CHDIR chemin$` | Cette procédure permet de changer le répertoire courant. |
| `CIRCLE [STEP](x,y),rayon[,[couleur][,[début],[fin][,aspect]]]` | Cette procédure permet de tracer un cercle, une ellipse ou un arc (angles en radians). |
| `CLEAR [,[mémoire][,pile]]` | Cette procédure permet d'effacer toutes les variables, les tableaux et les fonctions `DEF FN`, et de fermer les fichiers. |
| `CLOSE [[#]n[,[#]n...]]` | Cette procédure permet de fermer les fichiers indiqués, ou tous les fichiers. |
| `CLR` | Cette procédure permet d'effacer les variables, comme `CLEAR` (extension du clone). |
| `CLS` | Cette procédure permet d'effacer l'écran (ou la fenêtre graphique définie par `VIEW`). |
| `COLOR [avant][,[fond][,bordure]]` | Cette procédure permet de choisir les couleurs du texte et du fond (en `SCREEN 1` : `COLOR fond,palette`). |
| `COM(n) {ON\|OFF\|STOP}` | Cette procédure permet d'activer ou de suspendre l'interception des événements du port série n (accepté, aucun événement n'est produit). |
| `COMMON variable[,tableau()...]` | Cette procédure permet de déclarer les variables transmises au programme appelé par `CHAIN`. |
| `CONT` | Cette procédure permet de reprendre l'exécution après `STOP`, `END` ou Ctrl+C. |
| `DATA constante[,constante...]` | Cette procédure permet de déclarer des données lues par `READ`. |
| `DATE$ = chaîne$` | Cette procédure permet de changer la date du système (`mm-jj-aaaa`). |
| `DEF FNnom[(paramètre,...)] = expression` | Cette procédure permet de définir une fonction utilisateur d'une ligne. |
| `DEF SEG [= segment]` | Cette procédure permet de définir le segment utilisé par `PEEK`, `POKE`, `BLOAD`, `BSAVE`, `CALL` et `USR`. |
| `DEF USR[n] = déplacement` | Cette procédure permet de définir l'adresse de la routine en langage machine `USR`n. |
| `{DEFINT\|DEFSNG\|DEFDBL\|DEFSTR} lettre[-lettre][,...]` | Cette procédure permet de définir le type par défaut des variables selon leur première lettre. |
| `DELETE [début][-[fin]]` | Cette procédure permet de supprimer des lignes du programme. |
| `DIM tableau(max[,max...])[,...]` | Cette procédure permet de dimensionner un tableau (jusqu'à 8 dimensions). |
| `DRAW chaîne$` | Cette procédure permet de dessiner avec le macro-langage graphique (`U D L R E F G H M B N C S A X`). |
| `EDIT ligne` | Cette procédure permet d'afficher une ligne du programme pour la modifier. |
| `END` | Cette procédure permet de terminer le programme et de fermer tous les fichiers. |
| `ENVIRON "NOM=valeur"` | Cette procédure permet de définir une variable d'environnement, consultable par `ENVIRON$`. |
| `ERASE tableau[,tableau...]` | Cette procédure permet de supprimer des tableaux. |
| `ERROR code` | Cette procédure permet de provoquer l'erreur de numéro code. |
| `FIELD #n,largeur AS variable$[,...]` | Cette procédure permet de découper le tampon d'un fichier à accès direct en champs. |
| `FILES [masque$]` | Cette procédure permet d'afficher la liste des fichiers et l'espace libre. |
| `FOR variable = début TO fin [STEP pas]` | Cette procédure permet de commencer une boucle terminée par `NEXT`. |
| `GET #n[,enregistrement]` | Cette procédure permet de lire un enregistrement d'un fichier à accès direct. |
| `GET [STEP](x1,y1)-[STEP](x2,y2),tableau` | Cette procédure permet de copier une zone de l'écran graphique dans un tableau. |
| `GOSUB ligne` | Cette procédure permet d'appeler un sous-programme terminé par `RETURN`. |
| `GOTO ligne` | Cette procédure permet de poursuivre l'exécution à la ligne indiquée. |
| `HELP` | Cette procédure permet d'afficher la liste des mots réservés (extension du clone). |
| `IF condition THEN {instructions\|ligne} [ELSE {instructions\|ligne}]` | Cette procédure permet d'exécuter des instructions selon une condition ; `IF condition GOTO ligne` est aussi accepté. |
| `INPUT[;] ["invite"{;\|,}] variable[,variable...]` | Cette procédure permet de lire des valeurs au clavier. |
| `INPUT #n,variable[,variable...]` | Cette procédure permet de lire des valeurs dans un fichier séquentiel. |
| `IOCTL #n,chaîne$` | Cette procédure permet d'envoyer une chaîne de contrôle à un périphérique (impossible sur un fichier disque). |
| `KEY {ON\|OFF\|LIST}` | Cette procédure permet d'afficher, de masquer ou de lister les touches de fonction. |
| `KEY n,chaîne$` | Cette procédure permet de définir le texte de la touche de fonction n (1 à 10). |
| `KEY(n) {ON\|OFF\|STOP}` | Cette procédure permet d'activer ou de suspendre l'interception de la touche n (1 à 10 = F1 à F10, 11 à 14 = flèches). |
| `KILL fichier$` | Cette procédure permet de supprimer des fichiers (caractères génériques acceptés). |
| `[LET] variable = expression` | Cette procédure permet d'affecter une valeur à une variable. |
| `LINE [[STEP](x1,y1)]-[STEP](x2,y2)[,[couleur][,B[F]]]` | Cette procédure permet de tracer une ligne, un rectangle (`B`) ou un rectangle plein (`BF`). |
| `LINE INPUT[;] ["invite";]variable$` | Cette procédure permet de lire une ligne entière au clavier, virgules comprises. |
| `LINE INPUT #n,variable$` | Cette procédure permet de lire une ligne entière dans un fichier. |
| `LIST [début][-[fin]]` | Cette procédure permet d'afficher le programme. |
| `LLIST [début][-[fin]]` | Cette procédure permet d'imprimer le programme. |
| `LOAD fichier$[,R]` | Cette procédure permet de charger un programme (et de l'exécuter avec `R`). |
| `LOCATE [ligne][,[colonne]]` | Cette procédure permet de placer le curseur. |
| `LOCK`, `UNLOCK`, `LCOPY`, `PCOPY`, `MOTOR` | Ces procédures sont acceptées pour la compatibilité, sans effet. |
| `LPRINT [USING format$;] liste` | Cette procédure permet d'écrire sur l'imprimante. |
| `LSET variable$ = chaîne$` | Cette procédure permet de placer une chaîne à gauche d'un champ (complétée par des espaces). |
| `MERGE fichier$` | Cette procédure permet d'ajouter les lignes d'un programme texte à celui en mémoire. |
| `MID$(variable$,début[,longueur]) = chaîne$` | Cette procédure permet de remplacer une partie d'une chaîne. |
| `MKDIR chemin$` | Cette procédure permet de créer un répertoire. |
| `NAME ancien$ AS nouveau$` | Cette procédure permet de renommer un fichier. |
| `NEW` | Cette procédure permet d'effacer le programme et les variables. |
| `NEXT [variable[,variable...]]` | Cette procédure permet de terminer une boucle `FOR`. |
| `ON expression {GOTO\|GOSUB} ligne[,ligne...]` | Cette procédure permet de sauter à la ligne choisie selon la valeur de l'expression. |
| `ON ERROR GOTO ligne` | Cette procédure permet d'intercepter les erreurs (`ON ERROR GOTO 0` désactive l'interception). |
| `ON {KEY(n)\|TIMER(secondes)\|COM(n)\|PEN\|PLAY(n)\|STRIG(n)} GOSUB ligne` | Cette procédure permet de définir le sous-programme appelé lors d'un événement. |
| `OPEN fichier$ FOR {INPUT\|OUTPUT\|APPEND\|RANDOM} AS [#]n [LEN=longueur]` | Cette procédure permet d'ouvrir un fichier (aussi `OPEN mode$,[#]n,fichier$[,longueur]` avec mode `I`, `O`, `A` ou `R`). |
| `OPTION BASE {0\|1}` | Cette procédure permet de choisir le premier indice des tableaux. |
| `OUT port,valeur` | Cette procédure permet d'écrire un octet sur un port d'entrée-sortie. |
| `PAINT [STEP](x,y)[,[couleur][,bordure]]` | Cette procédure permet de remplir une zone fermée. |
| `PALETTE [attribut,couleur]` | Cette procédure permet de changer une couleur de la palette (sans paramètre : palette par défaut). |
| `PALETTE USING tableau%(indice)` | Cette procédure permet de changer les 16 couleurs de la palette d'après un tableau. |
| `PEN {ON\|OFF\|STOP}` | Cette procédure permet d'activer l'interception du crayon optique (accepté, aucun événement n'est produit). |
| `PLAY chaîne$` | Cette procédure permet de jouer de la musique avec le macro-langage musical (`A`-`G`, `O`, `L`, `T`, `N`, `P`, `M`, `<`, `>`, `X`). |
| `PLAY {ON\|OFF\|STOP}` | Cette procédure permet de contrôler l'interception de la musique en arrière-plan. |
| `POKE adresse,valeur` | Cette procédure permet d'écrire un octet en mémoire (segment `DEF SEG`). |
| `PRESET [STEP](x,y)[,couleur]` | Cette procédure permet d'allumer un point dans la couleur de fond (ou la couleur indiquée). |
| `PRINT [USING format$;] liste` (ou `?`) | Cette procédure permet d'afficher des valeurs à l'écran (`;` les colle, `,` passe à la zone suivante de 14 colonnes). |
| `PRINT #n,[USING format$;] liste` | Cette procédure permet d'écrire dans un fichier séquentiel. |
| `PSET [STEP](x,y)[,couleur]` | Cette procédure permet d'allumer un point. |
| `PUT #n[,enregistrement]` | Cette procédure permet d'écrire un enregistrement dans un fichier à accès direct. |
| `PUT [STEP](x,y),tableau[,{PSET\|PRESET\|AND\|OR\|XOR}]` | Cette procédure permet d'afficher une image obtenue par `GET` graphique. |
| `RANDOMIZE [germe]` | Cette procédure permet d'initialiser le générateur aléatoire (la valeur est demandée si elle est omise). |
| `READ variable[,variable...]` | Cette procédure permet de lire les valeurs des lignes `DATA`. |
| `REM texte` (ou `' texte`) | Cette procédure permet d'écrire un commentaire. |
| `RENUM [nouveau][,[ancien][,pas]]` | Cette procédure permet de renuméroter les lignes du programme. |
| `RESET` | Cette procédure permet de fermer tous les fichiers. |
| `RESTORE [ligne]` | Cette procédure permet de relire les `DATA` depuis le début ou depuis la ligne indiquée. |
| `RESUME [0\|NEXT\|ligne]` | Cette procédure permet de reprendre l'exécution à la fin d'un sous-programme d'erreur. |
| `RETURN [ligne]` | Cette procédure permet de revenir d'un sous-programme appelé par `GOSUB`. |
| `RMDIR chemin$` | Cette procédure permet de supprimer un répertoire vide. |
| `RSET variable$ = chaîne$` | Cette procédure permet de placer une chaîne à droite d'un champ (précédée d'espaces). |
| `RUN [ligne\|fichier$[,R]]` | Cette procédure permet d'exécuter le programme en mémoire ou de charger et d'exécuter un fichier. |
| `SAVE fichier$[,A\|,P]` | Cette procédure permet de sauvegarder le programme (toujours en texte). |
| `SCREEN mode` | Cette procédure permet de choisir le mode d'écran : 0 (texte), 1 (320×200, 4 couleurs), 2 (640×200), 7, 8 et 9 (EGA). |
| `SHELL [commande$]` | Cette procédure permet d'exécuter une commande du système d'exploitation. |
| `SLEEP [secondes]` | Cette procédure permet de faire une pause (extension du clone). |
| `SOUND fréquence,durée` | Cette procédure permet de produire un son (durée en battements d'horloge, 18,2 par seconde). |
| `STOP` | Cette procédure permet d'arrêter le programme en affichant le numéro de ligne (`CONT` pour reprendre). |
| `STRIG(n) {ON\|OFF\|STOP}` | Cette procédure permet de contrôler l'interception des boutons de la manette de jeu (accepté, aucun événement n'est produit). |
| `SWAP variable1,variable2` | Cette procédure permet d'échanger le contenu de deux variables de même type. |
| `SYSTEM` | Cette procédure permet de quitter l'interpréteur. |
| `TIME$ = chaîne$` | Cette procédure permet de changer l'heure du système (`hh:mm:ss`). |
| `TIMER {ON\|OFF\|STOP}` | Cette procédure permet de contrôler l'interception de la minuterie définie par `ON TIMER`. |
| `TRON`, `TROFF` | Ces procédures permettent d'activer ou de désactiver l'affichage des numéros de lignes exécutées. |
| `VIEW [[SCREEN](x1,y1)-(x2,y2)[,[couleur][,bordure]]]` | Cette procédure permet de définir une fenêtre graphique (sans paramètre : écran complet). |
| `VIEW PRINT [haut TO bas]` | Cette procédure permet de limiter le défilement du texte aux lignes indiquées. |
| `WAIT port,masque[,inversion]` | Cette procédure permet d'attendre qu'un bit d'un port d'entrée-sortie change d'état. |
| `WHILE condition` ... `WEND` | Cette procédure permet de répéter des instructions tant que la condition est vraie. |
| `WIDTH {40\|80}` | Cette procédure permet de choisir 40 ou 80 colonnes. |
| `WINDOW [[SCREEN](x1,y1)-(x2,y2)]` | Cette procédure permet de définir un système de coordonnées graphiques personnalisé. |
| `WRITE [#n,] liste` | Cette procédure permet d'écrire des valeurs séparées par des virgules, les chaînes entre guillemets. |

<h3>Fonctions</h3>

| Syntaxe | Description |
|---------|-------------|
| `ABS(x)` | Cette fonction retourne la valeur absolue de x. |
| `ASC(chaîne$)` | Cette fonction retourne le code ASCII du premier caractère de la chaîne. |
| `ATN(x)` | Cette fonction retourne l'arc tangente de x, en radians. |
| `CDBL(x)` | Cette fonction retourne x converti en double précision. |
| `CHR$(code)` | Cette fonction retourne le caractère correspondant au code ASCII. |
| `CINT(x)` | Cette fonction retourne x arrondi en entier (-32768 à 32767). |
| `COS(x)` | Cette fonction retourne le cosinus de x (en radians). |
| `CSNG(x)` | Cette fonction retourne x converti en simple précision. |
| `CSRLIN` | Cette fonction retourne la ligne où se trouve le curseur. |
| `CVI(chaîne$)`, `CVS(chaîne$)`, `CVD(chaîne$)` | Ces fonctions retournent le nombre entier, simple ou double précision contenu dans une chaîne de 2, 4 ou 8 octets (format binaire Microsoft). |
| `DATE$` | Cette fonction retourne la date du système (`mm-jj-aaaa`). |
| `ENVIRON$({nom$\|n})` | Cette fonction retourne la valeur d'une variable d'environnement, ou la n-ième entrée `NOM=valeur`. |
| `EOF(n)` | Cette fonction retourne -1 si la fin du fichier n est atteinte, sinon 0. |
| `ERDEV`, `ERDEV$` | Ces fonctions retournent le code et le nom du périphérique en erreur (toujours 0 et une chaîne vide). |
| `ERL` | Cette fonction retourne le numéro de la ligne où s'est produite la dernière erreur. |
| `ERR` | Cette fonction retourne le code de la dernière erreur. |
| `EXP(x)` | Cette fonction retourne e (2,718282) élevé à la puissance x. |
| `EXTERR(n)` | Cette fonction retourne l'information d'erreur étendue du DOS (n = 0 à 3, Turbo Pascal seulement). |
| `FIX(x)` | Cette fonction retourne la partie entière de x, sans arrondir. |
| `FNnom[(arguments)]` | Cette fonction retourne la valeur d'une fonction définie par `DEF FN`. |
| `FRE(x)` | Cette fonction retourne la quantité de mémoire libre. |
| `HEX$(x)` | Cette fonction retourne la représentation hexadécimale de x. |
| `INKEY$` | Cette fonction retourne la touche enfoncée, ou une chaîne vide (sans attendre). |
| `INP(port)` | Cette fonction retourne l'octet lu sur un port d'entrée-sortie. |
| `INPUT$(n[,[#]fichier])` | Cette fonction retourne n caractères lus au clavier (sans écho) ou dans un fichier. |
| `INSTR([début,]chaîne$,recherche$)` | Cette fonction retourne la position de recherche$ dans chaîne$, ou 0. |
| `INT(x)` | Cette fonction retourne le plus grand entier inférieur ou égal à x. |
| `IOCTL$([#]n)` | Cette fonction retourne la chaîne de contrôle d'un périphérique (impossible sur un fichier disque). |
| `LEFT$(chaîne$,n)` | Cette fonction retourne les n premiers caractères de la chaîne. |
| `LEN(chaîne$)` | Cette fonction retourne la longueur de la chaîne. |
| `LOC(n)` | Cette fonction retourne la position courante dans le fichier n (numéro d'enregistrement en accès direct). |
| `LOF(n)` | Cette fonction retourne la taille du fichier n en octets. |
| `LOG(x)` | Cette fonction retourne le logarithme naturel de x. |
| `LPOS(n)` | Cette fonction retourne la position de la tête d'impression. |
| `LTRIM$(chaîne$)` | Cette fonction retourne la chaîne sans ses espaces de gauche (extension du clone). |
| `MID$(chaîne$,début[,longueur])` | Cette fonction retourne une partie de la chaîne. |
| `MKI$(x)`, `MKS$(x)`, `MKD$(x)` | Ces fonctions retournent un nombre converti en chaîne de 2, 4 ou 8 octets, pour les fichiers à accès direct. |
| `OCT$(x)` | Cette fonction retourne la représentation octale de x. |
| `PEEK(adresse)` | Cette fonction retourne l'octet lu en mémoire (segment `DEF SEG`). |
| `PEN(n)` | Cette fonction retourne l'état du crayon optique (toujours 0). |
| `PLAY(n)` | Cette fonction retourne le nombre de notes en attente dans la file musicale (toujours 0). |
| `PMAP(coordonnée,n)` | Cette fonction retourne une coordonnée convertie entre le système de `WINDOW` et l'écran (n = 0 à 3). |
| `POINT(x,y)` | Cette fonction retourne la couleur du point (x,y) ; `POINT(n)` retourne la position courante du curseur graphique. |
| `POS(n)` | Cette fonction retourne la colonne où se trouve le curseur. |
| `RIGHT$(chaîne$,n)` | Cette fonction retourne les n derniers caractères de la chaîne. |
| `RND[(x)]` | Cette fonction retourne un nombre aléatoire entre 0 et 1 (même suite que le GW-BASIC). |
| `RTRIM$(chaîne$)` | Cette fonction retourne la chaîne sans ses espaces de droite (extension du clone). |
| `SCREEN(ligne,colonne[,z])` | Cette fonction retourne le code du caractère affiché à cette position (ou son attribut si z est non nul). |
| `SGN(x)` | Cette fonction retourne 1, 0 ou -1 selon le signe de x. |
| `SIN(x)` | Cette fonction retourne le sinus de x (en radians). |
| `SPACE$(n)` | Cette fonction retourne une chaîne de n espaces. |
| `SPC(n)` | Cette fonction permet, dans `PRINT`, d'afficher n espaces. |
| `SQR(x)` | Cette fonction retourne la racine carrée de x. |
| `STICK(n)` | Cette fonction retourne une coordonnée de la manette de jeu (Turbo Pascal seulement). |
| `STR$(x)` | Cette fonction retourne le nombre converti en chaîne, tel que `PRINT` l'affiche. |
| `STRIG(n)` | Cette fonction retourne -1 si le bouton n de la manette de jeu est enfoncé (Turbo Pascal seulement). |
| `STRING$(n,{caractère$\|code})` | Cette fonction retourne une chaîne formée de n fois le même caractère. |
| `TAB(n)` | Cette fonction permet, dans `PRINT`, de se placer à la colonne n. |
| `TAN(x)` | Cette fonction retourne la tangente de x (en radians). |
| `TIME$` | Cette fonction retourne l'heure du système (`hh:mm:ss`). |
| `TIMER` | Cette fonction retourne le nombre de secondes écoulées depuis minuit. |
| `TRIM$(chaîne$)` | Cette fonction retourne la chaîne sans ses espaces de gauche et de droite (extension du clone). |
| `USR[n](x)` | Cette fonction retourne le résultat d'une routine en langage machine définie par `DEF USR` (Turbo Pascal seulement). |
| `VAL(chaîne$)` | Cette fonction retourne la valeur numérique d'une chaîne. |
| `VARPTR(variable)`, `VARPTR(#n)` | Cette fonction retourne un identifiant de l'adresse d'une variable ou d'un fichier. |
| `VARPTR$(variable)` | Cette fonction retourne une chaîne de 3 octets désignant une variable, utilisable dans `DRAW` et `PLAY` (`"X"+VARPTR$(a$)`, `"="+VARPTR$(n)`). |

<h3>Différences avec le GW-BASIC</h3>

* Les messages d'erreur sont en français, avec les mêmes numéros d'erreur.
* `SAVE` sauvegarde toujours en texte ; les fichiers binaires du GW-BASIC peuvent cependant être chargés.
* Les instructions graphiques utilisent l'écran VGA 640×480 : les coordonnées des modes du GW-BASIC sont mises à l'échelle.
* Sous Free Pascal, `PEEK`, `POKE`, `BLOAD` et `BSAVE` agissent sur un segment de 64 Ko simulé, et `CALL`, `CALLS`, `USR`, `STICK`, `STRIG` et `EXTERR` ne sont pas disponibles.
* `VARPTR` retourne un identifiant et non une adresse réelle : `PEEK(VARPTR(A))` ne lit pas la valeur de A.
* Les événements `COM`, `PEN`, `PLAY` et `STRIG` sont acceptés mais ne se produisent jamais ; `PLAY` et `SOUND` jouent la musique en avant-plan.
* `ENVIRON` modifie l'environnement vu par `ENVIRON$`, mais pas celui transmis aux programmes lancés par `SHELL`.

<h2>Compilation</h2>
	
Les fichiers Pascal n'ont aucune dépendances, il suffit de télécharger le fichier désiré et de le compiler avec Free Pascal avec la syntaxe de commande  :

<pre><b>fpc</b> GWBASIC.PAS</pre>
	
Sinon, vous pouvez également le compiler avec le Turbo Pascal à l'aide de la syntaxe de commande suivante :	

<pre><b>tpc</b> GWBASIC.PAS</pre>

Le code du programme principal tient dans un seul segment de 64 Ko sous Turbo Pascal 7.

Remarque : sous Linux, l'unité PtcGraph de Free Pascal exige que l'unité <b>cthreads</b> soit la première de la clause Uses, sinon le programme s'arrête au démarrage (erreur 211).
	
<h2>Licence</h2>
<ul>
 <li>Le code source est publié sous la licence <a href="https://github.com/gladir/GWBASIC-0/blob/main/LICENSE">MIT</a>.</li>
 <li>Le paquet original est publié sous la licence <a href="https://github.com/gladir/GWBASIC-0/blob/main/LICENSE">MIT</a>.</li>
</ul>
