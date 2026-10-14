---
description: >-
  Dans INGENEO PRECOMPTA, le panneau Importer des entreprises crée plusieurs
  entreprises à partir d'un modèle Excel, puis importe leurs FEC dans un fichier
  zip.
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

# Comment créer plusieurs entreprises en une fois par import dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de créer plusieurs entreprises en une fois dans INGENEO PRECOMPTA, à partir d'un modèle Excel importé depuis l'écran `Entreprises`. Le traitement d'un import prend 5 à 15 minutes selon la volumétrie. Elle nécessite les droits `Autoriser la création d'entreprise` et `Autoriser l'accès au déploiement en masse`.

## Objectif

Dans INGENEO PRECOMPTA, l'import des entreprises crée plusieurs entreprises à partir d'un seul fichier Excel. C'est une alternative à la création une par une décrite dans [Créer une entreprise](creer-une-entreprise.md).

Une entreprise doit exister dans INGENEO PRECOMPTA avant de pouvoir traiter ses factures ou accéder à ses [paramètres avancés](parametrages-generaux.md).

Le même panneau `Importer des entreprises` permet ensuite d'importer en une fois les FEC de ces entreprises, dans un fichier zip.

## Prérequis

* Droits : l'utilisateur doit avoir le droit `Autoriser la création d'entreprise` et le droit `Autoriser l'accès au déploiement en masse`. Le détail des droits est dans [Détail des droits](../administration/detail-des-droits.md).
* Modèles d'entreprise : pour appliquer un modèle aux entreprises importées, créez-le avant l'import. La procédure est dans [Modèles d'entreprises](../administration/modeles-dentreprises.md).
* Codes dossier : préparez, pour chaque entreprise, le code dossier utilisé dans le logiciel comptable.
* FEC : si vous importez les FEC, préparez des fichiers FEC à jour, au format `.txt` conforme au format FEC. Le nom de chaque fichier doit commencer par le numéro SIREN de l'entreprise, par exemple `533951687FEC241101.txt`.
* Taille : un fichier importé dans le panneau `Importer des entreprises` ne doit pas dépasser 150 Mo. La limite s'applique au modèle Excel et au fichier zip de FEC.

{% hint style="danger" %}
Dans le modèle Excel d'import des entreprises d'INGENEO PRECOMPTA, la colonne `Code` doit contenir un code identique au code dossier du logiciel comptable. Sinon, la migration des données entre INGENEO PRECOMPTA et le logiciel comptable n'est pas possible.
{% endhint %}

## Étapes

### Télécharger le modèle d'import

1. Dans INGENEO PRECOMPTA, cliquez sur `Entreprises` dans le menu de gauche.
2. Sur l'écran `Entreprises`, cliquez sur `Actions`.
3. Dans la rubrique `DÉPLOIEMENT`, cliquez sur `Importer des entreprises`.
4. Dans le panneau `Importer des entreprises`, partie `IMPORTER DES ENTREPRISES`, cliquez sur `Télécharger le modèle`.

### Remplir le modèle d'import

Le modèle Excel d'INGENEO PRECOMPTA contient un onglet `Entreprises`. Remplissez une ligne par entreprise, à partir de la ligne 2. Les colonnes avec une liste proposent les valeurs disponibles dans un menu déroulant : choisissez une valeur de cette liste.

Les listes des colonnes `Logiciel comptable`, `Modèle` et `Site` dépendent du paramétrage de votre plateforme INGENEO PRECOMPTA. Téléchargez donc le modèle depuis la plateforme sur laquelle vous importez.

| Colonne du modèle                        | Obligatoire | Saisie         | Remarques                                                                                                                                                                                                                                                                                 |
| ---------------------------------------- | ----------- | -------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Logiciel comptable`                     | Oui         | Menu déroulant | Logiciel comptable de l'entreprise.                                                                                                                                                                                                                                                       |
| `SIREN`                                  | Oui         | Saisie libre   | Numéro SIREN de l'entreprise.                                                                                                                                                                                                                                                             |
| `Raison sociale`                         | Oui         | Saisie libre   | Raison sociale de l'entreprise.                                                                                                                                                                                                                                                           |
| `Code`                                   | Oui         | Saisie libre   | Doit être identique au code dossier du logiciel comptable.                                                                                                                                                                                                                                |
| `Modèle`                                 | Non         | Menu déroulant | Modèle d'entreprise à appliquer. La liste contient les modèles existants de la plateforme.                                                                                                                                                                                                |
| `Code achat`                             | Non         | Saisie libre   | Code comptable affecté au classeur des achats. Pris en compte uniquement si la colonne `Modèle` est vide.                                                                                                                                                                                 |
| `Code vente`                             | Non         | Saisie libre   | Code comptable affecté au classeur des ventes. Pris en compte uniquement si la colonne `Modèle` est vide.                                                                                                                                                                                 |
| `Site`                                   | Oui         | Menu déroulant | Site de rattachement de l'entreprise.                                                                                                                                                                                                                                                     |
| `Mode de facturation`                    | Oui         | Menu déroulant | Valeurs du modèle : `Partage documentaire`, `SCI/LMNP/BNC`, `BNC`, `BIC 50 factures/an`, `BIC 150 factures/an`, `BIC 1000 factures/an`, `BIC 5000 factures/an`.                                                                                                                           |
| `Date de fin d'exercice (jj/MM)`         | Oui         | Saisie libre   | Format jour/mois. La valeur la plus courante est 31/12.                                                                                                                                                                                                                                   |
| `Lancer la synchronisation après import` | Non         | Menu déroulant | Valeurs : `Oui` ou `Non`. Avec `Oui`, la synchronisation récupère les référentiels comptables depuis le logiciel comptable. Elle n'est pas disponible pour tous les logiciels comptables interconnectés à INGENEO PRECOMPTA. Si la colonne est vide, la synchronisation n'est pas lancée. |

### Importer le modèle rempli

1. Dans INGENEO PRECOMPTA, ouvrez le panneau `Importer des entreprises` depuis `Entreprises > Actions > Importer des entreprises`.
2. Dans la partie `IMPORTER DES ENTREPRISES`, cliquez sur `Importer un fichier`.
3. Dans la fenêtre de votre ordinateur, sélectionnez le modèle Excel rempli.

INGENEO PRECOMPTA affiche le message `Vous serez notifié par mail lors de la fin du process d'import de votre fichier.` À la fin du traitement, l'utilisateur qui a importé le fichier reçoit un email avec le résultat de l'import. Le traitement prend 5 à 15 minutes selon la volumétrie.

### Importer les FEC des entreprises (conseillé)

Dans INGENEO PRECOMPTA, l'import des FEC est conseillé après l'import des entreprises. Il crée les [référentiels comptables](referentiels-comptables.md) de chaque entreprise : codes journaux, comptes de tiers et comptes comptables. Il récupère aussi les occurrences, pour que les propositions de saisie soient adaptées dès le début de la saisie.

1. Regroupez les fichiers FEC dans un fichier zip. Le nom de chaque fichier FEC doit commencer par le numéro SIREN de l'entreprise.
2. Dans INGENEO PRECOMPTA, ouvrez le panneau `Importer des entreprises` depuis `Entreprises > Actions > Importer des entreprises`.
3. Dans la partie `IMPORTER DES FICHIERS FEC`, cliquez sur `Importer un fichier (zip)`.
4. Dans la fenêtre de votre ordinateur, sélectionnez le fichier zip.

Le résultat de l'import des FEC est envoyé par email à l'utilisateur qui a importé le fichier zip. Si plusieurs entreprises ont le même numéro SIREN, le FEC est intégré à chacune de ces entreprises.

## Résultat attendu

Dans INGENEO PRECOMPTA, après l'import du modèle Excel, le message `Vous serez notifié par mail lors de la fin du process d'import de votre fichier.` s'affiche. L'utilisateur qui a importé le fichier reçoit ensuite un email avec le résultat de l'import.

Les entreprises importées apparaissent dans la liste de l'écran `Entreprises` dès que l'import est validé. Les lignes rejetées sont listées dans l'email de résultat, avec la raison du rejet.

Avant de traiter les factures, vérifiez la cohérence des données importées pour chaque entreprise. Pour modifier les paramètres d'une entreprise après l'import, ouvrez ses [paramètres avancés](parametrages-generaux.md) depuis l'écran `Entreprises`.

## Erreurs fréquentes

**Ligne rejetée à l'import des entreprises.** Dans INGENEO PRECOMPTA, une ligne en erreur du modèle Excel est rejetée seule : les autres lignes sont importées. L'email de résultat indique la raison du rejet. Corrigez les lignes rejetées dans le fichier, puis réimportez le fichier complet. L'import reconnaît une entreprise déjà existante à son code dossier, saisi dans la colonne `Code`. Les lignes dont le code dossier existe déjà sont ignorées : l'import ne crée pas de doublon.

**Colonne obligatoire vide dans le modèle d'import des entreprises.** Dans INGENEO PRECOMPTA, les colonnes `Logiciel comptable`, `SIREN`, `Raison sociale`, `Code`, `Site`, `Mode de facturation` et `Date de fin d'exercice (jj/MM)` sont obligatoires. Complétez-les pour chaque ligne avant d'importer le fichier.

**`Code achat` ou `Code vente` non appliqué.** Dans le modèle d'import des entreprises d'INGENEO PRECOMPTA, les colonnes `Code achat` et `Code vente` sont ignorées quand la colonne `Modèle` est renseignée. Pour qu'elles soient prises en compte, laissez la colonne `Modèle` vide.

**Valeur saisie hors liste.** Dans le modèle d'import des entreprises d'INGENEO PRECOMPTA, les colonnes `Logiciel comptable`, `Modèle`, `Site`, `Mode de facturation` et `Lancer la synchronisation après import` attendent une valeur de leur menu déroulant. Sélectionnez la valeur dans la liste au lieu de la saisir. Utilisez un modèle téléchargé depuis la plateforme sur laquelle vous importez.

**Erreur à l'import des FEC.** Dans INGENEO PRECOMPTA, chaque FEC doit être un fichier `.txt` conforme au format FEC, avec les codes journaux renseignés. Le nom de chaque fichier doit commencer par le numéro SIREN de l'entreprise.

**Fichier refusé à cause de sa taille.** Dans INGENEO PRECOMPTA, le modèle Excel et le fichier zip de FEC ne doivent pas dépasser 150 Mo chacun.

## Fiches liées

* [Créer une entreprise](creer-une-entreprise.md) : création d'une seule entreprise depuis `Entreprises > Ajouter`.
* [Modèles d'entreprises](../administration/modeles-dentreprises.md) : créer le modèle choisi dans la colonne `Modèle`.
* [Référentiels comptables](referentiels-comptables.md) : référentiels créés par l'import des FEC et par la synchronisation.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-creer-entreprises-en-masse-ingeneo-precompta
* titre\_menu : Créer des entreprises par import
* titre : Comment créer plusieurs entreprises en une fois par import dans INGENEO PRECOMPTA ?
* type : procedure
* module : Gestion des entreprises
* version\_outil : toutes
* roles\_concernes : utilisateur avec les droits `Autoriser la création d'entreprise` et `Autoriser l'accès au déploiement en masse`
* tags : import, entreprises, création en masse, modèle Excel, FEC, déploiement
* formulations\_utilisateur : « Comment créer des entreprises en masse ? » ; « Importer plusieurs dossiers d'un coup » ; « Où trouver le modèle d'import des entreprises ? » ; « Importer plusieurs FEC en zip »
* sources : Refonte de la page GitBook ingeneo-pre-compta/gestion-des-entreprises/creer-une-entreprise-1 ; observation de l'application INGENEO PRECOMPTA (2026-10-13) ; modèle Excel d'import des entreprises ; réponses de l'expert 2026-10-13
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-13
* statut : brouillon

</details>
