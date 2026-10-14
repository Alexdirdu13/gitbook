---
description: >-
  Dans INGENEO PRECOMPTA, l'onglet Paramétrage général du menu Comptabilité
  d'une entreprise définit le logiciel comptable, le code dossier, les options
  générales et les exercices.
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

# Comment faire le paramétrage général de la comptabilité d'une entreprise dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de définir le logiciel comptable, le code dossier, les options générales et les exercices d'une entreprise dans INGENEO PRECOMPTA. Elle prend environ 3 minutes. Elle nécessite le droit `Autoriser l'accès au paramétrage de la comptabilité`.

## Objectif

Dans INGENEO PRECOMPTA, l'onglet `Paramétrage général` du menu `Comptabilité` d'une entreprise se trouve dans `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage général`. Il contient trois blocs :

* `LOGICIEL COMPTABLE` : le logiciel comptable de l'entreprise et son code dossier, utilisés pour la synchronisation des référentiels et l'export des données.
* `PARAMÉTRAGE GÉNÉRAL` : le type de comptabilité, le régime de déclaration de TVA et trois options.
* `EXERCICES` : la date de fin d'exercice et la liste des exercices de l'entreprise.

Utilisez cette procédure dans les cas suivants :

* configuration initiale après la [création d'une entreprise](creer-une-entreprise.md) ;
* changement de logiciel comptable, ou mise à jour majeure du logiciel comptable ;
* modification du régime fiscal ou du type de comptabilité de l'entreprise ;
* création ou clôture d'un exercice.

Les comptes fournisseurs et clients, le plan comptable, l'export comptable et l'analytique se paramètrent dans l'onglet `Paramétrage avancé`, décrit dans [Paramétrage avancé de la comptabilité](parametrage-comptabilite-avance.md).

## Prérequis

* Droit : l'utilisateur doit avoir le droit `Autoriser l'accès au paramétrage de la comptabilité`. Sans ce droit, le menu `Comptabilité` de l'entreprise est masqué. Le détail des droits est dans [Détail des droits](../administration/detail-des-droits.md).
* Code dossier : relevez le code dossier de l'entreprise dans le logiciel comptable. Le code saisi dans INGENEO PRECOMPTA doit être strictement identique, espaces et caractères spéciaux compris.
* Logiciel comptable : vérifiez la version et les paramètres du logiciel comptable avant la configuration.

{% hint style="warning" %}
Dans INGENEO PRECOMPTA, une mauvaise configuration du menu `Comptabilité` d'une entreprise peut compromettre l'export vers le logiciel comptable. Ne modifiez pas ce paramétrage en cours d'exercice sans l'accord préalable de l'expert-comptable. Ne le modifiez pas non plus pendant les périodes de clôture ou de déclarations fiscales.
{% endhint %}

## Étapes

### Ouvrir le paramétrage général de la comptabilité

1. Dans INGENEO PRECOMPTA, cliquez sur `Entreprises` dans le menu de gauche.
2. Sur l'écran `Entreprises`, sur la ligne de l'entreprise, cliquez sur `Editer`.
3. Dans l'onglet `Entreprise`, cliquez sur `Comptabilité`.

L'onglet `Paramétrage général` s'affiche.

### Choisir le logiciel comptable et le code dossier

Dans INGENEO PRECOMPTA, le bloc `LOGICIEL COMPTABLE` contient les champs `Logiciel` et `Code dossier`. Le `Code dossier` doit être identique à celui du logiciel comptable, pour permettre la synchronisation des référentiels et l'export des données. Quand la technologie de connexion au logiciel comptable le permet, le plus souvent une API, le code dossier est proposé dans une liste.

1. Ouvrez `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage général`.
2. Dans le champ `Logiciel`, sélectionnez le logiciel comptable de l'entreprise.
3. Si le champ `Code dossier` propose une liste, sélectionnez le dossier de l'entreprise.
4. Si le champ `Code dossier` ne propose pas de liste, saisissez le code dossier du logiciel comptable.
5. Cliquez sur `Enregistrer`.

Pour modifier le code dossier à la main, cliquez sur l'icône crayon à droite du champ `Code dossier`, saisissez le code, puis cliquez sur `Enregistrer`.

### Renseigner les options générales

Dans INGENEO PRECOMPTA, le bloc `PARAMÉTRAGE GÉNÉRAL` de l'onglet `Comptabilité > Paramétrage général` contient les champs suivants :

| Champ                                                      | Valeurs                                                                                                   | Effet                                                                                                                                                                                         |
| ---------------------------------------------------------- | --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Type de comptabilité`                                     | `Comptabilité d'engagement`, `Comptabilité de trésorerie`                                                 | Information sur l'entreprise. À ce jour, aucun effet sur la pré-saisie ni sur l'export.                                                                                                       |
| `Régime de déclaration de TVA`                             | `CA3 mensuel`, `CA3 trimestre`, `Annuel RSI`, `Annuel agricole`, `Acompte de RSI`, `Remboursement de TVA` | Information sur l'entreprise. À ce jour, aucun effet sur la pré-saisie ni sur l'export.                                                                                                       |
| `Entreprise non assujettie à la TVA.`                      | Interrupteur                                                                                              | Activé : INGENEO PRECOMPTA ne propose plus de ligne de TVA.                                                                                                                                   |
| `Inclure les comptes inactifs lors de la synchronisation.` | Interrupteur                                                                                              | Activé : la synchronisation des référentiels inclut les comptes inactifs du logiciel comptable. S'applique quand la synchronisation est possible, notamment avec une interconnexion par API.  |
| `Clôture par situation`                                    | Interrupteur                                                                                              | Activé : les journaux comptables se clôturent par situation, comme un exercice mais sur une période choisie. L'utilisateur choisit le journal et sa date de clôture dans le menu `Bannettes`. |

1. Ouvrez `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage général`.
2. Dans le bloc `PARAMÉTRAGE GÉNÉRAL`, modifiez le champ ou l'interrupteur voulu.
3. Cliquez sur `Enregistrer`.

### Créer un exercice

Dans INGENEO PRECOMPTA, le champ `Date de fin d'exercice` du bloc `EXERCICES` (par exemple `31/12`) sert à calculer les dates de l'exercice créé avec le bouton `+`. Une entreprise peut avoir au maximum 2 exercices ouverts en même temps.

1. Ouvrez `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage général`.
2. Dans le bloc `EXERCICES`, vérifiez la valeur du champ `Date de fin d'exercice`.
3. Cliquez sur le bouton `+` sous la liste des exercices.
4. Vérifiez les champs `Date de début` et `Date de fin` de la nouvelle ligne.
5. Cliquez sur `Enregistrer`.

Si 2 exercices sont déjà ouverts, le message `Seules 2 périodes d'exercice ouvertes simultanément sont autorisées` s'affiche. Clôturez d'abord l'exercice le plus ancien.

### Clôturer un exercice

1. Ouvrez `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage général`.
2. Dans le bloc `EXERCICES`, sur la ligne de l'exercice, activez l'interrupteur `Clôturé`.
3. Cliquez sur `Enregistrer`.

## Résultat attendu

Dans INGENEO PRECOMPTA, après un clic sur `Enregistrer` dans `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage général`, le paramétrage est conservé pour l'entreprise.

* Le logiciel comptable et le code dossier enregistrés servent à la synchronisation des référentiels et à l'export des données.
* Un nouvel exercice apparaît dans la liste du bloc `EXERCICES`, avec ses dates de début et de fin.
* Un exercice clôturé affiche l'interrupteur `Clôturé` activé dans le bloc `EXERCICES`.

## Erreurs fréquentes

**Le menu `Comptabilité` n'apparaît pas.** Dans INGENEO PRECOMPTA, le menu `Comptabilité` d'une entreprise n'est visible qu'avec le droit `Autoriser l'accès au paramétrage de la comptabilité`. Demandez à un administrateur d'ajouter ce droit à votre profil. Le détail des droits est dans [Détail des droits](../administration/detail-des-droits.md).

**La synchronisation ou l'export échoue systématiquement.** Dans INGENEO PRECOMPTA, onglet `Comptabilité > Paramétrage général`, vérifiez que le `Code dossier` est strictement identique à celui du logiciel comptable, espaces et caractères spéciaux compris. Vérifiez ensuite les paramètres du logiciel comptable.

**Le message `Seules 2 périodes d'exercice ouvertes simultanément sont autorisées` s'affiche.** Dans INGENEO PRECOMPTA, une entreprise accepte au maximum 2 exercices ouverts. Dans le bloc `EXERCICES` de l'onglet `Comptabilité > Paramétrage général`, activez l'interrupteur `Clôturé` de l'exercice le plus ancien, puis cliquez sur `Enregistrer`. Créez ensuite le nouvel exercice avec le bouton `+`.

**Les comptes inactifs du logiciel comptable n'arrivent pas dans INGENEO PRECOMPTA.** Par défaut, la synchronisation des référentiels n'inclut pas les comptes inactifs. Dans l'onglet `Comptabilité > Paramétrage général`, activez `Inclure les comptes inactifs lors de la synchronisation.`, puis cliquez sur `Enregistrer`.

**Aucune ligne de TVA n'est proposée.** Dans INGENEO PRECOMPTA, l'interrupteur `Entreprise non assujettie à la TVA.` supprime les lignes de TVA. Si l'entreprise est assujettie à la TVA, désactivez cet interrupteur dans l'onglet `Comptabilité > Paramétrage général`, puis cliquez sur `Enregistrer`.

## Fiches liées

* [Paramétrage avancé de la comptabilité](parametrage-comptabilite-avance.md) : comptes fournisseurs et clients, plan comptable, export comptable et analytique.
* [Créer une entreprise](creer-une-entreprise.md) : création de l'entreprise, avant son paramétrage comptable.
* [Détail des droits](../administration/detail-des-droits.md) : droit `Autoriser l'accès au paramétrage de la comptabilité`.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-parametrer-comptabilite-general-entreprise-ingeneo-precompta
* titre : Comment faire le paramétrage général de la comptabilité d'une entreprise dans INGENEO PRECOMPTA ?
* titre\_menu : Paramétrage général de la comptabilité
* type : procedure
* module : Gestion des entreprises
* version\_outil : 2.11.0 (version observée)
* roles\_concernes : utilisateur avec le droit `Autoriser l'accès au paramétrage de la comptabilité`
* tags : comptabilité, logiciel comptable, code dossier, exercice, clôture, TVA
* formulations\_utilisateur : « Où renseigner le code dossier d'une entreprise ? » ; « Comment changer de logiciel comptable pour un dossier ? » ; « Ma synchronisation échoue systématiquement » ; « Comment clôturer un exercice ? » ; « Seules 2 périodes d'exercice ouvertes simultanément sont autorisées » ; « Comment ouvrir un nouvel exercice ? »
* sources : Refonte de la page GitBook ingeneo-pre-compta/gestion-des-entreprises/parametrage-comptabilite ; observation de l'application INGENEO PRECOMPTA 2.11.0 (2026-10-14) ; réponses de l'expert 2026-10-14
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-14
* statut : brouillon

</details>
