---
description: >-
  Créer un classeur comptable dans INGENEO PRECOMPTA et régler sa pré-saisie
  comptable : journal par défaut, doublons, éléments comptables et options
  avancées.
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

# Comment créer et paramétrer un classeur comptable dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de créer un classeur comptable pour une entreprise dans INGENEO PRECOMPTA et de régler la pré-saisie comptable de ses documents. Elle prend environ 4 minutes. Elle nécessite le droit `Autoriser l'accès au paramétrage de la comptabilité`.

## Objectif

Dans INGENEO PRECOMPTA, un classeur comptable regroupe les documents d'une entreprise selon leur type. Il apparaît dans le menu `Bannettes`. Son paramétrage s'applique à la pré-saisie comptable de tous ses documents, en trois onglets :

* `Paramétrage général` : ordre d'affichage, nom, journal par défaut et contrôle des doublons.
* `Eléments comptables` : champs affichés et obligatoires en pré-saisie comptable.
* `Paramétrage avancé` : outils IA, dépôt de document, enregistrement de document et alertes de vigilance.

Dans INGENEO PRECOMPTA, plusieurs classeurs du même type permettent d'automatiser des besoins distincts. Exemple : si 50 % des factures d'achat d'une entreprise sont en dollars, créez un second classeur `Factures d'achat` avec le dollar comme devise par défaut.

## Prérequis

* Droit de paramétrage : dans INGENEO PRECOMPTA, seul un utilisateur avec le droit [`Autoriser l'accès au paramétrage de la comptabilité`](../administration/detail-des-droits.md) peut créer et paramétrer un classeur comptable.
* Profil d'entreprise : si un utilisateur a un profil d'entreprise, attribuez-lui le droit `Gérer les référentiels associés (ajouter, modifier, supprimer)` sur chaque nouveau classeur. Ce réglage se fait dans `Entreprises > Editer > Administration > Profil d'entreprise`. Sans ce droit, l'utilisateur ne voit pas le bouton d'édition du classeur.
* Profil de site : un utilisateur avec un profil de site reçoit les droits associés au type du classeur. Si l'utilisateur a aussi un profil d'entreprise, le profil d'entreprise l'emporte.

## Étapes

### Créer un classeur comptable

{% hint style="warning" %}
Dans INGENEO PRECOMPTA, le type d'un classeur comptable ne peut plus être modifié après sa création. Pour changer de type, créez un nouveau classeur avec le bon type.
{% endhint %}

1. Dans INGENEO PRECOMPTA, cliquez sur `Entreprises` dans le menu de gauche.
2. Sur l'écran `Entreprises`, sur la ligne de l'entreprise, cliquez sur `Editer`.
3. Dans l'onglet `Entreprise`, cliquez sur `Classeurs comptables`.
4. Cliquez sur `Ajouter`.
5. Dans le panneau `Créer un classeur comptable`, saisissez un nom explicite dans le champ `Nom`.
6. Dans le champ `Type`, sélectionnez `Factures d'achat`, `Factures de vente`, `Caisse`, `Banque` ou `Notes de frais`.
7. Cliquez sur `Enregistrer`.

Le classeur est créé. Le panneau `Editer un classeur comptable` s'ouvre directement, avec les onglets `Paramétrage général`, `Eléments comptables` et `Paramétrage avancé`.

### Ouvrir le paramétrage d'un classeur existant

Dans INGENEO PRECOMPTA, le panneau `Editer un classeur comptable` s'ouvre de deux façons :

* Dans `Entreprises > Editer > Entreprise > Classeurs comptables`, cliquez sur le bouton d'édition (icône crayon orange) sur la ligne du classeur.
* Dans le menu `Bannettes`, sélectionnez l'entreprise et le classeur. Cliquez sur l'icône à 3 traits horizontaux, à droite entre les classeurs et les documents, puis sur `Paramétrage du classeur`.

### Régler le paramétrage général

Dans INGENEO PRECOMPTA, l'onglet `Paramétrage général` du panneau `Editer un classeur comptable` contient le bloc `CONFIGURATION` :

