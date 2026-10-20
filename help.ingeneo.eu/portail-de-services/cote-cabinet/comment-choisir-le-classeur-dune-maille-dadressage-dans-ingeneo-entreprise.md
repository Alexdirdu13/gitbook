---
description: >-
  Dans INGENEO ENTREPRISE, Mon espace partenaire : synchroniser les classeurs et
  choisir le classeur où arrivent les documents d'une maille d'adressage.
---

# Comment choisir le classeur d'une maille d'adressage dans INGENEO ENTREPRISE ?

**Résumé :** Cette procédure permet à un cabinet d'expertise comptable de choisir, dans INGENEO ENTREPRISE, le classeur où arrivent les documents reçus par une maille d'adressage d'une entreprise cliente. Elle se fait depuis `Mon espace partenaire` et prend environ 2 minutes. Elle nécessite le droit `Administrer le portail de services` ou `Gérer le portail de services` dans INGENEO PRECOMPTA.

## Objectif

Dans INGENEO ENTREPRISE, une maille d'adressage est le niveau auquel est rattachée l'adresse de réception des factures électroniques d'une entreprise (`0225:Identifiant`) dans l'annuaire du Portail Public de Facturation (PPF). Ce niveau est l'entreprise (SIREN), un établissement (SIRET), un service (Code Routage) ou un canal fonctionnel (SIREN\_SUFFIXE).

Dans INGENEO ENTREPRISE, chaque maille d'adressage dépose ses documents dans un classeur. Sans choix, les documents arrivent dans le premier classeur d'achat, celui qui porte le numéro 1 dans INGENEO PRECOMPTA. Utilisez cette procédure pour choisir un autre classeur.

Le classeur d'une maille d'adressage choisi dans INGENEO ENTREPRISE est indépendant du `Classeur d'achat associé` choisi dans INGENEO PRECOMPTA. Chaque réglage s'applique dans son logiciel, selon que l'utilisateur fait le traitement des validations dans INGENEO ENTREPRISE ou dans INGENEO PRECOMPTA.

## Prérequis

* Avoir accès à `Mon espace partenaire` dans INGENEO ENTREPRISE. Cet accès est réservé aux collaborateurs du cabinet qui ont le droit `Administrer le portail de services` ou `Gérer le portail de services` dans leur profil de droits INGENEO PRECOMPTA.
* Avoir accès à l'entreprise concernée. Cet accès dépend des droits d'accès à l'entreprise dans INGENEO PRECOMPTA.
* Avoir le droit de voir le classeur de destination dans INGENEO ENTREPRISE. Les droits sur les classeurs se règlent dans l'entreprise, engrenage en haut à gauche, menu `Gestion des classeurs`.
* Le classeur de destination existe dans l'entreprise dans INGENEO PRECOMPTA.

## Étapes

### Synchroniser les classeurs de l'entreprise

Dans INGENEO ENTREPRISE, `Synchroniser les classeurs` récupère la liste des classeurs de l'entreprise dans INGENEO PRECOMPTA. Lancez-la avant de choisir le classeur d'une maille d'adressage, et après chaque création de classeur dans INGENEO PRECOMPTA.

1. Dans INGENEO ENTREPRISE, `Mon espace partenaire`, cliquez sur `Liste des clients` dans le menu de gauche.
2. Sur la ligne de l'entreprise concernée, cliquez sur les 3 points tout à droite.
3. Cliquez sur `Synchroniser les classeurs`.
4. Cliquez sur `Valider`.
5. Attendez la fin de la synchronisation, qui dure quelques secondes.

### Choisir le classeur d'une maille d'adressage

