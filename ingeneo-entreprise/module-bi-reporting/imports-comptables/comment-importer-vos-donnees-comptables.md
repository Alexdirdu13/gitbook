# Comment importer vos données comptables ?

## Préambule

Pour importer manuellement vos données comptables, dans un premier temps, vous devez télécharger depuis votre logiciel comptable votre **grand livre comptable** au format CSV UTF-8 et avec un format de date "Date Courte" sous Excel. Par exemple : le format 12/01/2019 est accepté alors que 12/01/19 n'est pas accepté par Qotid.

Pour cela deux possibilités :

* Vous pouvez paramétrer le bon format de date lors des exports directement depuis votre logiciel comptable.
* Vous pouvez également faire la manipulation sur Excel directement.

Nous vous expliquons cela dans les prochaines étapes.

## Modifier la date au format date courte

Pour convertir la date de votre fichier en format "Date Courte", ouvrez votre fichier sous Excel, sélectionnez la colonne puis choisissez le format Date Courte.

## Enregistrer sous au format UTF-8

Une fois la date au bon format, vous pouvez aisément enregistrer votre Excel au format CSV UTF-8 (délimité par des virgules) en sélectionnant **Enregistrer Sous** puis en choisissant le format de fichier "**CSV UTF-8 (délimité par des virgules)"**.

## Comment importer votre grand livre comptable ?

Une fois votre grand livre téléchargé au bon format, retournez sur Qotid :

1/ Cliquez sur "**Données**" puis "**Comptabilité**".

2/ Cliquez sur "**Importer un fichier**".

3/ Sélectionnez dans votre répertoire, le grand livre comptable que vous venez de télécharger. La fenêtre présente ici à gauche va s'afficher :

4/ Sur les colonnes récupérées par Qotid, lors de la première intégration le logiciel reconnaîtra automatiquement les colonnes Débit, Crédit, Date, Libellé et N° de Compte. Si ce n'est pas le cas, vous pouvez manuellement définir la colonne en cliquant sur la première ligne (encadré rouge ci-dessous).

5/ Cliquez sur "**Importer le fichier**".

**Attention :**

Veuillez faire attention que la date affichée soit bien au format 01/01/2022.

## Attention aux doublons des données

Si vous insérez 2 fois consécutivement un fichier contenant les mêmes écritures comptables, **vos données seront affichées en doublon** dans QOTID.

Avant d'insérer votre fichier comptable, assurez vous donc de ne pas avoir déjà importé des données sur cette période.

## Fin du guide

## Comment éviter les doublons lors de l'import de vos données comptables ?

Consultez également le guide [Comment éviter les doublons lors de l'import de vos données comptables ?](comment-supprimer-vos-donnees-comptables-et-eviter-les-doublons-lors-de-limport-de-vos-donnees-comp.md).