| Champ                                        | Effet                                                                                                                                                                                                                  |
| -------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Ordre d'affichage`                          | Position du classeur dans le menu `Bannettes` et dans la liste `Classeurs comptables` de l'entreprise.                                                                                                                 |
| `Nom`                                        | Nom du classeur.                                                                                                                                                                                                       |
| `Journal par défaut`                         | Obligatoire. Journal saisi automatiquement dans la pré-saisie comptable des documents du classeur, par exemple `ACH - Achats`.                                                                                         |
| `Contrôle des doublons (à l'enregistrement)` | `Par défaut` : contrôle sur `Compte tiers`, `Date de facture`, `Numéro de facture` (si renseigné) et `Montant`, ainsi que sur `Numéro de pièce`. `Paramétrable` : contrôle sur les éléments choisis par l'utilisateur. |

Avec `Paramétrable`, chaque paramètre réunit les éléments qui doivent être identiques pour identifier un doublon. Plusieurs paramètres peuvent être ajoutés : ils sont vérifiés en parallèle.

1. Dans le panneau `Editer un classeur comptable`, cliquez sur l'onglet `Paramétrage général`.
2. Sélectionnez l'`Ordre d'affichage`.
3. Sélectionnez le `Journal par défaut`.
4. Dans `Contrôle des doublons (à l'enregistrement)`, sélectionnez `Par défaut` ou `Paramétrable`.
5. Si vous avez sélectionné `Paramétrable`, cliquez sur `+` sous `Paramètres`.
6. Choisissez les éléments qui doivent être identiques pour identifier un doublon.
7. Cliquez sur `Enregistrer`.

### Choisir les éléments comptables

Dans INGENEO PRECOMPTA, l'onglet `Eléments comptables` du panneau `Editer un classeur comptable` règle les champs de la pré-saisie comptable du classeur :

* `Actif` : le champ est affiché en pré-saisie comptable.
* `Obligatoire` : la pré-saisie comptable ne peut pas être enregistrée si le champ est vide.
* `Autoriser la saisie sur les classes de compte :` et `Obliger la saisie sur les classes de compte :` : limitent le champ, ou le rendent obligatoire, aux lignes dont le compte commence par les classes choisies (par exemple 2, 6 ou 7). Ces réglages existent pour `PÉRIODICITÉ`, `CODES TVA` et `ANALYTIQUES`.

Les autres éléments de l'onglet sont `DATE D'ÉCHÉANCE`, `NUMÉRO DE PIÈCE`, `MODE DE RÈGLEMENT`, `COLLECTIF`, `ETABLISSEMENT`, `INFORMATION COMPLÉMENTAIRE`, `QUANTITÉ #1`, `QUANTITÉ #2` et `LIBELLÉ DE PIÈCE`. Cinq éléments ont un fonctionnement particulier :

| Élément              | Fonctionnement                                                                                                                                                            |
| -------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Libellé d'écriture` | Modèle du libellé d'écriture rempli automatiquement. Un clic droit dans le champ donne accès aux variables. `Majuscule obligatoire` met le libellé en majuscules.         |
| `NUMÉRO DE FACTURE`  | Toujours affiché. L'interrupteur `Obligatoire` le rend obligatoire ou facultatif.                                                                                         |
| Date de facture      | Toujours affichée et toujours obligatoire. Elle n'apparaît pas dans l'onglet.                                                                                             |
| `DEVISE`             | Une fois `Actif` activé, une liste déroulante des devises apparaît. La devise choisie devient la devise par défaut du classeur. Sans choix, la devise par défaut est EUR. |
| `ANALYTIQUES`        | Propose aussi `Axe analytique par défaut :` et `Section analytique par défaut niveau 1 :`.                                                                                |

1. Dans le panneau `Editer un classeur comptable`, cliquez sur l'onglet `Eléments comptables`.
2. Pour chaque élément à afficher, activez `Actif`.
3. Pour chaque élément à rendre obligatoire, activez `Obligatoire`.
4. Cliquez sur `Enregistrer`.

### Régler le paramétrage avancé du classeur

Dans INGENEO PRECOMPTA, l'onglet `Paramétrage avancé` du panneau `Editer un classeur comptable` est propre au classeur. Il est distinct de l'onglet `Comptabilité > Paramétrage avancé` de l'entreprise.

| Bloc                         | Interrupteur                                                                                                            | Effet quand il est activé                                                                                                                                                                                   |
| ---------------------------- | ----------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `OUTILS IA`                  | `Activer la comptabilisation par ligne d'article`                                                                       | Rend disponible l'option ligne par ligne sur un compte tiers. Cette option sert aux bénéfices agricoles.                                                                                                    |
| `DÉPÔT DE DOCUMENT`          | `Activer le découpage automatique`                                                                                      | Un PDF qui contient plusieurs factures est découpé en plusieurs documents au dépôt.                                                                                                                         |
| `DÉPÔT DE DOCUMENT`          | `Activer la détection des pages blanches`                                                                               | Les pages blanches sont supprimées au dépôt.                                                                                                                                                                |
| `DÉPÔT DE DOCUMENT`          | `Activer la rotation automatique de documents`                                                                          | Les pages mal orientées sont redressées au dépôt.                                                                                                                                                           |
| `DÉPÔT DE DOCUMENT`          | `Préfixer les noms de fichier avec la date de réception`                                                                | La date de réception est ajoutée au début du nom du fichier déposé.                                                                                                                                         |
| `ENREGISTREMENT DE DOCUMENT` | `Activer la fonction « Ne pas exporter »`                                                                               | En pré-saisie comptable, le document affiche l'interrupteur `Ne pas exporter`. Activé, il empêche l'export du document vers le logiciel comptable.                                                          |
| `VIGILANCE`                  | `Alerter si la date de facture supérieure à la date d’échéance`                                                         | Un avertissement s'affiche si la date de facture est postérieure à la date d'échéance.                                                                                                                      |
| `VIGILANCE`                  | `Afficher la validité de l’entreprise`                                                                                  | La pré-saisie comptable indique si l'entreprise du tiers est active ou radiée, d'après la base SIRENE.                                                                                                      |
| `VIGILANCE`                  | `Afficher les fenêtres d'avertissements lors de la détection d'une incohérence sur les lignes de TVA`                   | Un symbole d'attention (point d'exclamation dans un triangle) s'affiche sur la ligne de TVA incohérente avec les montants HT et TTC.                                                                        |
| `VIGILANCE`                  | `Contrôle IBAN sur les factures`                                                                                        | L'IBAN lu sur la facture est comparé à l'IBAN du compte tiers. Un écart est signalé.                                                                                                                        |
| `VIGILANCE`                  | `Afficher la fenêtre d'avertissement lorsque la date de facture n'est pas comprise dans la période d'exercice en cours` | Une fenêtre d'avertissement s'ouvre si la date de facture est hors de l'exercice ouvert. Elle propose de forcer l'export : le document prend alors la date du premier jour de la prochaine période ouverte. |
| `VIGILANCE`                  | `Choix d’un circuit de validation obligatoire pour tous les documents`                                                  | Chaque document du classeur doit passer par un circuit de validation avant l'export.                                                                                                                        |

