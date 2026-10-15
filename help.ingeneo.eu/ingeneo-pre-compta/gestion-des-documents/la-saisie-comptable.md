---
description: >-
  Faire la pré-saisie comptable d'un document dans INGENEO PRECOMPTA : compte
  tiers, comptes de charges et de TVA, enregistrement et export. Nécessite le
  droit Enregistrer les documents.
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

# Comment faire la pré-saisie comptable d'un document dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de faire la pré-saisie comptable d'un document dans l'écran de pré-saisie comptable du menu `Bannettes` d'INGENEO PRECOMPTA : compte tiers, comptes de charges et de TVA, puis enregistrement et export. Elle nécessite le droit `Enregistrer les documents`.

## Objectif

Dans INGENEO PRECOMPTA, la pré-saisie comptable attribue à un document d'un classeur comptable ses comptes et ses éléments comptables. Elle se fait dans l'écran de pré-saisie comptable, ouvert depuis le menu `Bannettes`.

Après un clic sur `Enregistrer`, le document est exporté automatiquement vers le logiciel comptable de l'entreprise. Exception : les entreprises en export On Demand ne sont pas exportées automatiquement. Leurs écritures s'exportent à la demande, comme décrit dans [Export des écritures On Demand](../divers/export-des-ecritures-on-demand.md).

L'écran de pré-saisie comptable n'affiche ni titre ni libellé. Il ne faut pas le confondre avec un masque de saisie, qui est un modèle d'écritures enregistré et rappelé par raccourci clavier.

## Prérequis

* Dans INGENEO PRECOMPTA, l'utilisateur doit avoir le droit `Enregistrer les documents`. Le détail des droits est dans [Détail des droits](../administration/detail-des-droits.md).
* Le document doit être présent dans un classeur comptable de l'entreprise, dans le menu `Bannettes`.
* Avant de commencer, vérifiez que l'entreprise sélectionnée dans le menu `Bannettes` est la bonne, pour éviter les erreurs de comptabilisation.
* Pour imputer les bons comptes, l'utilisateur doit connaître le plan comptable de l'entreprise.
* Les éléments comptables affichés dépendent du paramétrage du classeur comptable, décrit dans [Comment créer et paramétrer un classeur comptable dans INGENEO PRECOMPTA ?](../gestion-des-entreprises/classeurs-comptables.md).

## Étapes

### Ouvrir l'écran de pré-saisie comptable

1. Dans INGENEO PRECOMPTA, cliquez sur `Bannettes` dans le menu de gauche.
2. Sélectionnez l'entreprise dans la liste.
3. Sélectionnez ou recherchez le classeur comptable qui contient le document.
4. Sur la ligne du document, cliquez sur la loupe en bout de ligne.

L'écran de pré-saisie comptable s'ouvre. Il a 3 volets redimensionnables :

* la liste des documents du classeur comptable ;
* le volet de pré-saisie comptable du document ;
* l'aperçu du document, avec son historique et ses notes.

Pour passer à un autre document du même classeur comptable, sélectionnez-le dans la liste des documents de l'écran de pré-saisie comptable.

### Vérifier les éléments comptables

Dans l'écran de pré-saisie comptable d'INGENEO PRECOMPTA, la plupart des éléments comptables sont renseignés par le traitement OCRLAD du document. Par défaut, la date de facture, la date d'échéance et le numéro de facture sont affichés.

1. Dans le volet de pré-saisie comptable, vérifiez chaque élément comptable renseigné par l'OCRLAD.
2. Si un élément est faux ou vide, corrigez-le.

Pour afficher d'autres éléments comptables, ou en rendre certains obligatoires, réglez l'onglet `Eléments comptables` du classeur comptable.

### Renseigner le compte tiers

Dans l'écran de pré-saisie comptable d'INGENEO PRECOMPTA, le compte tiers est renseigné automatiquement si deux conditions sont réunies : le fournisseur a été reconnu dans le document, et le compte tiers est présent dans le FEC de l'entreprise. Sinon, renseignez le compte tiers dans le champ `Compte` d'une ligne d'écriture, par l'une des trois méthodes suivantes.

**Rechercher le compte tiers par saisie**

1. Dans le tableau des lignes d'écriture, cliquez dans le champ `Compte` de la ligne à renseigner.
2. Saisissez les premiers caractères du code du compte tiers ou de son intitulé.
3. Dans la liste qui s'affiche, sélectionnez le compte tiers.

**Rechercher le compte tiers dans le panneau de recherche**

