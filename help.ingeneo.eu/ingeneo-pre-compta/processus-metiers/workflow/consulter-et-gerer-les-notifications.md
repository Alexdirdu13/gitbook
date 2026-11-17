---
description: >-
  Consulter les notifications (cloche) et les alertes (triangle) d'INGENEO
  PRECOMPTA, prendre en compte ou supprimer une notification. Aucun droit
  particulier n'est nécessaire.
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

# Comment consulter et gérer les notifications et les alertes dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de consulter les notifications et les alertes d'INGENEO PRECOMPTA, puis de prendre en compte ou de supprimer une notification. Elle ne nécessite aucun droit particulier : l'accès à l'entreprise suffit.

## Objectif

Dans INGENEO PRECOMPTA, deux icônes de l'en-tête, en haut à gauche à droite du logo, signalent ce qui demande l'attention de l'utilisateur :

* la cloche ouvre le panneau `Actions / Notifications`, qui regroupe les notifications des entreprises : rapports générés, demandes d'action, validations, connecteurs en échec ;
* le triangle, sous la cloche, ouvre le panneau `Alertes`, qui compte les documents en cours de traitement ou bloqués.

Dans INGENEO PRECOMPTA, chaque notification a un type, choisi dans la liste `Action / Notification` de l'onglet `Actions / Notifications` : `Connecteurs Bancaires`, `Connecteurs Clouds`, `Connecteurs Marchands`, `Demande d'action`, `Demande de paiement`, `Export fichiers d'écritures`, `Formulaire Engagement de dépenses`, `Formulaire note de frais`, `Note`, `Obsolescence de documents`, `Reporting`, `Validation`, `Validation Engagement de dépenses`, `Validation note de frais`. Chaque notification a aussi une `Origine` : `Système` ou `Utilisateur`.

Consultez la cloche d'INGENEO PRECOMPTA chaque jour, pour éviter l'accumulation de notifications et repérer celles qui demandent une action.

## Prérequis

* Droits : dans INGENEO PRECOMPTA, aucun droit particulier n'est nécessaire pour consulter les notifications et le panneau `Alertes`, ni pour utiliser `Prise en compte de la notification`, `Prise en compte de toutes les notifications` et `Supprimer`.
* Périmètre : dans INGENEO PRECOMPTA, l'utilisateur ne voit que les notifications des entreprises auxquelles il a accès. Ces accès sont configurés par l'administrateur.

## Étapes

### Consulter les notifications depuis la cloche de l'en-tête

Dans INGENEO PRECOMPTA, la cloche de l'en-tête porte un badge orange. Ce badge indique le nombre d'entreprises qui ont des notifications, et non le nombre total de notifications.

1.  Depuis n'importe quelle page d'INGENEO PRECOMPTA, cliquez sur la cloche, en haut à gauche de l'en-tête.

    Le panneau `Actions / Notifications` affiche une ligne par entreprise : « Vous avez N notifications pour l'entreprise : \[nom de l'entreprise] ».
2.  Sur la ligne de l'entreprise, cliquez sur le bouton œil.

    Le menu `Bannettes` s'ouvre sur cette entreprise, onglet `Actions / Notifications`.
3. Pour lire le détail d'une notification, cliquez sur le bouton `Voir` (icône œil) de sa ligne, dans la colonne `Actions`.

### Consulter les notifications d'une entreprise depuis le menu Bannettes

Dans INGENEO PRECOMPTA, la liste `Entreprises` du menu `Bannettes` affiche une cloche suivie du nombre de notifications pour chaque entreprise concernée. Cette méthode convient quand vous travaillez sur une seule entreprise.

1. Dans le menu de gauche d'INGENEO PRECOMPTA, cliquez sur `Bannettes`.
2. Dans la liste `Entreprises`, cliquez sur l'entreprise.
3. Cliquez sur l'onglet `Actions / Notifications`.

Dans INGENEO PRECOMPTA, l'onglet `Actions / Notifications` d'une entreprise liste ses notifications dans les colonnes `Date`, `Titre`, `Origine`, `Date de prise en compte` et `Actions`.

* La liste `Afficher` règle le nombre de lignes : 10, 25, 50 ou 100.
* Le champ `Rechercher` filtre la liste sur un texte.
* Le bouton `Filtres` affiche les filtres `Action / Notification`, `Origine` et `Période`, ainsi que le bouton `Réinitialiser`. La `Période` couvre un an par défaut.

### Prendre en compte ou supprimer une notification

Dans INGENEO PRECOMPTA, une notification prise en compte disparaît de la liste de l'onglet `Actions / Notifications`. Une notification supprimée est effacée définitivement.

1. Ouvrez `Bannettes` > entreprise > onglet `Actions / Notifications`.
2. Repérez la ligne de la notification.
3. Pour marquer la notification comme traitée, cliquez sur `Prise en compte de la notification` (coche orange), dans la colonne `Actions`.
4. Pour effacer la notification, cliquez sur `Supprimer` (corbeille rouge), dans la colonne `Actions`.

{% hint style="danger" %}
Dans INGENEO PRECOMPTA, le bouton `Supprimer` d'une notification de l'onglet `Actions / Notifications` l'efface définitivement. Une notification supprimée ne peut pas être récupérée.
{% endhint %}

Pour prendre en compte toutes les notifications d'une entreprise en une fois :