1. Dans le panneau `Editer un classeur comptable`, cliquez sur l'onglet `Paramétrage avancé`.
2. Activez ou désactivez les interrupteurs voulus.
3. Cliquez sur `Enregistrer`.

### Dupliquer un classeur comptable

Dans INGENEO PRECOMPTA, ouvrez `Entreprises > Editer > Entreprise > Classeurs comptables`. Sur la ligne du classeur, cliquez sur le bouton de duplication (icône bleu foncé à deux rectangles). Le nouveau classeur reprend tout le paramétrage du classeur d'origine. Son type peut être choisi et tous ses paramètres restent modifiables.

### Supprimer un classeur comptable

{% hint style="warning" %}
Dans INGENEO PRECOMPTA, la suppression d'un classeur comptable propose de supprimer ses documents. Pour conserver les documents, choisissez de les déplacer dans un autre classeur.
{% endhint %}

1. Ouvrez `Entreprises > Editer > Entreprise > Classeurs comptables`.
2. Sur la ligne du classeur, cliquez sur le bouton de suppression (icône corbeille rouge).
3. Choisissez de supprimer les documents du classeur ou de les déplacer dans un autre classeur.

## Résultat attendu

Dans INGENEO PRECOMPTA, le classeur apparaît dans `Entreprises > Editer > Entreprise > Classeurs comptables` avec son type, son nom, son créateur et sa date de création. Il apparaît aussi dans le menu `Bannettes`, à la position définie par `Ordre d'affichage`. La pré-saisie comptable de ses documents applique le journal par défaut, les éléments comptables et les options du paramétrage avancé du classeur.