1. Dans le tableau des lignes d'écriture, cliquez dans le champ `Compte` de la ligne à renseigner.
2. Appuyez sur la touche `Entrée` du clavier.
3. Dans le panneau `Recherche d'un enregistrement`, repérez le compte tiers. Les colonnes du tableau sont notamment `Compte`, `Intitulé`, `Collectif` et `Type`.
4. Sur la ligne du compte tiers, cliquez sur la coche verte de la colonne `Actions`.

**Créer le compte tiers**

Si le compte tiers n'existe pas, créez-le depuis l'écran de pré-saisie comptable :

1. Dans le champ `Compte` de la ligne à renseigner, saisissez le code du nouveau compte tiers.
2. Appuyez sur la touche `Entrée` du clavier. Le panneau `Création d'un enregistrement` s'ouvre directement.
3. À l'étape `Compte tiers`, renseignez les champs du compte (`Type`, `Compte`, `Intitulé`, `Compte collectif`, `Mode de règlement`, `Journal`, ainsi que les blocs `MODALITÉS D'ÉCHÉANCES` et `DEVISES`).
4. Si besoin, cliquez sur l'étape `Entreprise` et complétez les informations sur l'entreprise du tiers.
5. Si besoin, cliquez sur l'étape `Options avancées` et sélectionnez les options voulues.
6. Cliquez sur `Enregistrer`, en bas du panneau `Création d'un enregistrement`.

À la création, seuls le code (`Compte`) et l'intitulé (`Intitulé`) du compte tiers sont obligatoires, sauf si le paramétrage avancé de la comptabilité de l'entreprise impose d'autres champs. Le compte tiers est créé dans le logiciel comptable au moment de l'intégration de l'écriture.

### Saisir les comptes de charges et de TVA

Dans l'écran de pré-saisie comptable d'INGENEO PRECOMPTA, le tableau des lignes d'écriture contient les colonnes `Journal`, `Compte`, `Libellé`, `Code TVA`, `Débit` et `Crédit`.

1. Dans le champ `Compte` d'une ligne de charge, saisissez les premiers caractères ou chiffres du compte, ou un mot de son libellé.
2. Dans la liste qui s'affiche, sélectionnez le compte de charges.
3. Dans le champ `Compte` d'une ligne de TVA, saisissez les premiers caractères ou chiffres du compte, ou un mot de son libellé.
4. Dans la liste qui s'affiche, sélectionnez le compte de TVA.

Pour gérer les lignes du tableau des lignes d'écriture :

* **Ajouter une ligne à la fin du tableau** : cliquez sur le bouton `+` bleu, à gauche sous la dernière ligne, ou utilisez le raccourci `Ctrl +`.
* **Insérer une ligne entre deux lignes** : survolez avec la souris l'espace entre les deux lignes, puis cliquez sur `Insérer une ligne d'écriture`.
* **Supprimer une ligne** : cliquez sur la corbeille rouge, à gauche de la ligne, ou utilisez le raccourci `Ctrl -`.

Ces boutons n'affichent pas d'infobulle au survol.

### Contrôler l'onglet Vigilances

Dans l'écran de pré-saisie comptable d'INGENEO PRECOMPTA, l'onglet `Vigilances` n'apparaît que si le document présente au moins une vigilance. Il reprend les indicateurs du document, par exemple un doublon, une date en dehors de l'exercice ou une saisie déjà enregistrée.

1. Si l'onglet `Vigilances` est affiché, cliquez dessus.
2. Traitez chaque vigilance avant d'enregistrer la pré-saisie comptable.

### Enregistrer la pré-saisie comptable

{% hint style="warning" %}
Dans INGENEO PRECOMPTA, un document exporté après un clic sur `Enregistrer` dans l'écran de pré-saisie comptable ne peut plus être corrigé dans INGENEO PRECOMPTA. Pour corriger l'écriture, faites la correction dans le logiciel comptable, ou déposez de nouveau le document dans le classeur comptable. Vérifiez la pré-saisie comptable et l'onglet `Vigilances` avant d'enregistrer.
{% endhint %}

1. Vérifiez le compte tiers, les comptes de charges et les comptes de TVA.
2. Cliquez sur `Enregistrer`.

## Résultat attendu

Dans INGENEO PRECOMPTA, après un clic sur `Enregistrer` dans l'écran de pré-saisie comptable :

* le document est exporté automatiquement vers le logiciel comptable, sauf si l'entreprise est en export On Demand ;
* le document n'apparaît plus dans le classeur comptable du menu `Bannettes` ;
* le document reste accessible avec le menu `Rechercher`.

## Erreurs fréquentes

* **Le document n'apparaît plus dans le classeur comptable après la pré-saisie comptable.** Dans INGENEO PRECOMPTA, un document enregistré est exporté et quitte le classeur comptable du menu `Bannettes`. Solution : retrouvez-le avec le menu `Rechercher`.
* **Une erreur est découverte après l'enregistrement.** Dans INGENEO PRECOMPTA, un document exporté ne se corrige plus. Solution : corrigez l'écriture dans le logiciel comptable, ou déposez de nouveau le document dans le classeur comptable.
* **Le compte tiers n'est pas renseigné automatiquement.** Dans l'écran de pré-saisie comptable d'INGENEO PRECOMPTA, le compte tiers n'est renseigné automatiquement que si le fournisseur est reconnu dans le document et que le compte tiers est présent dans le FEC. Solution : recherchez le compte tiers dans le champ `Compte`, ou créez-le avec la touche `Entrée`.
* **Le message `Compte collectif obligatoire` s'affiche à la création d'un compte tiers.** Dans INGENEO PRECOMPTA, l'interrupteur `Obliger la saisie d'un collectif lors de la création d'un compte.` est activé dans `Comptabilité > Paramétrage avancé`. Solution : renseignez le `Compte collectif` du tiers dans le panneau `Création d'un enregistrement`.
* **La création d'un compte tiers demande le SIREN et l'IBAN.** Dans INGENEO PRECOMPTA, l'interrupteur `Obliger la saisie des informations sur l'entreprise.` est activé dans `Comptabilité > Paramétrage avancé`. Solution : renseignez le SIREN et l'IBAN du tiers dans le panneau `Création d'un enregistrement`.
* **Un document enregistré n'est pas exporté.** Dans INGENEO PRECOMPTA, vérifiez que l'interrupteur `Ne pas exporter` du document est désactivé dans l'écran de pré-saisie comptable. Si l'entreprise est en export On Demand, exportez les écritures comme décrit dans [Export des écritures On Demand](../divers/export-des-ecritures-on-demand.md).