1. Dans INGENEO ENTREPRISE, `Mon espace partenaire > Liste des clients`, cliquez sur la ligne de l'entreprise concernée.
2. Dans l'entreprise, cliquez sur l'engrenage en haut à gauche de l'écran.
3. Dans le menu déroulant, cliquez sur `Adressage pour la facture électronique`. L'écran `Adressage pour la facturation électronique` liste les mailles d'adressage de l'entreprise. Les colonnes sont `Statut`, `Identifiant d'adressage`, `Date d'activation`, `Date de fin` et `Classeur`.
4. Repérez la maille d'adressage concernée dans la colonne `Identifiant d'adressage`.
5. Cliquez sur le crayon en bout de ligne, à droite de cette maille d'adressage.
6. Dans le champ `Classeur`, sélectionnez le classeur de destination.
7. Cliquez sur `Mettre à jour`.
8. Si vous paramétrez d'autres mailles d'adressage, refaites les étapes 4 à 7 pour chacune.

## Résultat attendu

* Dans INGENEO ENTREPRISE, le message `Mise à jour effectuée` s'affiche après le clic sur `Mettre à jour`.
* Dans l'écran `Adressage pour la facturation électronique`, la colonne `Classeur` de la maille d'adressage affiche le classeur choisi.
* Les nouveaux documents reçus par cette maille d'adressage arrivent dans le classeur choisi.
* Les documents déjà reçus par cette maille d'adressage restent dans l'ancien classeur.
* Le `Classeur d'achat associé` de la maille d'adressage dans INGENEO PRECOMPTA ne change pas : les deux réglages sont indépendants.

## Erreurs fréquentes

* **Classeur absent de la liste `Classeur`.** Dans INGENEO ENTREPRISE, la liste `Classeur` ne propose que les classeurs déjà synchronisés que l'utilisateur a le droit de voir. Si le classeur vient d'être créé dans INGENEO PRECOMPTA, relancez `Synchroniser les classeurs` depuis les 3 points de la ligne de l'entreprise dans `Liste des clients`. Si le classeur n'apparaît toujours pas, vérifiez les droits dans l'engrenage de l'entreprise, menu `Gestion des classeurs`.
* **Message `Erreur lors de la synchronisation`.** Dans INGENEO ENTREPRISE, ce message s'affiche après `Synchroniser les classeurs` en cas de coupure internet ou si l'entreprise n'existe plus dans INGENEO PRECOMPTA. Contactez le support.
* **Anciens documents toujours dans l'ancien classeur.** Dans INGENEO ENTREPRISE, changer le classeur d'une maille d'adressage ne s'applique qu'aux nouveaux documents. Les documents déjà reçus restent dans l'ancien classeur.
* **Documents arrivés dans un classeur inattendu.** Dans INGENEO ENTREPRISE, une maille d'adressage sans classeur choisi dépose ses documents dans le premier classeur d'achat, celui qui porte le numéro 1 dans INGENEO PRECOMPTA. Choisissez le classeur dans l'écran `Adressage pour la facturation électronique`.
* **Classeur différent dans INGENEO PRECOMPTA.** Le classeur choisi dans INGENEO ENTREPRISE ne modifie pas le `Classeur d'achat associé` d'INGENEO PRECOMPTA. Réglez chaque logiciel séparément, selon celui où l'utilisateur fait le traitement des validations.

## Fiches liées

* [Choisir le classeur d'une maille d'adressage](../../ingeneo-pre-compta/gestion-des-entreprises/choisir-le-classeur-dune-maille-dadressage.md) : le même réglage dans INGENEO PRECOMPTA (`Classeur d'achat associé`), indépendant de celui d'INGENEO ENTREPRISE.
* [Comment mettre une date de fin à une maille d'adressage dans INGENEO ENTREPRISE ?](comment-mettre-une-date-de-fin-a-une-maille-dadressage-dans-ingeneo-entreprise.md) : autre réglage de la même maille d'adressage, depuis le même écran `Adressage pour la facturation électronique`.
* [Comment créer et paramétrer un classeur comptable dans INGENEO PRECOMPTA ?](../../ingeneo-pre-compta/gestion-des-entreprises/classeurs-comptables.md) : création des classeurs récupérés par `Synchroniser les classeurs`.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-choisir-classeur-maille-adressage-ingeneo-entreprise
* titre\_menu : Classeur d'une maille d'adressage
* type : procedure
* module : Portail de services (côté cabinet)
* version\_outil : toutes
* roles\_concernes : collaborateur du cabinet d'expertise comptable avec le droit `Administrer le portail de services` ou `Gérer le portail de services`
* tags : facture électronique, maille d'adressage, classeur, synchronisation des classeurs, Mon espace partenaire
* formulations\_utilisateur : « affecter un classeur à une maille d'adressage » ; « rapprocher une maille d'adressage d'un classeur d'achat » ; « dans quel classeur arrivent les factures de la maille » ; « synchroniser les classeurs »
* sources : transcription 2026-10-20 ; réponses de l'expert 2026-10-20
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-20
* statut : brouillon

</details>
