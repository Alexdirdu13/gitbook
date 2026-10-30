---
description: >-
  Créer un circuit de validation prédéfini dans INGENEO PRECOMPTA : classeurs,
  statuts, niveaux, rôles et options par étape. Droit requis : paramétrage des
  processus métier.
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

# Comment créer un circuit de validation dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de créer un circuit de validation de type `Prédéfini` pour les documents d'un ou plusieurs classeurs dans INGENEO PRECOMPTA. Elle nécessite le droit `Autoriser l’accès au paramétrage des processus métier`.

## Objectif

Dans INGENEO PRECOMPTA, un circuit de validation fait valider un document par des utilisateurs, niveau par niveau, avant sa comptabilisation. Il trace le parcours de validation du document.

INGENEO PRECOMPTA propose deux types de circuits de validation :

* `Prédéfini` : circuit associé à des classeurs comptables ou à des classeurs du plan de classement. Cette procédure crée ce type de circuit.
* `Formulaire` : circuit associé à un formulaire des processus métier. Son paramétrage est décrit dans [Paramétrage note de frais](../notes-de-frais/) et [Paramétrage engagement de dépense](../engagement-de-depense/).

Un document entre dans un circuit de validation `Prédéfini` de deux façons :

* manuellement : dans l'écran de pré-saisie comptable du menu `Bannettes`, l'utilisateur choisit le circuit dans le champ `Circuit de validation`, puis clique sur `Enregistrer` ;
* automatiquement : si le circuit a l'option `Mémoriser le circuit de validation pour les comptes tiers`, il s'applique aux prochains documents du même compte tiers.

## Prérequis

* Droit : dans INGENEO PRECOMPTA, la création d'un circuit de validation nécessite seulement le droit `Autoriser l’accès au paramétrage des processus métier`. Le détail des droits est dans [Détail des droits](../../administration/detail-des-droits.md).
* Statuts : pour appliquer des statuts pendant le circuit, créez d'abord les listes de statuts dans `Entreprises > Editer > Plan de classement > Processus métier > Statuts`. Voir [Configurer les statuts de documents](configurer-les-statuts-de-documents.md).
* Rôles du circuit : chaque utilisateur d'une étape reçoit un rôle. Les 5 rôles d'un circuit de validation dans INGENEO PRECOMPTA sont :
  * `Initiateur` : toujours au niveau 1. Il lance le circuit de validation, sans être obligé de faire la pré-saisie comptable. Le niveau 1 peut compter plusieurs initiateurs.
  * `Valideur` : il valide le document. Si plusieurs valideurs sont au même niveau, la première validation fait passer le document au niveau suivant. Si des valideurs ont l'interrupteur `Obliger`, le document ne passe au niveau suivant qu'après l'action de tous ces valideurs.
  * `Aiguilleur` : il choisit le valideur du niveau suivant. Le niveau suivant doit compter au moins deux valideurs. Sinon, le circuit est incomplet et aucun message d'erreur ne s'affiche.
  * `Observateur` : il suit l'avancement du document à tous les niveaux, sans pouvoir agir.
  * `Gestionnaire` : il suit l'avancement du document à tous les niveaux et peut faire toutes les actions à tous les niveaux.
* Le niveau `0` est réservé aux rôles `Observateur` et `Gestionnaire`.

## Étapes

1. Dans INGENEO PRECOMPTA, cliquez sur `Entreprises` dans le menu de gauche.
2. Sur la ligne de l'entreprise, cliquez sur `Editer`.
3. Cliquez sur l'onglet `Plan de classement`.
4. Cliquez sur `Processus métier`.
5. Cliquez sur `Circuits de validation`.
6. Cliquez sur `+ Ajouter`. Le panneau `Créer un circuit de validation` s'ouvre.
7. Dans `Type de circuit`, sélectionnez `Prédéfini`.
8. Cliquez sur `Enregistrer`. Le panneau `Edition d'un circuit` s'ouvre.
9. Dans le bloc `CONFIGURATION`, saisissez le nom dans `Nom du circuit de validation`.
10. Pour exporter le document vers le logiciel comptable après la validation finale, activez `Transférer en comptabilité lors de la validation finale`.
11. Pour appliquer automatiquement ce circuit aux prochains documents du même compte tiers, activez `Mémoriser le circuit de validation pour les comptes tiers`.
12. Dans `Classeurs`, sélectionnez un ou plusieurs classeurs.
13. Pour appliquer des statuts pendant le circuit, sélectionnez une ou plusieurs listes dans `Listes de statuts applicables`.
14. Dans le bloc `ETAPES`, sur la première ligne, saisissez `1` dans `Niveau`.
15. Sur la même ligne, sélectionnez l'utilisateur dans `Utilisateur(s)`.
16. Sur la même ligne, sélectionnez `Initiateur` dans `Rôle`.
17. Pour ajouter une ligne, cliquez sur le bouton `+` en haut à droite du bloc `ETAPES`.
18. Sur la nouvelle ligne, saisissez le niveau dans `Niveau`.
19. Sur la nouvelle ligne, sélectionnez l'utilisateur dans `Utilisateur(s)`.
20. Sur la nouvelle ligne, sélectionnez le rôle dans `Rôle`.
21. Si l'utilisateur doit agir pour que le document passe au niveau suivant, activez `Obliger` sur sa ligne.
22. Si l'utilisateur peut refuser le document, activez `Refuser` sur sa ligne.
23. Si `Refuser` est activé, choisissez l'effet du refus dans `Refuser et` : `Renvoyer à l'étape précédente`, `Arrêter le circuit de validation` ou `Envoyer à l'étape suivante`.
24. Si l'utilisateur peut modifier le document, activez `Modifier Info`.
25. Pour exporter le document vers le logiciel comptable à cette étape, activez `Export Compta`.
26. Pour régler les options de l'utilisateur, cliquez sur le bouton de la colonne `Autres`.
27. Activez les options voulues :
    * `Changer le circuit de validation` : autoriser la sélection d'un autre circuit dans le même classeur ;
    * `Changer le classeur` : autoriser la sélection d'un autre circuit dans un classeur différent de même type ;
    * `Activer la validation par mail` : avec cette option, l'utilisateur ne peut pas saisir de commentaire ;
    * `Obliger la saisie analytique` ;
    * `Obliger la saisie d’une note` ;
    * `Obliger l’ajout d’une pièce jointe` ;
    * `Appliquer la signature` ;
    * `Appliquer le tampon` ;
    * `Appliquer le statut après validation` ;
    * `Appliquer le statut après refus`.
