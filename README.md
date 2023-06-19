# publisher-vi

---
$$Information$$

TAG :  #TableOfContents

THÉMATIQUES : Table of contents

✍ Fais par : @SmockingArt 

🧭 le : 2023-05-16 

_**Table of Contents**_ : [Saisie](#Saisie) | [Sortie et sauvegarde](#Sortie-et-sauvegarde) | [Déplacement](#Déplacement) | [Correction](#Correction) | [Recherche simple](#Recherche-simple) | [Copier-coller](#Copier-coller) | [Autres commandes](#Autres-commandes)

---

### Saisie

Les actions suivantes sont en mode commande. Elles doivent être précédées d’un appui sur [Echap] :

|Commande|Action|
|---|---|
|**a**|Ajout après le caractère courant (add).|
|**A**|Ajout de texte en fin de ligne.|
|**i**|Insertion devant le caractère courant, comme dans un traitement de texte (insert).|
|**I**|Insertion de texte en début de ligne.|
|**o**|Ajout d’une ligne sous la ligne actuelle.|
|**O**|Insertion d’une ligne au-dessus de la ligne actuelle.|
|**R**|Remplacer des caractères.|

### Sortie et sauvegarde

Pour rappel, les **:** signifient que la commande se tape en ligne de commande : [Echap]+[:], saisie de la commande puis [Entrée].

|Commande|Action|
|---|---|
|**ZZ**|Sauvegarde le fichier et quitte.|
|**:q!**|Quitte sans sauvegarder (quit).|
|**:q**|Quitte si le fichier n’a pas été modifié (message d’erreur sinon).|
|**:w**|Sauvegarde le fichier. Vous pouvez préciser un nom à la suite (write).|
|**:wq** ou **:x**|Sauvegarde et quitte.|
|**1,10w fic**|Sauvegarde les lignes de 1 à 10 dans le fichier nommé "fic".|

### Déplacement

|Commande|Action|
|---|---|
|**h** ou **[Flèche à gauche]**|Aller vers la gauche.|
|**l** (L minuscule) ou **[Flèche à droite]**|Aller vers la droite.|
|**k** ou **[Flèche en haut]**|Aller vers le haut.|
|**j** ou **[Flèche en bas]**|Aller vers le bas.|
|**0** (zéro)|Début de ligne.|
|**:0 (zéro)**|Début de fichier (première ligne).|
|**$**|Fin de ligne.|
|**:$**|Fin de fichier (dernière ligne).|
|**w**|Aller au mot suivant (word).|
|**b**|Aller au mot précédent (back).|
|**[Ctrl] f**|Avance d’un écran (Forward).|
|**[Ctrl] b**|Recule d’un écran (Backward).|
|**[Ctrl] g**|Aaffiche la position dans le fichier et l'éta de celui-ci.|
|**G**|Dernière ligne du fichier (go).|
|**nG**|Saute à la ligne « n » (ex : 10G va à la 10ème ligne).|
|**:<n>**|Idem ( :10 va à la 10ème ligne).|
|**%**| Lorsque le curseur est sur (,),[,],{,} déplace sur le caractère correspondant.|

### Correction

|Commande|Action|
|---|---|
|**x**|Efface le caractère sous le curseur.|
|**r<c>**|Remplace le caractère sous le curseur par le caractère « c ».|
|**dw**|Efface depuis le curseur jusqu’à la fin du mot (delete).|
|**d$** ou **D**|Efface depuis le curseur jusqu’à la fin de la ligne.|
|**d0** (zéro)|Efface depuis le début de la ligne jusqu’au curseur.|
|**df<c>**|Efface tout jusqu’au caractère « c » (delete find).|
|**dG**|Efface tout jusqu’à la dernière ligne, y compris la ligne actuelle.|
|**d1G**|Efface tout jusqu’à la première ligne, y compris la ligne actuelle.|
|**dd**|Efface la ligne actuelle.|
|**u**|Annule la dernière action (undo).|

Ces commandes peuvent être répétées. 5dd supprime 5 lignes, 4dw, 4 mots, 5x, 5 caractères, etc.

### Recherche simple

La commande de recherche est le caractère /. On indique ensuite le critère (la chaîne de caractères recherchée), puis on lance la recherche avec [Entrée]. La recherche démarre du caractère courant à la fin du fichier. Ainsi, /echo recherche la chaîne ’echo’ dans la suite du fichier. Quand la chaîne est trouvée, le curseur s’arrête sur le premier caractère de cette chaîne.

En appuyant sur [n] (commande n), la recherche continue. La commande N (appui sur [N]) effectue la recherche en sens inverse.

### Copier-coller

|Commande|Action|
|---|---|
|**v**|Sélection visuelle, le texte est surligné. Déplacez le curseur pour sélectionner le texte. Ensuite utilisez une des commandes suivantes.|
|**y**|Copie (yank).|
|**d**|Couper (Déplacer ou delete).|
|**c**|Couper (cut), mais vi reste en mode édition.|
|**p**|Coller (put below).|
|**u**|Annule la saisie.|
Les actions suivantes sont possibles en mode commande, sans sélection préalable :

| Commande | Description                                   |
|----------|-----------------------------------------------|
| yw       | Copier un mot.                                |
| yy       | Copier une ligne.                             |
| 5yy      | Copier cinq lignes.                           |
| dw       | Couper un mot.                                |
| dd       | Couper une ligne.                             |
| 5dd      | Couper cinq lignes.                           |
| p        | Placer les lignes copiées à un endroit donné. |

### Autres commandes

| Commande | Description                                   |
|---|---|
|**:r fic**|Insère le contenu de fic à partir de la position courante du curseur.|
|**:! cmd**|Exécute la commande. Appuyez sur [Entrée] pour revenir sous vi.|
|**:r! cmd**|Le résultat de la commande est inséré à l’endroit actuel.|

| Commande | Description                                   |
|---|---|
| :help w | |
| :help c_CTRL-D | |
| :help c_<T | |
| :help insert-index | |
| :help user-manual | |
| F1 | |

