---
description: >-
  Cette procédure permet de créer un devis dans INGENEO ENTREPRISE, menu `Ventes
  > Devis`, puis de l'envoyer, de changer son statut ou de le convertir en
  facture. Elle prend environ 1 minute et nécessit
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
  - portail-de-service
---

# Comment créer un devis dans INGENEO ENTREPRISE ?

## Objectif

Dans INGENEO ENTREPRISE, cette procédure permet de créer un devis pour un client à partir des produits du menu `Ventes > Produits`. Le devis enregistré reçoit un numéro au format `D000001` et le statut `BROUILLON`. La procédure couvre aussi l'envoi du devis, le changement manuel de son statut et sa conversion avec `Convertir en`.

## Prérequis

Pour créer un devis dans INGENEO ENTREPRISE, vérifiez les points suivants :

* L'établissement dispose au minimum de l'offre `PACK PRO`.
* L'utilisateur dispose du droit `Créer des devis`, dans la catégorie `Module de vente`.
* Le client existe, ou vous pouvez le créer pendant la saisie du devis.
* Le produit existe dans `Ventes > Produits`, ou vous pouvez le créer pendant la saisie du devis.
* Pour envoyer le devis au client, un contact est rattaché au client et une adresse email est rattachée à ce contact.
* Pour qu'un compte bancaire soit proposé dans le champ `Compte *` du devis, les coordonnées bancaires sont renseignées dans la fiche client. Sans coordonnées bancaires, l'enregistrement du devis n'est pas bloqué.
* La numérotation des devis se paramètre dans `Ventes > Paramètres`.

## Étapes

1. Dans INGENEO ENTREPRISE, sélectionnez l'établissement concerné dans la liste des établissements en haut de l'écran.
2. Ouvrez `Ventes > Devis`.
3. Cliquez sur `Créer un devis`. La fenêtre `Nouveau devis` s'ouvre.
4. Si le client n'existe pas encore, ouvrez la liste `Client *` et cliquez sur `Créer`.
5. Dans la liste `Client *`, sélectionnez le client. Les champs `Adresse de facturation` et `Adresse de livraison` apparaissent.
6. Si nécessaire, sélectionnez une adresse dans `Adresse de facturation` et dans `Adresse de livraison`.
7. Si vous prévoyez d'envoyer le devis par INGENEO ENTREPRISE, sélectionnez dans le champ `Contact` un contact qui possède une adresse email.
8. Dans `Modes de paiement *`, conservez `Virement` ou sélectionnez un autre mode de paiement.
9. Si nécessaire, renseignez les champs facultatifs `N° de bon de commande` et `Ref. client`.
10. Vérifiez le champ `Date d'émission`. Par défaut, il contient la date du jour.
11. Dans `Délai de signature`, conservez `30 jours` ou sélectionnez un autre délai. Le champ `À signer avant le` se calcule automatiquement et n'est pas modifiable.
12. Dans le champ `Objet`, saisissez l'objet du devis.
13. Si nécessaire, insérez une balise dans l'objet, par exemple `Numéro du jour courant`. Cliquez sur `Voir tous` pour afficher les autres balises, comme `Nom du mois courant` ou `Année courante`.
14. Dans le bloc `Liste des articles`, cliquez sur `Ajouter des articles`. La fenêtre `Ajouter un ou plusieurs produits` s'ouvre.
15. Si le produit n'existe pas encore, cliquez sur `Créer un produit`.
16. Dans le champ de recherche `Nom, Référence, Description...`, saisissez le nom ou la référence du produit.
17. Cliquez sur le bouton `+` à droite de chaque produit à ajouter. Le produit apparaît dans `Articles sélectionnés`.
18. Cliquez sur `Ajouter les produit(s)`. Les produits apparaissent dans le bloc `Liste des articles`.
19. Si nécessaire, modifiez sur chaque ligne les colonnes `Quantité`, `Prix HT`, `Remise` et le taux de TVA (`20%` par défaut pour le produit testé).
20. Si nécessaire, regroupez les produits en sections avec `Ajouter une section` et le champ `Saisir un titre de section`.
21. Si nécessaire, dans le bloc `Récapitulatif`, cliquez sur `Ajouter une remise globale`.
22. Si nécessaire, dans le bloc `Acompte`, cliquez sur `Demander un acompte`.
23. Dans le bloc `Details du paiement`, champ `Compte *`, sélectionnez le compte bancaire. Les champs `Nom du compte`, `IBAN` et `BIC/SWIFT` s'affichent.
24. Si nécessaire, cliquez sur `Ajouter un échéancier de paiement`.
25. Si nécessaire, dans le bloc `Pied de page`, renseignez `Mention spéciale`, `Conditions générales de ventes`, `Note de pied de page` et `Annexe`.
26. Si nécessaire, cliquez sur `Paramètre d'affichage`, puis activez ou désactivez les interrupteurs des éléments à afficher sur le devis. Les interrupteurs sont regroupés sous trois titres sans interrupteur :
    * Titre `Design du document` : `Afficher le logo`, `Afficher la référence produit`, `Afficher les sous-totaux par sections`, `Afficher le type d'unité`.
    * Titre `Afficher mes informations` : `Afficher l'adresse`, `Afficher l'email`, `Afficher le numéro de téléphone`, `Afficher le numéro de téléphone portable`, `Afficher uniquement le SIRET`, `Afficher le SIREN et le SIRET`.
    * Titre `Afficher les informations du client` : `Afficher le SIRET`, `Afficher le SIREN`, `Afficher le numéro de TVA intracommunautaire`, `Afficher le nom du contact`, `Afficher l'email`, `Afficher l'adresse`, `Afficher le numéro de téléphone`, `Afficher le numéro de téléphone portable`.
