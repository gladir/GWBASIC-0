# GWBASIC-0
Clone GWBASIC du DOS écrit en Pascal

![image](https://github.com/user-attachments/assets/75df72ff-a337-4f71-9678-99eeea4c16b6)

<h2>Quoi de neuf</h2>

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
	
<h2>Licence</h2>
<ul>
 <li>Le code source est publié sous la licence <a href="https://github.com/gladir/GWBASIC-0/blob/main/LICENSE">MIT</a>.</li>
 <li>Le paquet original est publié sous la licence <a href="https://github.com/gladir/GWBASIC-0/blob/main/LICENSE">MIT</a>.</li>
</ul>
