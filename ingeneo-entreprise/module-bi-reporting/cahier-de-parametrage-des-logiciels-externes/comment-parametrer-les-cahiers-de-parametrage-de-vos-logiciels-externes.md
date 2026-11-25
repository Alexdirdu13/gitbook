# Comment paramétrer les cahiers de paramétrage de vos logiciels externes ?

## Cahier de paramétrage des logiciels externes

Une fois que vous avez sélectionné le **cahier de paramétrage des logiciels externes** depuis "Paramètres de l'espace" après avoir cliqué sur la roue crantée, vous verrez:

1. La liste de tous vos cahiers de paramétrages
2. A droite du nom de chaque cahier, vous trouverez un crayon. Il vous suffit d'appuyer sur le crayon pour accéder au cahier et pouvoir le modifier.

## Présentation du cahier

1. Dans la première colonne vous trouverez chaque identifiant unique issu de votre logiciel qui vous permettra de comprendre la nature du produit. Il s'agit soit d'un code produit, nom de produit unique, etc
2. Dans la seconde vous retrouverez les libellés de ces codes. Ce champs est utile notamment lorsque nous récupérons un code produit sous forme d'identifiant unique
3.  Dans les colonnes suivantes vous retrouverez les différents éléments que nous récupérons pour alimenter le P\&L.

    **Attention :**

    Dans cet exemple vous pouvez voir que nous récupérons 3 type de données (Montant TTC, Montant HT et montant TVA). En fonction des cahiers de paramètrages, les montants récupérés peuvent différés.

    Vous devrez ici définir les rubriques de votre P\&L en fonction du code unique.

**À savoir :**

Dans notre exemple, le code unique AC1, le champs MONTANT TTC alimentera la rubrique de votre P\&L "Chiffre d'affaires TTC". Dans ce cas, si par exemple nous récupérons 100€ de chiffre d'affaires TTC sur le code unique de transaction AC1, nous alimenterons la rubrique de votre reporting "Chiffre d'affaires TTC".

**Il est possible d'indiquer "NE PAS PRENDRE EN COMPTE" lorsque vous considérez que le montant n'est pas à prendre en compte dans votre reporting. Nous avons l'exemple ici avec le montant de TVA.**

1. Cette colonne permet d'indiquer le taux de TVA correspondant à chaque code. **Cette rubrique n'est pas toujours présente et dépend de si Qotid doit recalculer les TVA ou non.**
2. Enfin en appuyant sur ce symbole vous serez redirigé vers le cahier de paramètrage des écritures comptables. **Attention cette colonne est visible uniquement si vous avez le module de génération des écritures comptables.**

**À savoir :**

N'hésitez pas à utiliser la barre de recherche pour faire des recherches et des modifications en masse sur plusieurs lignes.

## Réalisation du paramétrage des codes

1. Pour modifier un des champs il suffit de cliquer sur le stylo
2.  Pour sélectionner la rubrique du P\&L à associer :

    a) Cliquer sur le crayon du champ souhaité

    b) Vous avez accès directement à la barre de recherche pour chercher par nom directement

    c) Sélectionner la rubrique souhaitée (le chemin parent/enfant de la rubrique est indiqué pour mieux vous y retrouver)

    d) Si vous souhaitez que ce point de donnée ne soit pas pris en compte pour cet élément vous pouvez appuyer sur "**ne pas prendre en compte**"

    e) Valider
3. En ce qui concerne le taux de TVA, si la colonne est affichée, vous aurez juste à sélectionner un des taux proposé

**Attention: vous devez remplir tous les champs pour chaque code même les codes à ne pas prendre en compte et utiliser la corbeille le cas échéant.** **Si un code à un taux de TVA à 0, Il faut également obligatoirement indiquer 0% en taux.**

**À savoir :**

Si vous ne paramètrez pas l'ensemble des rubriques correctement ainsi que la TVA le cas échéant, vous aurez des alertes dans Qotid.

## Validation de votre paramétrage

Pour valider vos modifications appuyer sur **"valider"** en haut à gauche.

**Attention :**

Si vous ne cliquez pas sur Valider et que vous quittez le cahier, vos modifications seront perdues.

**Attention :**

**Attention a bien "Valider" uniquement lorsque vous avez terminé l'ensemble de vos changements. Le système réimportera l'ensemble de vos données et modifier les historiques le cas échéants.**

## Apparition des nouveaux codes

Les nouveaux codes apparaissent tout en bas du cahier.

Si jamais un nouveau code est une erreur (erreur d'import; mauvais fichier...) tout à droite vous avez **une corbeille,** si vous cliquez dessus vous pourrez effacer le code et toute la data qui lui est liée.

**Attention :**

Vous ne devez faire cette manipulation que si un mauvais import.

Si le code est correcte mais que vous ne souhaitez pas le prendre en compte dans votre reporting il faut utiliser la méthode précédemment expliquée et utiliser le bouton "Ne pas prendre en compte"

## Se rendre facilement sur le cahier de paramétrages des écritures comptables

En appuyant sur ce symbole cela vous amènera au cahier de paramétrage des écritures comptables sur le code que vous avez sélectionné. (Voir les 2 images)

**À savoir :**

Si vous commencez à paramétrer le cahier de paramétrage des logiciels externes. Le bouton pour aller vers le cahier des écritures comptables sera grisé. **Vous devez d'abord enregistrer vos modifications avant de sortir de ce cahier.**

**À savoir :**

Nous vous conseillons toujours de commencer par paramétrer le cahier de paramétrage des écritures comptables lors de l'apparition de nouveaux codes.

**Chemin : Fin du guide**

## Fin du guide

Merci e votre lecture

**Chemin : Cahier de paramétrage des écritures comptables**

## Comment paramétrer les cahiers de paramétrages des écritures comptables de vos logiciels externes ?

Ce parcours renvoie vers le guide [Comment paramétrer les cahiers de paramétrages des écritures comptables de vos logiciels externes ?](comment-parametrer-les-cahiers-de-parametrages-des-ecritures-comptables-de-vos-logiciels-externes.md).
