---
description: >-
  Découper, éclater, télécharger ou fusionner un document d'un classeur depuis
  le menu Bannettes d'INGENEO PRECOMPTA, avec le droit Enregistrer les
  documents.
layout:
  width: default
  title:
    visible: true
  description:
    visible: true
  tableOfContents:
    visible: true
  outline:
    visible: true
  pagination:
    visible: true
  metadata:
    visible: true
  tags:
    visible: false
  actions:
    visible: true
  anchors:
    visible: true
tags:
  - ingeneo
---

# Comment modifier un document dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de découper une zone, éclater, télécharger ou fusionner un document d'un classeur comptable depuis le menu `Bannettes` d'INGENEO PRECOMPTA. Elle nécessite le droit `Enregistrer les documents` sur le classeur.

## Objectif

Dans INGENEO PRECOMPTA, la modification d'un document se fait depuis le menu `Bannettes`, avant sa pré-saisie comptable. Elle sert à :

* découper une zone d'une page, par exemple un ticket sur une page de tickets scannés ;
* éclater un document de plusieurs pages en plusieurs documents ;
* télécharger un document au format PDF ;
* fusionner plusieurs documents en un seul ;
* corriger l'orientation d'un document scanné ou ajuster l'affichage (zoom, déplacement).

Le découpage, l'éclatement et le téléchargement se font dans l'écran `Modifier un document`. La fusion se fait uniquement depuis le classeur comptable, en sélectionnant plusieurs documents.

## Prérequis

* Dans INGENEO PRECOMPTA, l'utilisateur doit avoir le droit `Enregistrer les documents` sur le classeur comptable. Ce droit par classeur suffit pour modifier, découper, éclater, télécharger et fusionner des documents.
* Le document doit se trouver dans un classeur comptable du menu `Bannettes`, c'est-à-dire avant l'enregistrement de sa pré-saisie comptable.
* Les classeurs comptables de type `Banque` ne proposent pas ces fonctions.

## Étapes

{% hint style="warning" %}
Dans l'écran `Modifier un document` d'INGENEO PRECOMPTA, les modifications ne sont enregistrées qu'après un clic sur `Enregistrer sous...` puis sur `Valider`. Si vous fermez l'écran avant, toutes les modifications sont perdues.
{% endhint %}

### Ouvrir l'écran Modifier un document

1. Dans INGENEO PRECOMPTA, cliquez sur `Bannettes` dans le menu de gauche.
2. Sélectionnez l'entreprise dans la liste.
3. Sélectionnez le classeur comptable qui contient le document.
4. Faites un clic droit sur le document.
5. Cliquez sur `Modifier`. Le raccourci clavier `CTRL+E` ouvre le même écran.

L'écran `Modifier un document` s'ouvre et affiche les pages du document.

### Découper une ou plusieurs zones d'une page

1. Dans l'écran `Modifier un document` d'INGENEO PRECOMPTA, cliquez sur la page à découper.
2. Cliquez sur `Découper une zone`.
3. Tracez un rectangle à la souris autour de la zone à extraire.
4. Si d'autres zones de la page doivent être extraites, tracez un rectangle autour de chacune.
5. Cliquez sur `Enregistrer sous...`.
6. Dans le panneau `Enregistrer sous`, vérifiez ou modifiez le nom dans le champ `Veuillez saisir le nom du fichier`.
7. Si le document d'origine ne doit pas être conservé, activez `Mettre à la corbeille le document original.`.
8. Cliquez sur `Valider`.

Chaque zone découpée devient un document distinct, envoyé automatiquement en OCRLAD.

### Éclater un document toutes les X pages

1. Dans l'écran `Modifier un document` d'INGENEO PRECOMPTA, cliquez sur `Éclater...`.
2. Cliquez sur `Toutes les X pages`.
3. Dans le panneau `Éclater`, saisissez le nombre de pages de chaque nouveau document dans le champ `Découper toutes les X pages :`. La valeur par défaut est 1.
4. Cliquez sur `Valider`. Le panneau `Enregistrer sous` s'ouvre.
5. Dans le panneau `Enregistrer sous`, vérifiez ou modifiez le nom dans le champ `Veuillez saisir le nom du fichier`.
6. Si le document d'origine ne doit pas être conservé, activez `Mettre à la corbeille le document original.`.
7. Cliquez sur `Valider`.

Chaque nouveau document est envoyé automatiquement en OCRLAD.

### Éclater les pages sélectionnées

1. Dans l'écran `Modifier un document` d'INGENEO PRECOMPTA, sélectionnez les pages qui formeront le nouveau document.
2. Cliquez sur `Éclater...`.
3. Cliquez sur `La sélection`. Le panneau `Enregistrer sous` s'ouvre.
4. Dans le panneau `Enregistrer sous`, vérifiez ou modifiez le nom dans le champ `Veuillez saisir le nom du fichier`.
5. Si le document d'origine ne doit pas être conservé, activez `Mettre à la corbeille le document original.`.
6. Cliquez sur `Valider`.

Le nouveau document contient les pages sélectionnées et il est envoyé automatiquement en OCRLAD. Le document d'origine garde toutes ses pages, sauf si `Mettre à la corbeille le document original.` a été activé.

