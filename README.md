# GWBASIC-0
Clone GWBASIC du DOS écrit en Pascal  (Turbo Pascal ou Free Pascal).

![image](https://github.com/user-attachments/assets/75df72ff-a337-4f71-9678-99eeea4c16b6)

<h2>Quoi de neuf</h2>

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
