---
description: >-
  Autoriser les utilisateurs d'un profil de site ou d'entreprise à appliquer les
  statuts de la réforme aux factures électroniques dans INGENEO PRECOMPTA.
---

# Comment donner les droits sur les statuts de facture ?

**Résumé :** Cette procédure permet d'autoriser les utilisateurs d'un profil à appliquer des statuts de la réforme aux factures électroniques dans INGENEO PRECOMPTA. Elle prend environ 1 minute. Elle nécessite l'accès à `Paramètres` ou le droit `Autoriser l'accès au paramétrage de l'entreprise.`.

## Objectif

Dans INGENEO PRECOMPTA, un utilisateur ne peut appliquer un statut de la réforme que si son profil l'y autorise. Un statut non autorisé n'est pas affiché dans l'encart de saisie de la facture électronique.

**L'interrupteur `Autoriser l'application du statut « Refusée »` active à la fois le bouton `Prise en charge` et le bouton `Refusée`.** Sans ce droit, l'utilisateur ne peut pas prendre en charge une facture électronique ni en faire la présaisie comptable.

Ces droits se règlent par des interrupteurs, dans l'onglet `Droits sur les classeurs` d'un profil de site ou d'un profil d'entreprise, pour le classeur `Factures d'achats` :

* `Autoriser l'application du statut « Refusée »`
* `Autoriser l'application du statut « Approuvée »`
* `Autoriser l'application du statut « Approuvée partiellement »`
* `Autoriser l'application du statut « En litige »`
* `Autoriser l'application du statut « Suspendue »`
* `Autoriser l'application du statut « Paiement transmis »`

## Prérequis

* Pour modifier un profil de site dans INGENEO PRECOMPTA, vous devez être administrateur : le menu `Paramètres` leur est réservé.
* Pour modifier un profil d'entreprise dans INGENEO PRECOMPTA, votre profil de site doit inclure le droit `Autoriser l'accès au paramétrage de l'entreprise.`.
* L'utilisateur concerné doit avoir le droit sur le classeur qui reçoit les factures électroniques. Sans droit sur le classeur, il ne peut pas traiter le statut d'un document.
* Un profil de site règle les droits par type de classeur. Un profil d'entreprise règle les droits sur les classeurs spécifiques de l'entreprise.
* Si l'utilisateur a un profil de site et un profil d'entreprise, le profil d'entreprise prévaut.

## Étapes

### Si vous modifiez un profil de site

1. Dans INGENEO PRECOMPTA, cliquez sur `Paramètres`, en bas du menu de gauche.
2. Cliquez sur l'onglet `Profils de droits`.
3. Cliquez sur `Profils de site`.
4. Cliquez sur le bouton crayon du profil de site à modifier.
5. Cliquez sur l'onglet `Droits sur les classeurs`.
6. Repérez le type de classeur `Factures d'achats`.
7. En bas de ce type de classeur, activez l'interrupteur `Autoriser l'application du statut « Refusée »`. Ce droit active les boutons `Prise en charge` et `Refusée`.
8. Si l'utilisateur doit appliquer d'autres statuts, activez les interrupteurs correspondants.
9. Cliquez sur `Enregistrer`.

### Si vous modifiez un profil d'entreprise

1. Dans INGENEO PRECOMPTA, cliquez sur le menu `Entreprise` dans le menu de gauche.
2. Cliquez sur le bouton crayon de l'entreprise concernée.
3. Cliquez sur l'onglet `Administration`.
4. Cliquez sur le menu `Profils d'entreprise`.
5. Cliquez sur le bouton crayon du profil d'entreprise à modifier.
6. Cliquez sur l'onglet `Droits sur les classeurs`.
7. Repérez le classeur d'achats de l'entreprise qui reçoit les factures électroniques.
8. En bas de ce classeur, activez l'interrupteur `Autoriser l'application du statut « Refusée »`. Ce droit active les boutons `Prise en charge` et `Refusée`.
9. Si l'utilisateur doit appliquer d'autres statuts, activez les interrupteurs correspondants.
10. Cliquez sur `Enregistrer`.

## Résultat attendu

Dans INGENEO PRECOMPTA, la modification d'un profil de site ou d'un profil d'entreprise s'applique immédiatement après le clic sur `Enregistrer`. L'utilisateur n'a pas besoin de se reconnecter.

Dans le classeur d'achats concerné, l'encart de saisie d'une facture électronique affiche alors les boutons des statuts autorisés.

## Erreurs fréquentes

* **Bouton `Prise en charge` absent ou présaisie comptable bloquée :** dans INGENEO PRECOMPTA, le bouton `Prise en charge` dépend de l'interrupteur `Autoriser l'application du statut « Refusée »`. Activez cet interrupteur dans `Droits sur les classeurs`, pour le classeur d'achats concerné.
* **Bouton de statut absent malgré un profil de site correct :** dans INGENEO PRECOMPTA, le profil d'entreprise prévaut sur le profil de site. Si le profil d'entreprise n'autorise pas un statut, son bouton n'est pas affiché, même si le profil de site l'autorise. Activez l'interrupteur dans le profil d'entreprise.
* **Bouton de statut absent malgré le droit de statut :** dans INGENEO PRECOMPTA, l'utilisateur doit aussi avoir le droit sur le classeur qui reçoit les factures électroniques. Vérifiez les droits du profil sur ce classeur.
* **Droits de statut absents dans un classeur :** dans INGENEO PRECOMPTA, les droits de statut figurent uniquement dans les classeurs `Factures d'achats`. Ils n'apparaissent pas dans `Factures de ventes`, `Caisse` ni `Banque`.
* **Menu `Profils d'entreprise` inaccessible :** dans INGENEO PRECOMPTA, l'accès au paramétrage d'une entreprise requiert le droit `Autoriser l'accès au paramétrage de l'entreprise.` dans le profil de site.

## Fiches liées

* [Comment prendre en charge ou refuser une facture électronique dans INGENEO PRECOMPTA ?](../gestion-des-documents/comment-prendre-en-charge-ou-refuser-une-facture-electronique-dans-ingeneo-precompta.md) : utilisation des boutons de statut dans l'encart de saisie
* [Gérer les profils de droits](gerer-les-profils-de-droits.md) : création et modification générale des profils
