---
description: >-
  Déposer un ou plusieurs documents dans un classeur depuis le menu Bannettes
  d'INGENEO PRECOMPTA, avec le droit Déposer des documents. Traitement OCRLAD :
  quelques secondes à plusieurs minutes.
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

# Comment déposer manuellement des documents dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de déposer manuellement un ou plusieurs documents dans un classeur d'une entreprise, depuis le menu `Bannettes` d'INGENEO PRECOMPTA. Elle nécessite le droit `Déposer des documents` sur le classeur. Le traitement OCRLAD dure de quelques secondes à plusieurs minutes.

## Objectif

Dans INGENEO PRECOMPTA, le dépôt manuel envoie des fichiers de l'ordinateur dans un classeur d'une entreprise, depuis le menu `Bannettes`. Il sert au dépôt ponctuel, d'un fichier ou de plusieurs fichiers en une fois.

Le bouton `Ajouter` du menu `Bannettes` propose deux choix :

* `Déposer des documents` : dépôt d'un ou plusieurs fichiers.
* `Déposer et modifier un document` : dépôt d'un seul fichier, puis modification du document déposé (découper une zone, éclater, rotation).

Pour recevoir des documents en continu sans action manuelle, INGENEO PRECOMPTA propose des canaux de collecte : mail dédié, Google Drive, Dropbox, OneDrive, SharePoint et DématBox.

## Prérequis

* Dans INGENEO PRECOMPTA, l'utilisateur doit avoir le droit `Déposer des documents` sur le classeur (catégorie `Droits sur les classeurs` > `Traitements`). Ce droit suffit aussi pour ajouter un commentaire au dépôt et pour utiliser `Déposer et modifier un document`.
* Le dépôt est possible dans tous les types de classeurs.
* Un classeur `Banque` n'accepte que les fichiers CFONB, OFX et QIF. Les options de découpage automatique et d'OCRLAD n'y sont pas proposées.
* Pour les autres classeurs, les fichiers ZIP et Excel sont refusés. \[À VÉRIFIER : liste exacte des formats de fichiers acceptés par le dépôt manuel dans les classeurs autres que `Banque`.]
* Un même dépôt est limité, pour toutes les entreprises et toutes les offres, à :
  * 50 fichiers (`Nombre maximum de fichiers`) ;
  * 1024 Mo au total pour l'ensemble des fichiers (`Taille maximale`) ;
  * 250 pages par document (`Nombre de pages maximum pour un document`).
* Le nombre de documents déposés n'est pas limité par entreprise. L'enregistrement des documents peut l'être selon le type de dossier (dossier faible volume : 150 documents enregistrés par année civile) et selon l'offre.

## Étapes

### Déposer un ou plusieurs documents

1. Dans INGENEO PRECOMPTA, cliquez sur `Bannettes` dans le menu de gauche.
2. Sélectionnez l'entreprise dans la liste.
3. Sélectionnez le classeur qui doit recevoir les documents.
4. Cliquez sur `Ajouter`.
5. Cliquez sur `Déposer des documents`.
6. Dans l'explorateur de fichiers, sélectionnez un ou plusieurs fichiers.
7. Cliquez sur `Ouvrir`.
8. Dans le panneau de dépôt, vérifiez la liste des fichiers et les volumes affichés (`Taille totale actuelle`, `Nombre total de fichiers actuel`).
9. Si un fichier ne doit pas être déposé, cliquez sur la croix rouge de sa ligne.
10. Si un PDF contient plusieurs factures qui ne doivent pas être séparées, sélectionnez `Désactiver le découpage automatique` sur sa ligne.
11. Si le découpage automatique ne doit s'appliquer à aucun fichier, sélectionnez `Désactiver pour tous les fichiers`.
12. Si un document ne doit pas être océrisé, sélectionnez `Ne pas envoyer en OCRLAD` sur sa ligne.
13. Si vous voulez joindre un commentaire à un document, cliquez sur la bulle de discussion bleue de sa ligne.
14. Rédigez le commentaire dans le panneau de dépôt.
15. Cliquez sur `Valider le dépôt`.

Dans le menu `Bannettes` d'INGENEO PRECOMPTA, les fichiers peuvent aussi être glissés-déposés depuis l'ordinateur, sans passer par l'explorateur de fichiers.

### Déposer un document puis le modifier

1. Dans INGENEO PRECOMPTA, cliquez sur `Bannettes` dans le menu de gauche.
2. Sélectionnez l'entreprise dans la liste.
3. Sélectionnez le classeur qui doit recevoir le document.
4. Cliquez sur `Ajouter`.
5. Cliquez sur `Déposer et modifier un document`.
6. Dans l'explorateur de fichiers, sélectionnez un seul fichier.
7. Cliquez sur `Ouvrir`.
8. Dans le panneau de dépôt, réglez les options du fichier (`Désactiver le découpage automatique`, `Ne pas envoyer en OCRLAD`, commentaire).
9. Cliquez sur `Valider le dépôt`.
10. Modifiez le document dans l'écran d'édition. C'est le même écran que pour modifier un document déjà déposé : découper une zone, éclater, rotation.

### Options du panneau de dépôt

Dans le panneau de dépôt du menu `Bannettes` d'INGENEO PRECOMPTA, chaque fichier propose les options suivantes :

