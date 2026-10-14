---
description: >-
  Appliquer le statut Prise en charge ou Refusée à une facture électronique
  reçue dans INGENEO PRECOMPTA utilisé par une entreprise.
---

# Comment prendre en charge ou refuser une facture électronique dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet d'appliquer le statut `Prise en charge` ou `Refusée` à une facture électronique reçue dans INGENEO PRECOMPTA. **Le statut `Prise en charge` déverrouille la présaisie comptable de la facture.** La procédure prend quelques secondes par facture. Elle nécessite le droit `Autoriser l'application du statut « Refusée »` dans l'onglet `Droits sur les classeurs`.

## Objectif

Dans INGENEO PRECOMPTA utilisé par une entreprise, cette procédure permet de traiter une facture électronique reçue d'un fournisseur.

**Le statut `Prise en charge` déverrouille la présaisie comptable de la facture dans l'encart de saisie.** Ce statut n'est pas transmis au fournisseur : seule l'absence de refus lui est transmise.

Le statut `Refusée` renvoie la facture au fournisseur, sans présaisie comptable, de façon définitive. Cette procédure ne concerne pas INGENEO PRECOMPTA utilisé par un cabinet d'expertise comptable.

## Prérequis

* Dans INGENEO PRECOMPTA, l'entreprise est enrôlée sur la PA SEPTEO.
* Le profil de l'utilisateur inclut le droit `Autoriser l'application du statut « Refusée »` pour le classeur d'achats concerné, dans l'onglet `Droits sur les classeurs`. Ce droit active les boutons `Prise en charge` et `Refusée`.
* Ce droit se règle sur le profil de site ou sur le profil d'entreprise. Si l'utilisateur a les deux, le profil d'entreprise prévaut.
* Le document est une facture électronique. Dans le menu `Bannettes`, une facture électronique porte un X sur l'icône de document, à gauche de son titre.

## Étapes

1. Dans INGENEO PRECOMPTA, cliquez sur le menu `Bannettes` dans le menu de gauche.
2. Ouvrez un dossier enrôlé sur la PA SEPTEO.
3. Repérez la facture électronique : un X figure sur l'icône de document, à gauche du titre.
4. Cliquez sur la loupe de la facture pour l'ouvrir.
5. Repérez l'encart de saisie, en bas à gauche de la vue. Il contient le tableau de présaisie comptable.
6. Si vous traitez la facture, cliquez sur `Prise en charge` dans l'encart de saisie. **La présaisie comptable de la facture est alors déverrouillée.**
7. Si vous refusez la facture, cliquez sur `Refusée` dans l'encart de saisie. Une fenêtre de refus s'ouvre.
8. Dans la fenêtre de refus, sélectionnez le libellé du motif de refus.
9. Si vous souhaitez préciser le refus, saisissez un commentaire dans la fenêtre de refus. Le commentaire est transmis au fournisseur.
10. Cliquez sur `Refuser une facture`.

Dans INGENEO PRECOMPTA, la fenêtre de refus affiche uniquement les libellés des motifs. Ces motifs sont proposés pour le statut `Refusée` :

| Libellé affiché                               | Code associé       |
| --------------------------------------------- | ------------------ |
| `Taux de TVA erroné`                          | `TX_TVA_ERR`       |
| `Montant total erroné`                        | `MONTANTTOTAL_ERR` |
| `Erreur de calcul de la facture`              | `CALCUL_ERR`       |
| `Mention légale manquante`                    | `NON_CONFORME`     |
| `Facture en doublon`                          | `DOUBLON`          |
| `Erreur de destinataire`                      | `DEST_ERR`         |
| `Transaction inconnue`                        | `TRANSAC_INC`      |
| `Émetteur inconnu`                            | `EMMET_INC`        |
| `Contrat terminé`                             | `CONTRAT_TERM`     |
| `Double facture`                              | `DOUBLE_FACT`      |
| `N° de COMMANDE incorrect ou manquant`        | `CMD_ERR`          |
| `Adresse de facturation électronique erronée` | `ADR_ERR`          |
| `Référence contractuelle manquante`           | `REF_CT_ABSENT`    |

Ces codes motifs ne peuvent pas être modifiés, quelle que soit la configuration de l'entreprise.

## Résultat attendu

Dans INGENEO PRECOMPTA, après un clic sur `Prise en charge`, la facture électronique porte le statut `Prise en charge`. **La présaisie comptable de la facture est déverrouillée dans l'encart de saisie.** Ce statut n'est pas transmis au fournisseur, et le menu `Bannettes` ne l'affiche pas.

Après un clic sur `Refuser une facture`, la facture est renvoyée au fournisseur avec le motif et le commentaire éventuel. Le statut `Refusée` est terminal : la facture ne peut plus être émise de nouveau. Aucune présaisie comptable n'est à faire sur cette facture.

## Erreurs fréquentes

* **Message `Un statut cycle de vie FE doit être défini avant de pouvoir enregistrer le document.` :** dans INGENEO PRECOMPTA, ce message s'affiche à l'enregistrement du document. Il indique que la facture électronique n'a pas le statut `Prise en charge`. Cliquez sur `Prise en charge` dans l'encart de saisie de la facture.
* **Facture refusée par erreur :** dans INGENEO PRECOMPTA, le statut `Refusée` est terminal et ne peut pas être annulé. Le fournisseur doit émettre une nouvelle facture avec un nouveau numéro de facture.
* **Bouton `Prise en charge` ou `Refusée` absent :** dans INGENEO PRECOMPTA, ces deux boutons dépendent du droit `Autoriser l'application du statut « Refusée »`. Si l'un d'eux ne s'affiche pas dans l'encart de saisie, l'utilisateur n'a pas ce droit. Le profil d'entreprise prévaut sur le profil de site.
* **Refus après prise en charge :** dans la version actuelle d'INGENEO PRECOMPTA, le statut `Refusée` ne peut pas être appliqué à une facture déjà au statut `Prise en charge`. Cette possibilité est en cours de développement.

## Fiches liées

* [Comment donner les droits sur les statuts de facture ?](../administration/comment-donner-les-droits-sur-les-statuts-de-facture.md) : activation du droit `Autoriser l'application du statut « Refusée »`
* [Comment configurer les statuts de la réforme ?](../gestion-des-entreprises/comment-configurer-les-statuts-de-la-reforme.md) : statuts et codes motifs proposés pour une entreprise
* [Référence : codes motifs des statuts de la réforme](../gestion-des-entreprises/codes-motifs-des-statuts-de-la-reforme.md) : codes motifs de tous les statuts de la réforme
* [Gérer les profils de droits](../administration/gerer-les-profils-de-droits.md) : réglage des droits sur les profils de site et d'entreprise
* [La saisie comptable](la-saisie-comptable.md) : présaisie comptable d'un document
