---
description: >-
  Choisir le classeur d'achat dans lequel arrivent les factures fournisseurs
  d'une maille d'adressage dans INGENEO PRECOMPTA.
---

# Choisir le classeur d'une maille d'adressage

**Résumé :** Cette procédure permet de choisir le classeur d'achat dans lequel arrivent les factures fournisseurs d'une maille d'adressage dans INGENEO PRECOMPTA. Elle prend environ 3 minutes. Elle nécessite le droit `Autoriser l'accès au paramétrage de l'entreprise.` dans le profil de site.

## Objectif

Dans INGENEO PRECOMPTA, une maille d'adressage est l'adresse de réception des factures fournisseurs issues de la PA SEPTEO. Une maille d'adressage est créée par l'enrôlement de l'entreprise.

Chaque maille d'adressage dépose ses factures dans un seul classeur d'achat. Un même classeur d'achat peut recevoir les factures de plusieurs mailles d'adressage.

Sans paramétrage, les factures d'une maille d'adressage arrivent dans le premier classeur d'achat de la liste. Utilisez cette procédure pour choisir un autre classeur d'achat.

## Prérequis

* Dans INGENEO PRECOMPTA, votre profil de site inclut le droit `Autoriser l'accès au paramétrage de l'entreprise.`.
* L'entreprise est enrôlée sur la PA SEPTEO. Sinon, l'onglet `Facturation électronique` de l'entreprise affiche `Pas d'enrôlement effectif`.
* Le classeur d'achat de destination existe dans l'entreprise.

## Étapes

1. Dans INGENEO PRECOMPTA, cliquez sur le menu `Entreprise` dans le menu de gauche.
2. Cliquez sur le bouton crayon de l'entreprise concernée.
3. Cliquez sur l'onglet `Facturation électronique`.
4. Cliquez sur l'onglet `Adresses de réception`.
5. Repérez la ligne de la maille d'adressage à paramétrer.
6. Dans la liste déroulante `Classeur d'achat associé` de cette ligne, sélectionnez le classeur d'achat de destination.
7. Si vous paramétrez d'autres mailles d'adressage, refaites le choix dans la liste `Classeur d'achat associé` de chaque ligne.
8. Cliquez sur `Enregistrer`.

## Résultat attendu

Dans INGENEO PRECOMPTA, le changement de classeur s'applique immédiatement après le clic sur `Enregistrer`. Les nouvelles factures fournisseurs de la maille d'adressage arrivent dans le classeur d'achat choisi.

Les factures déjà déposées par la maille d'adressage restent dans l'ancien classeur. Pour changer leur classeur, faites un clic droit sur chaque document. `Déplacer vers` retire la facture de son classeur d'origine. `Copier vers` laisse la facture dans son classeur d'origine et en place une copie dans le classeur choisi.

## Erreurs fréquentes

* **Anciennes factures toujours dans l'ancien classeur :** dans INGENEO PRECOMPTA, changer le classeur d'une maille d'adressage ne déplace pas les factures déjà déposées. Faites un clic droit sur chaque document, puis choisissez `Déplacer vers`.
* **Factures arrivées dans un classeur inattendu :** dans INGENEO PRECOMPTA, une maille d'adressage sans classeur choisi dépose ses factures dans le premier classeur d'achat de la liste. Choisissez le classeur dans la liste `Classeur d'achat associé`, onglet `Adresses de réception`.
* **Garder une facture dans deux classeurs :** dans INGENEO PRECOMPTA, faites un clic droit sur le document, puis choisissez `Copier vers`. La facture reste dans son classeur d'origine.
* **Seuls des classeurs d'achat sont proposés :** dans INGENEO PRECOMPTA, la liste `Classeur d'achat associé` ne propose que des classeurs d'achat. Une maille d'adressage ne peut pas déposer dans un classeur de ventes, de caisse ou de banque.
* **Message `Pas d'enrôlement effectif` :** dans INGENEO PRECOMPTA, ce message s'affiche dans l'onglet `Facturation électronique` quand l'entreprise n'est pas enrôlée sur la PA SEPTEO. Aucune maille d'adressage n'est alors disponible.
* **Maille d'adressage absente de la liste :** dans INGENEO PRECOMPTA, onglet `Adresses de réception`, cliquez sur `+ Ajouter une maille`. Renseignez les champs `Type d'identifiant d'adressage` et `Date d'effet`. Le champ `Date de fin` est facultatif.
* **Maille d'adressage à supprimer :** dans INGENEO PRECOMPTA, onglet `Adresses de réception`, cliquez sur le bouton corbeille de la ligne de la maille d'adressage.
* **Onglet `Adresses de réception` inaccessible :** dans INGENEO PRECOMPTA, le paramétrage d'une entreprise requiert le droit `Autoriser l'accès au paramétrage de l'entreprise.` dans le profil de site.

## Fiches liées

* [Comment donner les droits sur les statuts de facture ?](../administration/comment-donner-les-droits-sur-les-statuts-de-facture.md) : droits de statut sur les classeurs d'achat
* [Comment configurer les statuts de la réforme ?](comment-configurer-les-statuts-de-la-reforme.md) : autre réglage de l'onglet `Facturation électronique`
* [Classeurs & éléments comptables](classeurs-comptables.md) : création des classeurs d'une entreprise