### Télécharger un document

1. Dans l'écran `Modifier un document` d'INGENEO PRECOMPTA, sélectionnez les pages à télécharger.
2. Cliquez sur `Télécharger la sélection`.

Le document est téléchargé au format PDF.

### Fusionner plusieurs documents

1. Dans INGENEO PRECOMPTA, cliquez sur `Bannettes` dans le menu de gauche.
2. Sélectionnez l'entreprise dans la liste.
3. Sélectionnez le classeur comptable qui contient les documents.
4. Sélectionnez les documents à fusionner. Maintenez `CTRL` pour les sélectionner un par un, ou `MAJ` pour sélectionner des documents consécutifs.
5. Faites un clic droit sur la sélection.
6. Cliquez sur `Fusionner`. L'écran `Modifier un document` s'ouvre avec les pages des documents sélectionnés.
7. Cliquez sur `Enregistrer sous...`.
8. Dans le panneau `Enregistrer sous`, vérifiez ou modifiez le nom dans le champ `Veuillez saisir le nom du fichier`.
9. Si les documents d'origine ne doivent pas être conservés, activez `Mettre à la corbeille les documents originaux.`.
10. Cliquez sur `Valider`.

## Résultat attendu

Dans le menu `Bannettes` d'INGENEO PRECOMPTA, après `Valider` dans le panneau `Enregistrer sous`, les nouveaux documents apparaissent dans le classeur comptable. Le nom proposé reprend celui du document d'origine. Exemples observés : « (page 2) » après un éclatement, « (Fusion 23-04-2025-11H57) » après une fusion.

Les documents issus d'un découpage ou d'un éclatement sont envoyés automatiquement en OCRLAD.

Sans l'option `Mettre à la corbeille le document original.` (ou `Mettre à la corbeille les documents originaux.` pour une fusion), les documents d'origine restent dans le classeur comptable. Avec l'option, ils vont à la corbeille et restent récupérables depuis le menu `Rechercher` d'INGENEO PRECOMPTA.

## Erreurs fréquentes

* **Modifications perdues.** Dans INGENEO PRECOMPTA, l'écran `Modifier un document` a été fermé avant `Enregistrer sous...` puis `Valider`. Solution : refaites les modifications, puis enregistrez-les. Pour annuler volontairement des modifications, fermez l'écran sans cliquer sur `Enregistrer sous...`.
* **`Fusionner` introuvable dans l'écran `Modifier un document`.** Dans INGENEO PRECOMPTA, la fusion ne se fait pas dans cet écran. Solution : sélectionnez plusieurs documents dans le classeur comptable du menu `Bannettes`, faites un clic droit, puis cliquez sur `Fusionner`.
* **Impossible de modifier un document.** Dans INGENEO PRECOMPTA, trois causes sont possibles : l'utilisateur n'a pas le droit `Enregistrer les documents` sur le classeur comptable ; le document n'est plus dans le menu `Bannettes`, car sa pré-saisie comptable est enregistrée ; le document est dans un classeur `Banque`. Solution : faites attribuer le droit, ou vérifiez l'emplacement du document.
* **Document d'origine mis à la corbeille par erreur.** Dans INGENEO PRECOMPTA, un document mis à la corbeille avec `Mettre à la corbeille le document original.` reste récupérable. Solution : retrouvez-le depuis le menu `Rechercher`, comme décrit dans la fiche « Rechercher un document ».

## Fiches liées

* [Rechercher un document](rechercher-un-document.md) : retrouver un document, y compris un document d'origine mis à la corbeille.
* [Déposer manuellement des documents](depot-manuel-de-document.md) : `Déposer et modifier un document` ouvre l'écran `Modifier un document` juste après le dépôt.
* [Faire la pré-saisie comptable](la-saisie-comptable.md) : étape qui suit la modification du document.
* [Détail des droits](../administration/detail-des-droits.md) : droit `Enregistrer les documents` sur les classeurs.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-modifier-document-ingeneo-precompta
* titre : Comment modifier un document dans INGENEO PRECOMPTA ?
* titre\_menu : Modifier un document
* type : procedure
* module : Gestion des documents
* version\_outil : toutes
* roles\_concernes : utilisateur avec le droit `Enregistrer les documents` sur le classeur comptable
* tags : Bannettes, Modifier un document, découper une zone, éclater, fusionner, OCRLAD
* formulations\_utilisateur : « Comment découper un ticket sur une page scannée ? » ; « Comment séparer un PDF de plusieurs pages en plusieurs documents ? » ; « Comment fusionner deux documents ? » ; « Comment remettre à l'endroit un document scanné ? » ; « J'ai perdu mes modifications sur le document »
* sources : Refonte de la page GitBook ingeneo-pre-compta/gestion-des-documents/modifier-un-document ; données des démos Arcade « Fusion de documents » (mise à jour 2026-07-24) et « Éclater les documents » ; réponses de l'expert 2026-11-05
* redacteur : CH
* relecteur :
* derniere\_verification : 2026-11-05
* statut : brouillon

</details>
