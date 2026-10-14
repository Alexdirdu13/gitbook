---
description: >-
  Dans INGENEO PRECOMPTA, l'onglet Paramétrage avancé du menu Comptabilité d'une
  entreprise règle la création des comptes fournisseurs et clients, le plan
  comptable, l'export comptable et l'analytique.
---

# Comment faire le paramétrage avancé de la comptabilité d'une entreprise dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de régler la création des comptes fournisseurs et clients, le plan comptable, l'export comptable, les options avancées et l'analytique d'une entreprise dans INGENEO PRECOMPTA. Elle prend environ 3 minutes. Elle nécessite le droit `Autoriser l'accès au paramétrage de la comptabilité`.

## Objectif

Dans INGENEO PRECOMPTA, l'onglet `Paramétrage avancé` du menu `Comptabilité` d'une entreprise se trouve dans `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage avancé`. Ces réglages agissent sur les automatisations de la pré-saisie comptable et sur l'export. L'onglet contient sept blocs :

* `PROTECTION DU LOGICIEL COMPTABLE` : identifiants d'une protection supplémentaire de l'entreprise dans le logiciel comptable.
* `PARAMÉTRAGE DES COMPTES FOURNISSEURS` : règles de création des comptes fournisseurs.
* `PARAMÉTRAGE DES COMPTES CLIENTS` : règles de création des comptes clients.
* `PARAMÉTRAGE DU PLAN COMPTABLE` : longueur des comptes du plan comptable.
* `EXPORT COMPTABLE` : éléments apposés sur le PDF du document exporté.
* `AVANCÉS` : comptes de TVA identiques et saisie à 0 €.
* `PARAMÉTRAGE DE L'ANALYTIQUE` : intitulés des sections analytiques.

Utilisez cette procédure dans les cas suivants :