1. Dans `Bannettes` > entreprise > onglet `Actions / Notifications`, cliquez sur le bouton orange à 3 traits, à droite.
2. Cliquez sur `Prise en compte de toutes les notifications`.

`Prise en compte de toutes les notifications` fait disparaître toutes les notifications de l'entreprise, quels que soient les filtres affichés.

Dans INGENEO PRECOMPTA, le même menu orange à 3 traits propose aussi `Documents à valider`, `Notes de frais à valider`, `Engagements à valider` et `Factures à payer`. Chacune de ces entrées ouvre une page dédiée.

### Consulter les alertes depuis le triangle de l'en-tête

Dans INGENEO PRECOMPTA, le triangle de l'en-tête n'affiche pas de badge. Ouvrez le panneau `Alertes` pour voir ses compteurs.

1.  Depuis n'importe quelle page d'INGENEO PRECOMPTA, cliquez sur le triangle, sous la cloche de l'en-tête.

    Le panneau `Alertes` affiche quatre compteurs :

    * `Documents en cours de LAD` : documents en cours de traitement OCRLAD ;
    * `Documents en attente d'export` : documents qui attendent leur export vers le logiciel comptable ;
    * `Documents corrompus` : documents illisibles ;
    * `Documents en erreur d'export` : documents dont l'export vers le logiciel comptable a échoué.
2.  Pour voir les documents en attente d'export, cliquez sur le bouton œil de `Documents en attente d'export`.

    Le menu `Rechercher` s'ouvre sur l'onglet de résultats `En attente d'export`, qui liste les documents concernés.

Dans le panneau `Alertes` d'INGENEO PRECOMPTA, un bouton œil figure seulement sur `Documents en attente d'export` et `Documents corrompus`, même quand le compteur vaut 0.

## Résultat attendu

Dans INGENEO PRECOMPTA, après `Prise en compte de la notification`, la notification disparaît de l'onglet `Actions / Notifications` de l'entreprise. Quand l'entreprise n'a plus de notification, elle quitte le panneau `Actions / Notifications` de la cloche et le badge orange diminue de 1.

Après `Supprimer`, la notification est effacée définitivement.

Après un clic sur le bouton œil de `Documents en attente d'export` du panneau `Alertes`, le menu `Rechercher` affiche l'onglet `En attente d'export` avec le nombre de documents concernés.

## Erreurs fréquentes

**Le badge de la cloche affiche un nombre plus petit que le nombre de notifications.** Dans INGENEO PRECOMPTA, le badge orange de la cloche compte les entreprises qui ont des notifications, et non les notifications. Le panneau `Actions / Notifications` de la cloche donne le nombre de notifications de chaque entreprise.

**Le triangle de l'en-tête n'affiche aucun nombre.** Dans INGENEO PRECOMPTA, le triangle n'a pas de badge. Cliquez sur le triangle pour afficher les compteurs du panneau `Alertes`.

**Une notification n'apparaît plus dans l'onglet `Actions / Notifications`.** Dans INGENEO PRECOMPTA, une notification disparaît de la liste après `Prise en compte de la notification`, `Prise en compte de toutes les notifications` ou `Supprimer`.

**Les notifications d'une entreprise ne s'affichent pas.** Dans INGENEO PRECOMPTA, l'utilisateur ne voit que les notifications des entreprises auxquelles il a accès. Demandez à l'administrateur de vérifier vos accès à cette entreprise.

**Le compteur `Documents corrompus` du panneau `Alertes` n'est pas à 0.** Dans INGENEO PRECOMPTA, un document corrompu est illisible. Téléchargez-le de nouveau depuis sa provenance.

**Les compteurs `Documents en attente d'export` ou `Documents en erreur d'export` du panneau `Alertes` ne sont pas à 0.** Dans INGENEO PRECOMPTA, vérifiez la connexion de l'entreprise à son logiciel comptable. Pour relancer l'export d'un document, faites un clic droit sur le document dans le menu `Rechercher`, puis cliquez sur `Remettre à l'export`.

## Fiches liées

* [Rechercher un document](../../gestion-des-documents/rechercher-un-document.md) : le menu `Rechercher` affiche les documents en attente d'export ouverts depuis le panneau `Alertes`.
* [Créer un circuit de validation](circuit-de-validation.md) : les validations d'un circuit de validation produisent des notifications de type `Validation`.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-consulter-gerer-notifications-ingeneo-precompta
* titre : Comment consulter et gérer les notifications et les alertes dans INGENEO PRECOMPTA ?
* titre\_menu : Consulter et gérer les notifications
* type : procedure
* module : Processus métier
* version\_outil : 2.16.0 (version observée)
* roles\_concernes : tout utilisateur ayant accès à l'entreprise
* tags : notifications, alertes, cloche, prise en compte, export, OCRLAD
* formulations\_utilisateur : « Où voir mes notifications ? » ; « Que veut dire le chiffre sur la cloche ? » ; « Comment faire disparaître une notification ? » ; « À quoi sert le triangle en haut de l'écran ? » ; « Comment voir les documents en attente d'export ? »
* sources : Refonte de la page GitBook ingeneo-pre-compta/processus-metiers/workflow/consulter-et-gerer-les-notifications ; observation de l'application INGENEO PRECOMPTA 2.16.0 (2026-11-06) ; réponses de l'expert 2026-11-06
* redacteur : CG
* relecteur :
* derniere\_verification : 2026-11-06
* statut : brouillon

</details>
