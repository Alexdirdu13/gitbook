---
description: >-
  Créer, modifier et supprimer une liste de statuts de documents dans INGENEO
  PRECOMPTA. Droit requis : paramétrage des processus métier.
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

# Comment configurer les statuts de documents dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de créer, modifier et supprimer une liste de statuts de documents dans INGENEO PRECOMPTA, puis d'appliquer un statut à un document. Elle nécessite le droit `Autoriser l’accès au paramétrage des processus métier`.

### Objectif

Dans INGENEO PRECOMPTA, un statut de document indique l'état d'un document, par exemple « Payé » ou « Litige ». Les statuts sont regroupés dans des listes de statuts. Chaque liste de statuts est associée à un ou plusieurs classeurs comptables ou classeurs du plan de classement.

Dans INGENEO PRECOMPTA, un statut s'applique à un document de deux façons :

* manuellement : dans l'écran de pré-saisie comptable du menu `Bannettes`, avec le champ `Statuts du document` ;
* automatiquement : par un circuit de validation, à l'étape du circuit où le statut est défini.

Utilisez les listes de statuts d'INGENEO PRECOMPTA pour définir les étapes de traitement d'un document et suivre les documents par état d'avancement. Créez-les avant le circuit de validation qui les utilise.

### Prérequis

* Droit pour configurer les statuts : dans INGENEO PRECOMPTA, seul un utilisateur avec le droit `Autoriser l’accès au paramétrage des processus métier` configure les listes de statuts. Le détail des droits est dans [Détail des droits](https://help.ingeneo.septeo.com/ingeneo-pre-compta/administration/detail-des-droits).
* Classeurs : les classeurs comptables ou les classeurs du plan de classement à associer existent déjà dans l'entreprise.
* Droit pour appliquer un statut avec `Enregistrer` : dans INGENEO PRECOMPTA, l'utilisateur a le droit par classeur `Enregistrer les documents`. Ce droit se trouve dans `Entreprises > Editer > Administration > Profils d'entreprise`, étape `Droits sur les classeurs`, bloc `TRAITEMENTS`. Sans ce droit, l'utilisateur applique le statut avec `Enregistrer comme brouillon`.

### Étapes

#### Créer une liste de statuts

1. Dans INGENEO PRECOMPTA, cliquez sur `Entreprises` dans le menu de gauche.
2. Sur la ligne de l'entreprise, cliquez sur `Editer`.
3. Cliquez sur l'onglet `Plan de classement`.
4. Cliquez sur `Processus métier`.
5. Cliquez sur `Statuts`. La liste des listes de statuts s'affiche.
6. Cliquez sur `+ Ajouter`. Le panneau `Création d'une nouvelle liste de statuts` s'ouvre.
7. Dans le bloc `CONFIGURATION`, saisissez le nom de la liste dans `Intitulé`.
8. Dans `Classeurs`, sélectionnez un ou plusieurs classeurs.
9. Laissez le champ `Type de document` sur `Aucun` : il n'est pas utilisé.
10. Dans le bloc `LISTE DES STATUTS`, cliquez sur `+`. Une ligne de statut s'ajoute.
11. Sur cette ligne, saisissez le nom du statut dans `Intitulé du statut`.
12. Pour donner une couleur au statut, choisissez-la dans `Couleur`. La couleur par défaut est le noir.
13. Pour retirer une ligne de statut, cliquez sur la corbeille rouge de la ligne.
14. Répétez les étapes 10 à 12 pour chaque statut de la liste.
15. Cliquez sur `Enregistrer`.

#### Modifier une liste de statuts

1. Dans INGENEO PRECOMPTA, ouvrez `Entreprises > Editer > Plan de classement > Processus métier > Statuts`.
2. Sur la ligne de la liste de statuts, cliquez sur le bouton d'édition.
3. Modifiez les champs voulus : `Intitulé`, `Classeurs`, `Intitulé du statut` ou `Couleur`.
4. Cliquez sur `Enregistrer`.

Dans INGENEO PRECOMPTA, la modification d'une liste de statuts met à jour les documents qui portent déjà ses statuts.

#### Supprimer un statut ou une liste de statuts

{% hint style="warning" %}
Dans INGENEO PRECOMPTA, quand un statut ou une liste de statuts est supprimé, le statut n'apparaît plus sur les documents qui le portaient.
{% endhint %}

1. Dans INGENEO PRECOMPTA, ouvrez `Entreprises > Editer > Plan de classement > Processus métier > Statuts`.
2. Pour supprimer toute la liste, cliquez sur le bouton de suppression de sa ligne.
3. Pour supprimer un seul statut, cliquez sur le bouton d'édition de la ligne de la liste.
4. Dans le bloc `LISTE DES STATUTS`, cliquez sur la corbeille rouge du statut.
5. Cliquez sur `Enregistrer`.

#### Appliquer manuellement un statut à un document

1. Dans INGENEO PRECOMPTA, cliquez sur `Bannettes` dans le menu de gauche.
2. Ouvrez le classeur du document.
3. Ouvrez l'écran de pré-saisie comptable du document.
4. Cliquez sur `Processus métiers`.
5. Dans `Statuts du document`, sélectionnez le statut.
6. Si la pré-saisie comptable est complète et correcte et que vous avez le droit `Enregistrer les documents`, cliquez sur `Enregistrer`.
7. Sinon, cliquez sur la flèche du bouton d'enregistrement, puis sur `Enregistrer comme brouillon`.

### Résultat attendu

Dans INGENEO PRECOMPTA, la liste de statuts apparaît dans `Entreprises > Editer > Plan de classement > Processus métier > Statuts`, avec les colonnes `Intitulé`, `Classeurs` et `Statuts`.

Pour les documents des classeurs associés, les statuts de la liste sont proposés dans le champ `Statuts du document` de l'écran de pré-saisie comptable. Le statut appliqué s'affiche dans la colonne `Statuts` de la liste des documents du menu `Bannettes`.

Dans le panneau `Edition d'un circuit`, la liste est proposée dans `Listes de statuts applicables` pour les circuits de validation des mêmes classeurs.

### Erreurs fréquentes

**Un statut n'est pas proposé dans le champ `Statuts du document`.** Dans INGENEO PRECOMPTA, le champ `Statuts du document` ne propose que les statuts des listes associées au classeur du document. Ajoutez le classeur dans le champ `Classeurs` de la liste de statuts.

**Un circuit de validation n'applique pas le statut voulu.** Dans INGENEO PRECOMPTA, un circuit de validation n'applique que les statuts d'une liste associée au classeur du circuit. Le statut à appliquer est défini dans le bloc `ETAPES` du circuit, avec les options `Appliquer le statut après validation` et `Appliquer le statut après refus`.

**Le statut a disparu d'un document.** Dans INGENEO PRECOMPTA, le statut ou sa liste de statuts a été supprimé dans l'écran `Statuts`. Le statut n'apparaît plus sur les documents qui le portaient.

**L'utilisateur ne peut pas appliquer le statut avec `Enregistrer`.** Dans INGENEO PRECOMPTA, `Enregistrer` demande une pré-saisie comptable complète et correcte, et le droit `Enregistrer les documents` sur le classeur. Sinon, l'utilisateur utilise `Enregistrer comme brouillon`.

### Fiches liées

* [Créer un circuit de validation](https://help.ingeneo.septeo.com/ingeneo-pre-compta/processus-metiers/workflow/circuit-de-validation) : utilisation des listes de statuts dans `Listes de statuts applicables` et dans les étapes du circuit.
* [Valider un document](https://help.ingeneo.septeo.com/ingeneo-pre-compta/gestion-des-documents/valider-un-document) : validation ou refus d'un document engagé dans un circuit de validation.
* [Détail des droits](https://help.ingeneo.septeo.com/ingeneo-pre-compta/administration/detail-des-droits) : droits `Autoriser l’accès au paramétrage des processus métier` et `Enregistrer les documents`.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-configurer-statuts-documents-ingeneo-precompta
* titre : Comment configurer les statuts de documents dans INGENEO PRECOMPTA ?
* titre\_menu : Configurer les statuts de documents
* type : procedure
* module : Processus métier
* version\_outil : 2.16.0 (version observée)
* roles\_concernes : utilisateur avec le droit `Autoriser l’accès au paramétrage des processus métier` ; utilisateur avec le droit `Enregistrer les documents`
* tags : statuts, liste de statuts, processus métier, circuit de validation, bannettes
* formulations\_utilisateur : « Comment créer des statuts sur mes documents ? » ; « Comment marquer une facture comme payée ? » ; « Comment changer la couleur d'un statut ? » ; « Pourquoi mon statut n'apparaît pas sur le document ? » ; « Comment supprimer un statut ? »
* sources : Refonte de la page GitBook ingeneo-pre-compta/processus-metiers/workflow/configurer-les-statuts-de-documents ; observation de l'application INGENEO PRECOMPTA 2.16.0 (2026-11-04) ; réponses de l'expert 2026-11-04
* redacteur : CG
* relecteur :
* derniere\_verification : 2026-11-04
* statut : brouillon

</details>