27. Cliquez sur `Enregistrer`. Pour afficher en plus un aperçu du devis, cliquez plutôt sur `Enregistrer et prévisualiser`. Dans les deux cas, le devis reste au statut `BROUILLON`.
28. Pour envoyer, changer le statut ou convertir le devis, ouvrez `Ventes > Devis` et cliquez sur la ligne du devis. Le panneau du devis s'ouvre, avec un aperçu du document.
29. Si un contact avec une adresse email est rattaché au devis, cliquez sur `Envoyer le devis` pour l'envoyer au client. Le devis passe automatiquement au statut `ENVOYÉ`.
30. Si le devis n'a pas été envoyé lors de sa création et que vous l'envoyez plus tard, cliquez sur le bouton `...` du panneau du devis, puis sur `Envoyer par email`.
31. Si vous avez envoyé le devis au client par un autre moyen qu'INGENEO ENTREPRISE, cliquez sur le bouton `...` du panneau du devis, puis sur `Marquer comme envoyé`.
32. Pour enregistrer la réponse du client ou annuler le devis, cliquez sur le bouton `...` du panneau du devis, puis sur `Marquer comme accepté`, `Marquer comme refusé` ou `Annuler le devis`. Le même menu propose aussi `Dupliquer le devis` et `Transformer en abonnement`.
33. Pour convertir le devis, cliquez sur `Convertir en` dans le panneau du devis, puis sur `Facture`, `Facture d'acompte`, `Facture intermédiaire` ou `Facture de solde`.

## Résultat attendu

Dans INGENEO ENTREPRISE, après un clic sur `Enregistrer` dans la fenêtre `Nouveau devis`, le message `Succès` s'affiche. La fenêtre prend le titre `Devis` suivi du numéro attribué, au format `D000001`.

Dans `Ventes > Devis`, le devis apparaît dans la liste avec le statut `BROUILLON`. La liste affiche les colonnes `Statut`, `Date d'émission`, `Client`, `N° de devis`, `TTC`, `HT`, `TVA` et `Date échéance`. La `Date échéance` correspond à la date du champ `À signer avant le`.

Les compteurs en haut de l'écran `Ventes > Devis` affichent le nombre et le montant TTC des devis par statut : `BROUILLON`, `ENVOYÉ`, `ACCEPTÉ`, `REFUSÉ`, `RESTANT À FACTURER`, `FACTURÉ`, `ANNULÉ` et `TOUS`. Le statut `ENVOYÉ` s'applique automatiquement après un envoi par `Envoyer le devis`, ou manuellement avec `Marquer comme envoyé`. Les statuts `ACCEPTÉ`, `REFUSÉ` et `ANNULÉ` se changent manuellement depuis le bouton `...` du panneau du devis. Un devis validé mais pas encore transformé en facture a le statut `RESTANT À FACTURER`. Un devis validé puis transformé en facture avec `Convertir en` a le statut `FACTURÉ`.

## Erreurs fréquentes

* **Situation :** dans la fenêtre `Nouveau devis` d'INGENEO ENTREPRISE, les boutons `Enregistrer` et `Enregistrer et prévisualiser` sont grisés. **Cause :** le champ `Client *` est vide ou le bloc `Liste des articles` ne contient aucun produit. **Solution :** sélectionnez un client dans `Client *`, puis ajoutez au moins un produit avec `Ajouter des articles`.
* **Situation :** dans la fenêtre `Nouveau devis` d'INGENEO ENTREPRISE, le champ `Compte *` ne propose aucun compte bancaire. **Cause :** les coordonnées bancaires ne sont pas renseignées dans la fiche client. **Solution :** l'enregistrement du devis reste possible malgré l'astérisque. Pour proposer un compte, renseignez les coordonnées bancaires dans la fiche client.
* **Situation :** dans INGENEO ENTREPRISE, l'utilisateur ne voit pas la fonction de création de devis. **Cause :** l'établissement n'a pas l'offre `PACK PRO` minimum, ou l'utilisateur n'a pas le droit `Créer des devis` de la catégorie `Module de vente`. Sans ce droit, la fonction n'apparaît pas à l'écran. **Solution :** si l'offre est en cause, mettez à jour l'offre commerciale de l'établissement vers `PACK PRO` minimum. Si le droit est en cause, demandez l'attribution du droit `Créer des devis`.

## Fiches liées

* Comment mettre à jour l'offre commerciale dans INGENEO ENTREPRISE ? (fiche à créer) : passage à l'offre `PACK PRO` minimum
* Comment attribuer le droit `Créer des devis` à un utilisateur dans INGENEO ENTREPRISE ? (fiche à créer) : attribution des droits de la catégorie `Module de vente`
* Comment paramétrer la numérotation des devis dans INGENEO ENTREPRISE ? (fiche à créer) : réglages des devis dans `Ventes > Paramètres`
* Comment renseigner les coordonnées bancaires dans la fiche client dans INGENEO ENTREPRISE ? (fiche à créer) : alimente le champ `Compte *` du devis

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-creer-devis-ingeneo-entreprise
* titre\_menu : Créer un devis
* type : procedure
* module : Ventes
* version\_outil :
* roles\_concernes : utilisateur disposant du droit `Créer des devis`
* tags : devis, ventes, brouillon, produits, client
* formulations\_utilisateur :
* sources : observation de l'interface 2026-10-13 (dossier de test) ; réponses de l'expert 2026-10-13 ; remplace la page GitBook portail-de-services/cote-entreprise/module-ventes/creer-un-devis
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-13
* statut : brouillon

</details>
