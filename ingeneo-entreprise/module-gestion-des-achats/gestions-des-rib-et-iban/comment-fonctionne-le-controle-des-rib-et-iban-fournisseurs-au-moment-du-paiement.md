# Comment fonctionne le contrôle des RIB et IBAN fournisseurs au moment du paiement ?

## Contrôle des IBAN au paiement de votre facture fournisseur

Au moment de la génération du paiement, en XML SEPA ou via le compte Pro Qotid, vous pourrez créer ou valider les RIB fournisseurs.

Plusieurs cas peuvent se présenter :

* Cas 1 : il n'y a qu'un seul RIB sur la fiche fournisseur
* Cas 2 : il y a plusieurs RIB sur la fiche fournisseur
* Cas 3 : il y a des RIB différents entre ceux de la fiche fournisseur et celui présent sur la facture fournisseur

**Chemin : Cas 1**

## Un seul RIB sur la fiche fournisseur et aucun conflit

S'il existe un seul RIB sur la fiche fournisseur et qu'il n'existe aucun conflit avec le RIB présent sur la facture, **le RIB sera sélectionné automatiquement au moment de la validation du paiement**.

**Chemin : Cas 2**

## Plusieurs RIB sur la fiche fournisseur

S'il y a plusieurs RIB sur la fiche fournisseur, Qotid ne choisira pas de RIB par défaut et vous demandera de sélectionner le bon RIB.

En cliquant sur la petite flèche en face du fournisseur, vous verrez les deux RIB présents sur la fiche fournisseur.

Vous devrez sélectionner le bon RIB à ce moment-là.

**Chemin : Cas 3**

## RIB différents entre ceux de la fiche fournisseur et celui de la facture fournisseur

En cas de conflit entre le ou les RIB présents sur la fiche fournisseur et le RIB présent sur la facture fournisseur, Qotid vous demandera de choisir le bon RIB.

**Attention :**

Si vous choisissez de prendre le RIB présent sur la facture, il ne sera pas automatiquement créé sur la fiche fournisseur. Vous devez le créer.

## Créer le RIB au moment du paiement

Pour créer le RIB au moment du paiement, cliquez sur le **+** en face du fournisseur sur lequel vous souhaitez ajouter un RIB.

## Valider la création du RIB

Une pop-up s'affichera et vous pourrez saisir :

* Un **libellé**. C'est pour vous y retrouver si le fournisseur a plusieurs RIB. En général, vous pouvez indiquer le nom de la banque, par exemple BNP Paribas.
* L'IBAN
* Le code **SWIFT / BIC**

**À savoir :**

Dans le cas où un RIB est présent sur la facture, vous pourrez directement récupérer l'IBAN présent sur la facture.

**Attention :**

Au moment de la validation du RIB, Qotid effectue un contrôle pour s'assurer que l'IBAN est correct. S'il est faux ou mal renseigné, vous ne pourrez pas valider la création de votre IBAN.

Votre RIB sera maintenant disponible dans la fiche fournisseur.
