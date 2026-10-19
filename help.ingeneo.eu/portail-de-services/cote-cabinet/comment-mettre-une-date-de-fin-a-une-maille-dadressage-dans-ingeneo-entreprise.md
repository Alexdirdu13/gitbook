---
description: >-
  Dans INGENEO ENTREPRISE, Mon espace partenaire : mettre une date de fin à une
  maille d'adressage. La DGFIP recommande de ne pas le faire.
---

# Comment mettre une date de fin à une maille d'adressage dans INGENEO ENTREPRISE ?

**Résumé :** Cette procédure permet à un cabinet d'expertise comptable de fixer une date de fin à une maille d'adressage d'une entreprise cliente dans INGENEO ENTREPRISE, depuis `Mon espace partenaire`. Elle prend environ 2 minutes et nécessite le droit `Administrer le portail de services` ou `Gérer le portail de services` dans INGENEO PRECOMPTA. La DGFIP recommande de ne pas mettre de date de fin à une maille d'adressage.

## Objectif

Dans INGENEO ENTREPRISE, une maille d'adressage est le niveau auquel est rattachée l'adresse de réception des factures électroniques d'une entreprise (`0225:Identifiant`) dans l'annuaire du Portail Public de Facturation (PPF). Ce niveau est l'entreprise (SIREN), un établissement (SIRET), un service (Code Routage) ou un canal fonctionnel (SIREN\_SUFFIXE).

Une date de fin sur une maille d'adressage arrête, à cette date, la réception des factures électroniques de l'entreprise par cette maille. Utilisez cette procédure uniquement dans l'un de ces trois cas : cessation d'activité de l'entreprise, décès, arrêt de la mission de l'expert-comptable auprès de l'entreprise.

ATTENTION : la DGFIP recommande de ne jamais mettre de date de fin à une maille d'adressage, même si elle l'autorise. Si l'entreprise souscrit à une nouvelle Plateforme Agréée (PA) après cette date, elle risque de ne plus recevoir ses documents. La bonne pratique est de ne pas mettre de date de fin : la nouvelle PA de l'entreprise écrase alors la maille d'adressage par la portabilité. Selon le texte de la réforme de la facturation électronique, cette reprise est de la responsabilité de la nouvelle PA.

## Prérequis

* Avoir accès à `Mon espace partenaire` dans INGENEO ENTREPRISE. Cet accès est réservé aux collaborateurs du cabinet qui ont le droit `Administrer le portail de services` ou `Gérer le portail de services` dans leur profil de droits INGENEO PRECOMPTA.
* Avoir accès à l'entreprise concernée. Cet accès dépend des droits d'accès à l'entreprise dans INGENEO PRECOMPTA. Aucun autre droit n'est nécessaire pour modifier une maille d'adressage.
* Connaître l'identifiant d'adressage de la maille à arrêter (SIREN, SIRET, Code Routage ou SIREN\_SUFFIXE).
* Choisir une date de fin postérieure à la date du jour. INGENEO ENTREPRISE n'accepte ni une date passée ni la date du jour.
* Vérifier que la situation de l'entreprise est une cessation d'activité, un décès ou un arrêt de la mission de l'expert-comptable. Dans les autres cas, la DGFIP recommande de ne pas mettre de date de fin.

## Étapes

1. Dans INGENEO ENTREPRISE, `Mon espace partenaire`, cliquez sur `Liste des clients` dans le menu de gauche.
2. Cliquez sur la ligne de l'entreprise concernée.
3. Dans l'entreprise, cliquez sur l'engrenage en haut à gauche de l'écran.
4. Dans le menu déroulant, cliquez sur `Adressage pour la facture électronique`. L'écran `Adressage pour la facturation électronique` liste les mailles d'adressage de l'entreprise. Les colonnes sont `Statut`, `Identifiant d'adressage`, `Date d'activation`, `Date de fin` et `Classeur`.
5. Repérez la maille d'adressage concernée dans la colonne `Identifiant d'adressage`.
6. Cliquez sur le crayon en bout de ligne, à droite de cette maille d'adressage.
7. Dans le champ `Date de fin`, saisissez une date postérieure à la date du jour.
8. Cliquez sur `Mettre à jour`.

## Résultat attendu

* Dans INGENEO ENTREPRISE, le message `Mise à jour effectuée` s'affiche après le clic sur `Mettre à jour`.
* Tant que la date de fin n'est pas atteinte, elle reste modifiable dans l'écran `Adressage pour la facturation électronique`. Cliquez sur le crayon de la maille d'adressage, puis remplacez la date ou videz le champ `Date de fin` pour retirer la date de fin. Cliquez ensuite sur `Mettre à jour`.
* Quand la date de fin est atteinte, la colonne `Statut` de la maille d'adressage passe à inactif. L'entreprise ne reçoit plus de factures électroniques par cette maille d'adressage.
* La colonne `Classeur` indique le classeur où étaient déposés les documents reçus par cette maille d'adressage.
* Dans l'annuaire du Portail Public de Facturation (PPF), l'arrêt de la maille d'adressage prend effet à la date de fin saisie dans INGENEO ENTREPRISE.

## Erreurs fréquentes

* **Date passée ou date du jour refusée.** Dans INGENEO ENTREPRISE, le champ `Date de fin` d'une maille d'adressage n'accepte qu'une date future. Saisissez une date postérieure à la date du jour.
* **Date de fin atteinte par erreur.** Une maille d'adressage inactive ne peut pas être réactivée dans INGENEO ENTREPRISE. Avant que la date soit atteinte, ouvrez l'écran `Adressage pour la facturation électronique`, cliquez sur le crayon et videz le champ `Date de fin`, puis cliquez sur `Mettre à jour`.
* **Date de fin mise lors d'un changement de Plateforme Agréée (PA).** Si l'entreprise souscrit à une nouvelle PA après la date de fin, elle risque de ne plus recevoir ses documents. La DGFIP recommande de ne pas mettre de date de fin : la nouvelle PA écrase la maille d'adressage par la portabilité. Si une date de fin a été saisie, videz le champ `Date de fin` avant qu'elle soit atteinte.

## Fiches liées

* [Comment transférer une entreprise de la PA SEPTEO à une autre PA ?](../../enrolement-and-mandats/cote-cabinet/procedure-de-portabilite-cabinet-dexpertise-comptable/comment-transferer-une-entreprise-de-la-pa-septeo-a-une-autre-pa.md) : portabilité de la maille d'adressage vers la nouvelle Plateforme Agréée (PA), la bonne pratique recommandée par la DGFIP à la place d'une date de fin.
* [Qu'implique la cessation d'activité d'une entreprise ?](../../enrolement-and-mandats/cote-cabinet/procedure-de-portabilite-cabinet-dexpertise-comptable/quimplique-la-cessation-dactivite-dune-entreprise.md) : effet de la cessation d'activité sur le rattachement de l'entreprise à la PA SEPTEO.
