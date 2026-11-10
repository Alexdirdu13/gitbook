---
description: >-
  Valider ou refuser un document en attente dans un circuit de validation
  d'INGENEO PRECOMPTA. Rôle Valideur requis, aucun droit de profil.
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

# Comment valider ou refuser un document dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet à un utilisateur `Valideur` d'un circuit de validation de valider ou de refuser un document dans INGENEO PRECOMPTA. Elle ne nécessite aucun droit de profil : l'utilisateur doit être créé dans INGENEO PRECOMPTA et avoir le rôle `Valideur` dans le circuit.

## Objectif

Dans INGENEO PRECOMPTA, un circuit de validation fait respecter un processus d'approbation structuré avant la finalisation d'un document. Le `Valideur` valide ou refuse chaque document qui attend son action, à son niveau du circuit.

Utilisez cette procédure quand vous êtes `Valideur` dans un circuit de validation d'INGENEO PRECOMPTA et qu'un document attend votre validation.

Dans INGENEO PRECOMPTA, chaque document se valide individuellement. Aucune validation en masse n'existe, y compris depuis la page `Documents à valider`.

## Prérequis

* Rôle : dans INGENEO PRECOMPTA, seul un utilisateur avec le rôle `Valideur` dans un circuit de validation valide des documents.
* Droits : aucun droit de profil n'est nécessaire. L'utilisateur doit seulement être créé comme utilisateur dans INGENEO PRECOMPTA.
* Étape du circuit : le document doit être arrivé à l'étape du circuit de validation où l'utilisateur est `Valideur`.
* Refus : dans INGENEO PRECOMPTA, le bouton `Refuser` ne s'affiche que si l'interrupteur `Refuser` est activé pour l'utilisateur, dans le bloc `ETAPES` du circuit de validation.

## Étapes

### Ouvrir un document à valider depuis le Tableau de bord

Dans INGENEO PRECOMPTA, le `Tableau de bord` affiche un raccourci orange `Document en attente de validation`. Ce raccourci affiche le nombre de documents à valider ; son libellé est au pluriel s'il y a plusieurs documents.

1. Dans le menu de gauche d'INGENEO PRECOMPTA, cliquez sur `Tableau de bord`.
2.  Cliquez sur le raccourci orange `Document en attente de validation`.

    L'écran de pré-saisie comptable s'ouvre directement sur le premier document à valider. Les documents suivants sont dans la liste en haut à gauche de l'écran.

### Ouvrir un document à valider depuis la cloche Actions / Notifications

1.  Depuis n'importe quelle page d'INGENEO PRECOMPTA, cliquez sur la cloche, en haut à gauche de l'en-tête.

    Le panneau `Actions / Notifications` affiche une ligne par entreprise.
2.  Sur la ligne de l'entreprise, cliquez sur le bouton œil.

    Le menu `Bannettes` s'ouvre sur cette entreprise, onglet `Actions / Notifications`.
3. Cliquez sur le bouton orange à 3 traits, à droite de l'onglet `Actions / Notifications`.
4.  Cliquez sur `Documents à valider`.

    La page `Documents à valider` liste les documents en attente de validation.
5.  Sur la ligne du document, cliquez sur le bouton bleu en forme d'œil, tout à droite. Au survol, il affiche `voir le document en attente de validation`.

    L'écran de pré-saisie comptable s'ouvre sur ce document.

### Valider le document

1. Dans l'écran de pré-saisie comptable d'INGENEO PRECOMPTA, cliquez sur le bouton vert `Valider`. Il se trouve au même endroit que le bouton `Enregistrer`.

### Refuser le document

Dans INGENEO PRECOMPTA, le bouton `Refuser` ne s'affiche que si l'interrupteur `Refuser` est activé pour l'utilisateur dans le circuit de validation.

1.  Dans l'écran de pré-saisie comptable, cliquez sur le bouton rouge `Refuser`. Il se trouve au même endroit que le bouton `Enregistrer`.

    La fenêtre `Refus d'un document` s'ouvre avec le texte « Vous allez refuser la validation d'un document. ».
2. Dans l'encart `Motif du refus`, saisissez le motif du refus. Ce motif est obligatoire.
3. Cliquez sur `Enregistrer`, en bas à droite de la fenêtre `Refus d'un document`.

## Résultat attendu