| Option                                | Effet                                                                                                                                                            |
| ------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Désactiver le découpage automatique` | Le découpage automatique sépare en plusieurs documents les factures contenues dans un même PDF. Il est actif par défaut. Cette option le retire pour le fichier. |
| `Désactiver pour tous les fichiers`   | Retire le découpage automatique pour tous les fichiers du dépôt.                                                                                                 |
| `Ne pas envoyer en OCRLAD`            | Le document est déposé brut : il n'est ni océrisé ni analysé, donc sans reconnaissance.                                                                          |
| Croix rouge                           | Retire le fichier de la liste avant le dépôt.                                                                                                                    |
| Bulle de discussion bleue             | Ajoute un commentaire au document.                                                                                                                               |

Le message `Le découpage automatique est actif sur ce classeur` indique que le classeur découpe les PDF par défaut. Pour désactiver le découpage automatique de façon permanente, ouvrez le panneau `Editer un classeur comptable`, onglet `Paramétrage avancé`, bloc `DÉPÔT DE DOCUMENT`, interrupteur `Activer le découpage automatique`.

## Résultat attendu

Dans le menu `Bannettes` d'INGENEO PRECOMPTA, après `Valider le dépôt`, chaque fichier déposé apparaît dans le classeur sur une ligne à son nom. Une roue de chargement s'affiche pendant le traitement OCRLAD.

Ce traitement dure de quelques secondes à plusieurs minutes. La durée dépend de la connexion internet, du volume déposé et de la qualité du fichier.

À la fin du traitement, un indicateur de qualité de reconnaissance remplace la roue de chargement. La légende des indicateurs s'ouvre avec l'icône `i` de la colonne des entreprises du menu `Bannettes`.

Si un commentaire a été ajouté au dépôt, l'indicateur `Le document contient un commentaire` apparaît. Le commentaire est visible dans la section `Notes` du document.

## Erreurs fréquentes

* **Format de fichier refusé.** Dans le panneau de dépôt du menu `Bannettes` d'INGENEO PRECOMPTA, le message `Le format de fichier .mp4 n’est pas autorisé. Veuillez choisir un format supporté.` s'affiche, avec l'extension du fichier concerné. Cause : le format n'est pas accepté, par exemple un ZIP ou un fichier Excel. Solution : convertissez le fichier dans un format accepté, puis déposez-le de nouveau.
* **Limite de dépôt dépassée.** Dans le panneau de dépôt, l'encadré des volumes autorisés passe en rouge et le dépôt est bloqué. Cause : plus de 50 fichiers, plus de 1024 Mo au total, ou un document de plus de 250 pages. Solution : retirez des fichiers avec la croix rouge, ou répartissez-les sur plusieurs dépôts.
* **Fichier refusé dans un classeur `Banque`.** Un classeur `Banque` n'accepte que les fichiers CFONB, OFX et QIF. Solution : déposez les autres documents dans un classeur d'un autre type.
* **Document mal reconnu après le traitement OCRLAD.** La qualité du fichier d'origine influe sur la reconnaissance. Solution : vérifiez la qualité du fichier d'origine (lisibilité, résolution du scan).
* **Factures séparées à tort, ou PDF non découpé.** Le découpage automatique, actif par défaut, sépare les factures d'un même PDF. Solution : au dépôt, sélectionnez ou non `Désactiver le découpage automatique` sur la ligne du fichier.

## Fiches liées

* [Modifier un document](modifier-un-document.md) : écran d'édition ouvert par `Déposer et modifier un document` (découper une zone, éclater, rotation).
* [Classeurs comptables](../gestion-des-entreprises/classeurs-comptables.md) : interrupteur `Activer le découpage automatique` du bloc `DÉPÔT DE DOCUMENT`.
* [Détail des droits](../administration/detail-des-droits.md) : droit `Déposer des documents` sur les classeurs.
* [Collecte automatique](../collecte-automatique/) : canaux de collecte pour recevoir des documents sans dépôt manuel ([Mail dédié](../collecte-automatique/parametrage-mail-dedie.md), [Google Drive](../collecte-automatique/parametrage-google-drive.md), [Dropbox](../collecte-automatique/parametrage-dropbox.md), [OneDrive](../collecte-automatique/parametrage-onedrive.md), [SharePoint](../collecte-automatique/parametrage-sharepoint.md)).

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-deposer-documents-manuellement-ingeneo-precompta
* titre : Comment déposer manuellement des documents dans INGENEO PRECOMPTA ?
* titre\_menu : Déposer manuellement des documents
* type : procedure
* module : Gestion des documents
* version\_outil : toutes
* roles\_concernes : utilisateur avec le droit `Déposer des documents`
* tags : dépôt, Bannettes, OCRLAD, découpage automatique, classeur, commentaire
* formulations\_utilisateur : « Comment ajouter une facture dans un classeur ? » ; « Comment déposer plusieurs documents en une fois ? » ; « Je n'arrive pas à déposer mon fichier ZIP » ; « Mon PDF de plusieurs factures a été découpé » ; « Le document tourne en chargement après le dépôt »
* sources : Refonte de la page GitBook ingeneo-pre-compta/gestion-des-documents/depot-manuel-de-document ; données de la démo Arcade « Déposer un document » (mise à jour 2026-07-24) ; FAQ GitBook (section Gestion des Documents) ; page « Détail des droits » ; réponses de l'expert 2026-10-15
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-15
* statut : brouillon

</details>