* configuration initiale après la [création d'une entreprise](creer-une-entreprise.md) ;
* automatisation de la création des comptes fournisseurs et clients ;
* optimisation des automatisations de la pré-saisie comptable.

Le logiciel comptable, le code dossier et les exercices se paramètrent dans l'onglet `Paramétrage général`, décrit dans [Paramétrage général de la comptabilité](parametrage-comptabilite.md).

## Prérequis

* Droit : l'utilisateur doit avoir le droit `Autoriser l'accès au paramétrage de la comptabilité`. Ce droit donne accès aux onglets `Paramétrage général` et `Paramétrage avancé`. Sans ce droit, le menu `Comptabilité` de l'entreprise est masqué. Le détail des droits est dans [Détail des droits](../administration/detail-des-droits.md).
* Règles de numérotation : préparez le préfixe et les longueurs de comptes utilisés pour l'entreprise dans le logiciel comptable.

{% hint style="warning" %}
Dans INGENEO PRECOMPTA, une mauvaise configuration du menu `Comptabilité` d'une entreprise peut compromettre l'export vers le logiciel comptable. Ne modifiez pas ce paramétrage en cours d'exercice sans l'accord préalable de l'expert-comptable. Ne le modifiez pas non plus pendant les périodes de clôture ou de déclarations fiscales.
{% endhint %}

## Étapes

### Ouvrir le paramétrage avancé de la comptabilité

1. Dans INGENEO PRECOMPTA, cliquez sur `Entreprises` dans le menu de gauche.
2. Sur l'écran `Entreprises`, sur la ligne de l'entreprise, cliquez sur `Editer`.
3. Dans l'onglet `Entreprise`, cliquez sur `Comptabilité`.
4. Cliquez sur l'onglet `Paramétrage avancé`.

### Renseigner la protection du logiciel comptable

Dans INGENEO PRECOMPTA, le bloc `PROTECTION DU LOGICIEL COMPTABLE` de l'onglet `Comptabilité > Paramétrage avancé` contient les champs `Nom d'utilisateur`, `Mot de passe` et `Code PIN`. Ces champs servent dans un cas très spécifique. Contactez le support INGENEO avant de les remplir.

### Paramétrer la création des comptes fournisseurs et clients

Dans INGENEO PRECOMPTA, onglet `Comptabilité > Paramétrage avancé`, les blocs `PARAMÉTRAGE DES COMPTES FOURNISSEURS` et `PARAMÉTRAGE DES COMPTES CLIENTS` contiennent les mêmes champs. Chaque bloc s'applique à son type de compte tiers.

| Champ                                                               | Effet                                                                                                                                                                                                                                                                                                                        |
| ------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Obliger la saisie d'un collectif lors de la création d'un compte.` | Interrupteur sous `Compte collectif`. Activé : la création d'un compte tiers sans compte collectif affiche le message `Compte collectif obligatoire`.                                                                                                                                                                        |
| `Prefixe des comptes`                                               | Préfixe des comptes tiers créés automatiquement, par exemple `F` pour les fournisseurs.                                                                                                                                                                                                                                      |
| `Mode d'auto-complétion`                                            | `Non défini` : aucune règle, l'utilisateur saisit le numéro de compte de son choix. `Intitulé INSEE (Construire à partir de l'intitulé INSEE)` : le compte est construit à partir de l'intitulé INSEE. `Numérique (Construire à partir de numéro incrémentiel)` : le compte est construit à partir d'un numéro incrémentiel. |
| `Longueur des comptes min.` et `Longueur des comptes max.`          | Nombre minimum et maximum de caractères des comptes tiers. S'appliquent aux modes `Intitulé INSEE` et `Numérique`.                                                                                                                                                                                                           |
| `Obliger la saisie des informations sur l'entreprise.`              | Interrupteur. Activé : la création d'un compte tiers exige le SIREN et l'IBAN du tiers.                                                                                                                                                                                                                                      |

1. Ouvrez `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage avancé`.
2. Dans le bloc `PARAMÉTRAGE DES COMPTES FOURNISSEURS`, renseignez les champs voulus.
3. Dans le bloc `PARAMÉTRAGE DES COMPTES CLIENTS`, renseignez les champs voulus.
4. Cliquez sur `Enregistrer`.

Pour automatiser la création des comptes tiers, utilisez un préfixe cohérent et des longueurs de comptes identiques pour toutes les entreprises de votre organisation.

### Paramétrer la longueur des comptes du plan comptable

Dans INGENEO PRECOMPTA, le bloc `PARAMÉTRAGE DU PLAN COMPTABLE` de l'onglet `Comptabilité > Paramétrage avancé` contient l'interrupteur `Compléter avec des 0 pour atteindre la taille définie.` et les champs `Longueur des comptes min.` et `Longueur des comptes max.`.

Quand l'interrupteur est activé, les comptes créés dans INGENEO PRECOMPTA sont complétés par des « 0 » jusqu'à la `Longueur des comptes min.`. Par exemple, avec une longueur minimum de 8, le compte `6064` devient `60640000`. Les comptes reçus par la synchronisation ne sont pas complétés.

1. Ouvrez `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage avancé`.
2. Dans le bloc `PARAMÉTRAGE DU PLAN COMPTABLE`, saisissez la `Longueur des comptes min.`.
3. Saisissez la `Longueur des comptes max.`.
4. Si les comptes doivent être complétés par des « 0 », activez `Compléter avec des 0 pour atteindre la taille définie.`.
5. Cliquez sur `Enregistrer`.

### Choisir les éléments apposés sur le PDF exporté

Dans INGENEO PRECOMPTA, le bloc `EXPORT COMPTABLE` de l'onglet `Comptabilité > Paramétrage avancé` propose trois interrupteurs sous `Options sur les documents`. Chaque interrupteur activé appose l'élément correspondant sur le PDF du document envoyé au logiciel comptable avec l'écriture :

* `Inclure les tampons.` : les tampons, marques visuelles posées sur le document avec l'outil tampon.
* `Inclure les notes.` : les notes du document.
* `Inclure le surlignage.` : les surlignages du document.

1. Ouvrez `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage avancé`.
2. Dans le bloc `EXPORT COMPTABLE`, activez les interrupteurs voulus.
3. Cliquez sur `Enregistrer`.

### Régler les options avancées

Dans INGENEO PRECOMPTA, le bloc `AVANCÉS` de l'onglet `Comptabilité > Paramétrage avancé` contient deux interrupteurs :

| Interrupteur                                           | Activé                                                                                                                             | Désactivé                                                                   |
| ------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------- |
| `Interdire l'ajout d'un 2eme compte de TVA identique.` | À l'export, les lignes d'une écriture sur le même compte de TVA sont fusionnées en une seule ligne, avec les montants additionnés. | À l'export, une écriture peut contenir 2 lignes avec le même compte de TVA. |
| `Autoriser la saisie à 0€.`                            | La pré-saisie comptable d'une écriture à 0 € est possible.                                                                         | Une écriture à 0 € et son document ne peuvent pas être exportés.            |

1. Ouvrez `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage avancé`.
2. Dans le bloc `AVANCÉS`, activez ou désactivez l'interrupteur voulu.
3. Cliquez sur `Enregistrer`.

### Personnaliser les intitulés des sections analytiques

Dans INGENEO PRECOMPTA, le bloc `PARAMÉTRAGE DE L'ANALYTIQUE` de l'onglet `Comptabilité > Paramétrage avancé` propose 10 champs, de `Section #1` à `Section #10`. Le texte saisi dans un champ remplace l'intitulé de la section dans la pré-saisie comptable. Un champ vide garde l'intitulé par défaut, par exemple `Section #1`.

1. Ouvrez `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage avancé`.
2. Dans le bloc `PARAMÉTRAGE DE L'ANALYTIQUE`, saisissez l'intitulé de chaque section utilisée.
3. Cliquez sur `Enregistrer`.

## Résultat attendu

Dans INGENEO PRECOMPTA, après un clic sur `Enregistrer` dans `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage avancé`, le paramétrage est conservé pour l'entreprise.

* Les comptes fournisseurs et clients créés suivent le préfixe, le mode d'auto-complétion et les longueurs définis.
* Les comptes du plan comptable créés dans INGENEO PRECOMPTA respectent les longueurs définies.
* Les PDF exportés portent les tampons, notes et surlignages choisis.
* La pré-saisie comptable affiche les intitulés personnalisés des sections analytiques.

## Erreurs fréquentes

**Le menu `Comptabilité` n'apparaît pas.** Dans INGENEO PRECOMPTA, le menu `Comptabilité` d'une entreprise n'est visible qu'avec le droit `Autoriser l'accès au paramétrage de la comptabilité`. Demandez à un administrateur d'ajouter ce droit à votre profil. Le détail des droits est dans [Détail des droits](../administration/detail-des-droits.md).

**Le message `Compte collectif obligatoire` s'affiche à la création d'un compte tiers.** Dans INGENEO PRECOMPTA, l'interrupteur `Obliger la saisie d'un collectif lors de la création d'un compte.` est activé pour ce type de compte. Renseignez le compte collectif du tiers. Pour retirer l'obligation, désactivez l'interrupteur dans l'onglet `Comptabilité > Paramétrage avancé`, puis cliquez sur `Enregistrer`.

**La création d'un compte tiers demande le SIREN et l'IBAN.** Dans INGENEO PRECOMPTA, l'interrupteur `Obliger la saisie des informations sur l'entreprise.` est activé pour ce type de compte. Renseignez le SIREN et l'IBAN du tiers. Pour retirer l'obligation, désactivez l'interrupteur dans l'onglet `Comptabilité > Paramétrage avancé`, puis cliquez sur `Enregistrer`.

**Deux lignes sur le même compte de TVA sont fusionnées à l'export.** Dans INGENEO PRECOMPTA, l'interrupteur `Interdire l'ajout d'un 2eme compte de TVA identique.` est activé. Les montants sont additionnés sur une seule ligne. Pour exporter des lignes séparées, désactivez l'interrupteur dans le bloc `AVANCÉS`, puis cliquez sur `Enregistrer`.

**Une écriture à 0 € et son document ne s'exportent pas.** Dans INGENEO PRECOMPTA, l'interrupteur `Autoriser la saisie à 0€.` est désactivé. Activez-le dans le bloc `AVANCÉS` de l'onglet `Comptabilité > Paramétrage avancé`, puis cliquez sur `Enregistrer`.

**Les tampons, notes ou surlignages n'apparaissent pas sur le PDF exporté.** Dans INGENEO PRECOMPTA, activez `Inclure les tampons.`, `Inclure les notes.` ou `Inclure le surlignage.` dans le bloc `EXPORT COMPTABLE` de l'onglet `Comptabilité > Paramétrage avancé`, puis cliquez sur `Enregistrer`.

## Fiches liées

* [Paramétrage général de la comptabilité](parametrage-comptabilite.md) : logiciel comptable, code dossier, options générales et exercices.
* [Créer une entreprise](creer-une-entreprise.md) : création de l'entreprise, avant son paramétrage comptable.
* [Détail des droits](../administration/detail-des-droits.md) : droit `Autoriser l'accès au paramétrage de la comptabilité`.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-parametrer-comptabilite-avance-entreprise-ingeneo-precompta
* titre : Comment faire le paramétrage avancé de la comptabilité d'une entreprise dans INGENEO PRECOMPTA ?
* titre\_menu : Paramétrage avancé de la comptabilité
* type : procedure
* module : Gestion des entreprises
* version\_outil : 2.11.0 (version observée)
* roles\_concernes : utilisateur avec le droit `Autoriser l'accès au paramétrage de la comptabilité`
* tags : comptabilité, comptes tiers, plan comptable, export comptable, TVA, analytique
* formulations\_utilisateur : « Comment automatiser la création des comptes fournisseurs ? » ; « Compte collectif obligatoire » ; « Pourquoi mes deux lignes de TVA sont fusionnées à l'export ? » ; « Mon écriture à 0 € ne part pas en compta » ; « Comment ajouter des zéros à mes comptes ? » ; « Les tampons n'apparaissent pas sur le PDF exporté »
* sources : Refonte de la page GitBook ingeneo-pre-compta/gestion-des-entreprises/parametrage-comptabilite (découpage) ; observation de l'application INGENEO PRECOMPTA 2.11.0 (2026-10-14) ; réponses de l'expert 2026-10-14
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-14
* statut : brouillon

</details>