**Après `Valider` :** dans INGENEO PRECOMPTA, le document passe au niveau suivant du circuit de validation. L'utilisateur du niveau suivant reçoit une notification de type `Validation` dans `Actions / Notifications`.

**Après `Refuser` :** dans INGENEO PRECOMPTA, l'effet du refus dépend du paramètre `Refuser et` de l'étape du circuit de validation :

* `Renvoyer à l'étape précédente` : le document revient à l'étape précédente ;
* `Arrêter le circuit de validation` : le circuit s'arrête ; le document se retrouve dans le menu `Rechercher` ;
* `Envoyer à l'étape suivante` : le document passe à l'étape suivante.

**Statut du document :** dans INGENEO PRECOMPTA, le statut du document change après une validation ou un refus si le circuit a les options `Appliquer le statut après validation` ou `Appliquer le statut après refus`.

**Export vers le logiciel comptable :** dans INGENEO PRECOMPTA, le moment de l'export dépend du paramétrage du circuit de validation :

* avec `Transférer en comptabilité lors de la validation finale`, le document est exporté après la validation du dernier niveau ;
* si le circuit compte plusieurs étapes, l'interrupteur `Export Compta` d'une étape détermine à quelle étape le document est exporté ;
* sans `Transférer en comptabilité lors de la validation finale`, le document est exporté dès que l'`Initiateur` clique sur `Enregistrer` dans l'écran de pré-saisie comptable.

## Erreurs fréquentes

**Le document à valider n'apparaît pas dans `Documents à valider`.** Dans INGENEO PRECOMPTA, trois causes sont possibles :

* l'utilisateur n'est pas `Valideur` à l'étape où se trouve le document ;
* le document n'a pas encore atteint le niveau de l'utilisateur dans le circuit de validation ;
* un autre `Valideur` du même niveau, sans l'interrupteur `Obliger`, a déjà validé le document, qui est passé au niveau suivant.

**Le bouton `Refuser` n'apparaît pas dans l'écran de pré-saisie comptable.** Dans INGENEO PRECOMPTA, l'interrupteur `Refuser` n'est pas activé pour l'utilisateur dans le bloc `ETAPES` du circuit de validation. Demandez la modification du circuit à la personne qui le paramètre.

**Le refus ne s'enregistre pas.** Dans INGENEO PRECOMPTA, l'encart `Motif du refus` de la fenêtre `Refus d'un document` est obligatoire. Saisissez un motif, puis cliquez sur `Enregistrer`.

**Plusieurs documents sont à valider en une fois.** Dans INGENEO PRECOMPTA, aucune validation en masse n'existe. Validez chaque document individuellement dans l'écran de pré-saisie comptable.

**Un document refusé a disparu.** Dans INGENEO PRECOMPTA, après un refus avec `Arrêter le circuit de validation`, le document se retrouve dans le menu `Rechercher`.

## Fiches liées

* [Créer un circuit de validation](../processus-metiers/workflow/circuit-de-validation.md) : rôles, interrupteurs `Refuser`, `Refuser et`, `Export Compta` et options de statut.
* [Consulter et gérer les notifications](../processus-metiers/workflow/consulter-et-gerer-les-notifications.md) : cloche `Actions / Notifications` et notifications de type `Validation`.
* [Rechercher un document](rechercher-un-document.md) : retrouver un document après l'arrêt du circuit de validation.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-valider-document-ingeneo-precompta
* titre : Comment valider ou refuser un document dans INGENEO PRECOMPTA ?
* titre\_menu : Valider ou refuser un document
* type : procedure
* module : Gestion des documents
* version\_outil : non précisée
* roles\_concernes : utilisateur avec le rôle `Valideur` dans un circuit de validation
* tags : circuit de validation, valideur, validation, refus, motif du refus, documents à valider
* formulations\_utilisateur : « Comment valider une facture ? » ; « Où voir les documents que je dois valider ? » ; « Comment refuser un document ? » ; « Je ne vois pas le document à valider » ; « Peut-on valider plusieurs documents en même temps ? »
* sources : Refonte de la page GitBook ingeneo-pre-compta/gestion-des-documents/valider-un-document ; démo Arcade « Valider un document » (retirée) ; fiche proc-creer-circuit-validation-ingeneo-precompta ; fiche proc-consulter-gerer-notifications-ingeneo-precompta ; réponses de l'expert 2026-11-06
* redacteur : CH
* relecteur :
* derniere\_verification : 2026-11-06
* statut : brouillon

</details>
