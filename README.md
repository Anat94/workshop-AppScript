# WORKSHOP Créer un Formulaire de saisie avec APP SCRIPT

## Le but de ce Workshop :

Le but est de découvrir un peu le langage Appscript developpé par Google. Mais que à la fin vous puissiez réaliser un formulaire de saisie d’information sur une feuille de calcul et stocker ces données dans une feuille de Google Sheet.

## Prérequis
Avoir à disposition un compte Google ou Microsoft pour faire ce Workshop.

## STEP 1 : Connexion

Aller sur https://docs.google.com/spreadsheets et créer une nouvelle feuille de calcul « INFO » et créér de colonne (Nom Prénom) en position A1 et B2 et en dessous mettre votre nom prénom.

<img src="https://github.com/Anat94/workshop-AppScript/blob/main/ETAPE1.png" width="300"/>

## STEP 2 : Editeur de texte Appscript

Aller sur l'onglet « EXTENSION » puis cliquer sur « Apps Scripts ».


# STEP 2.1 : Découverte d'Appscript
Pour commencer, nous allons créer une fonction qui va prendre en paramètre une variable name et qui va afficher un message dans la console de l'éditeur de texte.
Vous devez créer une deuxième fonction qui va prendre appeler la première fonction et lui passer en paramètre votre nom.

```
    Hello ${name} !
```
<img src="https://github.com/Anat94/workshop-AppScript/blob/main/ETAPE2.png" width="300"/>

- Créer une fonction ShowNumber qui prend en paramètre un nombre N et ensuite à afficher de 0 à N. ``` function ShowNumber() ```

- Créer une fonction FindElem qui prend en paramètre une liste et une string. La fonction doit afficher ***YES*** si le mot est dans la liste sinon ***NO***. `` function FindElem() ``

Example :
```
    let L = ["HELLO", "JE", "SUIS", "HOPPY"]
    findList(L, "SUIS")
```

Output : YES

- Créer une fonction additionNumList qui prend en parametre une liste de nombres et faire la somme de tous ces élements. `` function additionNumList() ``

Example :
```
    let L = [1,2,3,4,5,6,7,8,9]
    additionNumList(L)
```

Output : 45

## STEP 3 : Utiliser Appscript dans une feuille de calcul

### __3.1: Récupérer les données d'une feuille de calcul__

Créer une fonction GetInfo() qui doit récupérer votre nom et prénom depuis la feuille INFO et renvoie votre nom et prénom sur la console.

### __3.2: Ajouter les données d'une feuille de calcul__

#### __3.2.1: Ajouter les données d'une feuille de calcul

Créer une fonction ``AddHoppyName()`` qui ajoute sur la colonne "NOM" «Le chat» et "PRENOM" «Hoppy»

<img src="https://github.com/Anat94/workshop-AppScript/blob/main/ETAPE3.png" width="300"/>

#### __3.2.2: Ajouter les données d'une feuille de calcul à la ligne suivant

Créer une fonction AddName(nom, prenom) qui prend en paramètre 2 chaines de caractères (nom et prénom).
Cette fonction doit ajouter le nom et prénom à la ligne suivante.

Example : 
```
AddName("Hoopy", "Chat")
AddName("RAVENS", "BDE")
AddName("Kylian", "Mbappe")
```

Output:
```
```

### __3.3: Supprimer les données d'une feuille de calcul__

1.	Créer une fonction RemoveRow() qui doit supprimer la ligne numéro 3
2.	Ensuite, créer une fonction RemoveName(Nom) qui prend en paramètre une chaîne de caractères et devra supprimer la ligne ayant le nom associé.