28. Répétez les étapes 17 à 27 pour chaque utilisateur du circuit.
29. Cliquez sur `Enregistrer`.

## Résultat attendu

Dans INGENEO PRECOMPTA, le circuit apparaît dans la liste `Circuits de validation` de `Entreprises > Editer > Plan de classement > Processus métier`. Les colonnes sont `Type`, `Nom du circuit`, `Créé par`, `Date de création` et `Actions`.

Dans l'écran de pré-saisie comptable du menu `Bannettes`, le circuit est proposé dans le champ `Circuit de validation` pour les documents des classeurs associés. Le bouton de la colonne `Autres` affiche le nombre d'options activées pour l'utilisateur.

## Erreurs fréquentes

**L'`Aiguilleur` ne peut pas choisir de valideur.** Dans un circuit de validation d'INGENEO PRECOMPTA, le niveau qui suit un `Aiguilleur` doit compter au moins deux valideurs. L'application ne contrôle pas cette règle à l'enregistrement et n'affiche aucun message. Ajoutez au moins deux `Valideur` au niveau suivant.

**Le circuit n'est pas proposé dans le champ `Circuit de validation`.** Dans INGENEO PRECOMPTA, le champ `Circuit de validation` de l'écran de pré-saisie comptable ne propose que les circuits associés au classeur du document. Vérifiez le champ `Classeurs` du circuit.

**Le document ne peut pas être enregistré sans circuit.** Dans INGENEO PRECOMPTA, le classeur a l'option `Choix d’un circuit de validation obligatoire pour tous les documents` (classeur comptable > `Paramétrage avancé` > `VIGILANCE`). Chaque document de ce classeur doit passer par un circuit de validation.

**Un circuit en cours d'utilisation a été supprimé.** Dans INGENEO PRECOMPTA, les documents en attente de validation dans ce circuit restent visibles dans le menu `Rechercher`.

## Fiches liées

* [Configurer les statuts de documents](configurer-les-statuts-de-documents.md) : listes de statuts utilisées par `Listes de statuts applicables`.
* [Valider un document](../../gestion-des-documents/valider-un-document.md) : validation ou refus d'un document engagé dans un circuit.
* [Détail des droits](../../administration/detail-des-droits.md) : droit `Autoriser l’accès au paramétrage des processus métier`.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-creer-circuit-validation-ingeneo-precompta
* titre : Comment créer un circuit de validation dans INGENEO PRECOMPTA ?
* titre\_menu : Créer un circuit de validation
* type : procedure
* module : Processus métier
* version\_outil : 2.15.3 (version observée)
* roles\_concernes : utilisateur avec le droit `Autoriser l’accès au paramétrage des processus métier`
* tags : circuit de validation, workflow, valideur, initiateur, aiguilleur, statuts
* formulations\_utilisateur : « Comment mettre en place une validation des factures ? » ; « Comment ajouter un valideur ? » ; « À quoi sert l'aiguilleur ? » ; « Comment rendre une validation obligatoire ? » ; « Comment appliquer un circuit automatiquement à un fournisseur ? »
* sources : Refonte de la page GitBook ingeneo-pre-compta/processus-metiers/workflow/circuit-de-validation ; démo Arcade « Circuit de validation » ; observation de l'application INGENEO PRECOMPTA 2.15.3 (2026-10-30) ; réponses de l'expert 2026-10-30
* redacteur : CG
* relecteur :
* derniere\_verification : 2026-10-30
* statut : brouillon

</details>