## Fiches liées

* [Comment créer et paramétrer un classeur comptable dans INGENEO PRECOMPTA ?](../gestion-des-entreprises/classeurs-comptables.md) : éléments comptables affichés en pré-saisie comptable, options `Ne pas exporter` et vigilances du classeur.
* [Masque de saisie](masque-de-saisie.md) : modèles d'écritures enregistrés, rappelés avec `CTRL` + code depuis l'écran de pré-saisie comptable.
* [Export des écritures On Demand](../divers/export-des-ecritures-on-demand.md) : export manuel des écritures pour les entreprises en export On Demand.
* [Comment paramétrer et saisir l'analytique d'une entreprise dans INGENEO PRECOMPTA ?](../gestion-des-entreprises/analytique.md) : ventilation des lignes d'écriture avec `Insérer une ligne analytique`.
* [Comment faire le paramétrage avancé de la comptabilité d'une entreprise dans INGENEO PRECOMPTA ?](../gestion-des-entreprises/parametrage-comptabilite-avance.md) : règles de création des comptes tiers.
* [Rechercher un document](rechercher-un-document.md) : retrouver un document exporté.
* [Détail des droits](../administration/detail-des-droits.md) : droit `Enregistrer les documents`.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-faire-presaisie-comptable-document-ingeneo-precompta
* titre : Comment faire la pré-saisie comptable d'un document dans INGENEO PRECOMPTA ?
* titre\_menu : Faire la pré-saisie comptable
* type : procedure
* module : Gestion des documents
* version\_outil : toutes
* roles\_concernes : utilisateur avec le droit `Enregistrer les documents`
* tags : pré-saisie comptable, Bannettes, compte tiers, imputation, export, Vigilances
* formulations\_utilisateur : « Comment saisir une facture dans la bannette ? » ; « Comment créer un compte fournisseur depuis la saisie ? » ; « Comment ajouter une ligne de TVA ? » ; « Mon document a disparu après la saisie » ; « Je me suis trompé de compte après avoir enregistré »
* sources : Refonte de la page GitBook ingeneo-pre-compta/gestion-des-documents/la-saisie-comptable ; données de la démo Arcade « Création compte de tiers » (mise à jour 2026-07-24) ; pages GitBook « Masque de saisie », « Export des écritures On Demand », « Comment créer et paramétrer un classeur comptable », « Comment faire le paramétrage avancé de la comptabilité » ; réponses de l'expert 2026-10-15
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-15
* statut : brouillon

</details>