## Erreurs fréquentes

**Le type d'un classeur comptable ne peut pas être modifié.** Dans INGENEO PRECOMPTA, le type est fixé à la création du classeur. Créez un nouveau classeur avec le bon type. Le bouton de duplication permet de reprendre le paramétrage d'un classeur existant et de choisir un autre type.

**Le bouton d'édition d'un classeur comptable n'apparaît pas.** Dans INGENEO PRECOMPTA, l'utilisateur a un profil d'entreprise sans le droit `Gérer les référentiels associés (ajouter, modifier, supprimer)` sur ce classeur. Attribuez ce droit dans `Entreprises > Editer > Administration > Profil d'entreprise`.

**Impossible de créer ou de paramétrer un classeur comptable.** Dans INGENEO PRECOMPTA, l'utilisateur n'a pas le droit `Autoriser l'accès au paramétrage de la comptabilité`. Demandez à un administrateur d'ajouter ce droit à votre profil.

**L'enregistrement d'un document est bloqué comme doublon.** Dans INGENEO PRECOMPTA, le `Contrôle des doublons (à l'enregistrement)` du classeur a détecté un document identique. Cliquez sur le bouton en forme d'œil pour afficher les doublons. Pour changer les critères, sélectionnez `Paramétrable` dans l'onglet `Paramétrage général` du classeur.

**Un document n'est pas exporté vers le logiciel comptable.** Dans INGENEO PRECOMPTA, vérifiez que l'interrupteur `Ne pas exporter` du document est désactivé en pré-saisie comptable. Cet interrupteur n'existe que si `Activer la fonction « Ne pas exporter »` est activé dans le paramétrage avancé du classeur.

**La date d'un document a changé à l'export.** Dans INGENEO PRECOMPTA, la date de facture était hors de l'exercice ouvert et l'export a été forcé. Le document prend alors la date du premier jour de la prochaine période ouverte.

## Fiches liées

* [Paramétrage général de la comptabilité](parametrage-comptabilite.md) : logiciel comptable, code dossier, options générales et exercices de l'entreprise.
* [Créer une entreprise](creer-une-entreprise.md) : création de l'entreprise, avant le paramétrage de ses classeurs comptables.
* [Détail des droits](../administration/detail-des-droits.md) : droit `Autoriser l'accès au paramétrage de la comptabilité`.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-creer-parametrer-classeur-comptable-ingeneo-precompta
* titre : Comment créer et paramétrer un classeur comptable dans INGENEO PRECOMPTA ?
* titre\_menu : Créer et paramétrer un classeur comptable
* type : procedure
* module : Gestion des entreprises
* version\_outil : 2.11.0 (version observée)
* roles\_concernes : utilisateur avec le droit `Autoriser l'accès au paramétrage de la comptabilité`
* tags : classeur comptable, éléments comptables, doublons, journal par défaut, pré-saisie comptable, vigilance
* formulations\_utilisateur : « Comment créer un classeur comptable ? » ; « Je ne peux pas changer le type de mon classeur » ; « Je ne vois pas le bouton pour éditer le classeur » ; « Mon document est bloqué comme doublon » ; « Comment mettre une devise par défaut sur un classeur ? » ; « Comment rendre le numéro de facture obligatoire ? »
* sources : Refonte de la page GitBook ingeneo-pre-compta/gestion-des-entreprises/classeurs-comptables ; observation de l'application INGENEO PRECOMPTA 2.11.0 (2026-10-15) ; réponses de l'expert 2026-10-15
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-15
* statut : brouillon

</details>
