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


## STEP 3 : Découverte d'Appscript
Pour commencer, nous allons créer une fonction qui va prendre en paramètre une variable name et qui va afficher un message dans la console de l'éditeur de texte.
Vous devez créer une deuxième fonction qui va prendre appeler la première fonction et lui passer en paramètre votre nom.

```
    Hello ${name} !
```
<img src="https://github.com/Anat94/workshop-AppScript/blob/main/ETAPE2.png" width="300"/>