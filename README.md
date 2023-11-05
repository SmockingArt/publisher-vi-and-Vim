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
|**s**|Insertion d’une ligne and delete caractere|
|**S**|Insertion d’une ligne and delete line|
|**R**|Remplacer des caractères.|

### Sortie et sauvegarde

Pour rappel, les **:** signifient que la commande se tape en ligne de commande : [Echap]+[:], saisie de la commande puis [Entrée].

|Commande|Action|
|---|---|
|**ZZ**|Sauvegarde le fichier et quitte.|
|**:q!**|Quitte sans sauvegarder (quit).|
|**:e**| Annule la session de travail (quit).|
|**:q**|Quitte si le fichier n’a pas été modifié (message d’erreur sinon).|
|**:w**|Sauvegarde le fichier. Vous pouvez préciser un nom à la suite (write).|
|**:wq** ou **:x**|Sauvegarde et quitte.|
|**:w newfile**| Sauvegarde une copie|
|**:w pathname/file**| 
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
|**~**| Changing the case of a letter Uppercase Lowercase|
|**.**| Repeating command |

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
| ctrl-R   | Annule la derniere action                     |

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

|Text object|ChangeDeleteCopy|
One word|cw|dw|yw|
Two words, not counting punctuation|2cW or c2W|2dW or d2W|2yW or y2W|
Three words back|3cb or c3b|3db or d3b|3yb or y3b|
One line|cc|dd|yy or Y|
To end of line|c$ or C|d$ or D|y$|
To beginning of line|c0|d0|y0|
Single character|r|x or X|yl or yh|
Five characters|5s|5x|5yl|

## Vim motion commands

MovementCommand
Scroll forward one screen|^F
Scroll backward one screen|^B
Scroll forward half screen|^D
Scroll backward half screen|^U
Scroll forward one line|^E
Scroll backward one line|^Y
Move current line to top of screen and scrollz ENTER
Move current line to center of screen and scrollz.
Move current line to bottom of screen and scrollz-
Redraw the screen^L
Move to home—the top line of screenH
Move to middle line of screenM
Move to bottom line of screenL
Move to first character of next lineENTER
Move to first character of next line+
Move to first character of previous line-
Move to first nonblank character of current line^
Move to column n of current linen|
Move to end of worde
Move to end of word (ignore punctuation)E
Move to beginning of current sentence(
Move to beginning of next sentence)
Move to beginning of current paragraph{
Move to beginning of next paragraph}
Move to beginning of current section[[
Move to beginning of next section]]
Search forward for pattern/pattern
Search backward for pattern?pattern
Repeat last searchn
Repeat last search in opposite directionN
Repeat last search forward/
Repeat last search backward?
Move to next occurrence of x in current linefx
Move to previous occurrence of x in current lineFx
Move to just before next occurrence of x in current linetx
Move to just after previous occurrence of x in current lineTx
Repeat previous find command in same direction;
Repeat previous find command in opposite direction,
Go to given line nnG
Go to end of fileG
Return to previous mark or context``
Return to beginning of line containing previous mark''
Show current line (not a movement command)^G

## More commands

ChangeDeleteCopyFrom cursor to...
cHdHyHTop of screen
cLdLyLBottom of screen
c+d+y+Next line
c5|d5|y5|Column 5 of current line
2c)2d)2y)Second sentence following
c{d{y{Previous paragraph
c/patternd/patterny/patternPattern
cndnynNext pattern
cGdGyGEnd of file
c13Gd13Gy13GLine number 13

## Review of vi Buffer and Marking Commands
Table 4-2 summarizes the command-line options common to all versions of vi. Tables
4-3 and 4-4 summarize the buffer and marking commands.
Table 4-2. Command-line options
OptionMeaning
+n fileOpen file at line number n.
+ fileOpen file at last line.
+/pattern fileOpen file at first occurrence of pattern (traditional version of POSIX -c).
-c command fileRun command after opening file; usually a line number or search (POSIX version of +).
-ROperate in read-only mode (same as using view instead of vi).
-rRecover files after a crash.

Buffer namesBuffer use
1–9The last nine deletions, from most to least recent.
a–zNamed buffers for you to use as needed. Uppercase letters append to the buffer.

CommandMeaning
"b commandDo command with buffer b.
mxMark current position with x.
'xMove cursor to first character of line marked by x.
`xMove cursor to character marked by x.
``Return to exact position of previous mark or context.
''Return to beginning of the line of previous mark or context.

POSIX character classes
ClassMatching characters
[:alnum:]Alphanumeric characters
[:alpha:]Alphabetic characters
[:blank:]Space and tab characters
[:cntrl:]Control characters
[:digit:]Numeric characters
[:graph:]Printable and visible (nonspace) characters
[:lower:]Lowercase characters
[:print:]Printable characters (includes whitespace)
[:punct:]Punctuation characters
[:space:]Whitespace characters
[:upper:]Uppercase characters
[:xdigit:]Hexadecimal digits

