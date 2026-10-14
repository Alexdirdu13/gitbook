---
description: >-
  Liste des codes motifs des statuts de la réforme dans INGENEO PRECOMPTA :
  libellés, statuts concernés et règles de masquage.
---

# Codes motifs des statuts de la réforme

**Résumé :** Cette fiche liste les codes motifs des statuts de la réforme dans INGENEO PRECOMPTA. Pour chaque code, le tableau donne son libellé affiché, les statuts qui le proposent et ses règles de masquage.

## Tableau de référence

Dans INGENEO PRECOMPTA, les statuts `Refusée`, `Approuvée partiellement`, `En litige` et `Suspendue` proposent des codes motifs. La colonne « Valeur par défaut » indique si le code est proposé dans la `Configuration par défaut`.

| Nom exact          | Description                                   | Valeurs possibles                                              | Valeur par défaut | Remarques                                                        |
| ------------------ | --------------------------------------------- | -------------------------------------------------------------- | ----------------- | ---------------------------------------------------------------- |
| `AUTRE`            | `Autre`                                       | `Approuvée partiellement`, `En litige`                         | Proposé           | Masquable. Ne demande pas de commentaire obligatoire.            |
| `TX_TVA_ERR`       | `Taux de TVA erroné`                          | `Refusée`, `En litige`                                         | Proposé           | Non masquable pour `Refusée`. Masquable pour `En litige`.        |
| `MONTANTTOTAL_ERR` | `Montant total erroné`                        | `Refusée`, `En litige`                                         | Proposé           | Non masquable pour `Refusée`. Masquable pour `En litige`.        |
| `CALCUL_ERR`       | `Erreur de calcul de la facture`              | `Refusée`, `En litige`                                         | Proposé           | Non masquable pour `Refusée`. Masquable pour `En litige`.        |
| `NON_CONFORME`     | `Mention légale manquante`                    | `Refusée`, `En litige`                                         | Proposé           | Non masquable pour `Refusée`. Masquable pour `En litige`.        |
| `DOUBLON`          | `Facture en doublon`                          | `Refusée`, `En litige`                                         | Proposé           | Non masquable pour `Refusée`. Masquable pour `En litige`.        |
| `DEST_ERR`         | `Erreur de destinataire`                      | `Refusée`, `En litige`                                         | Proposé           | Non masquable pour `Refusée`. Masquable pour `En litige`.        |
| `TRANSAC_INC`      | `Transaction inconnue`                        | `Refusée`, `En litige`                                         | Proposé           | Non masquable pour `Refusée`. Masquable pour `En litige`.        |
| `EMMET_INC`        | `Émetteur inconnu`                            | `Refusée`, `En litige`                                         | Proposé           | Non masquable pour `Refusée`. Masquable pour `En litige`.        |
| `CONTRAT_TERM`     | `Contrat terminé`                             | `Refusée`, `En litige`                                         | Proposé           | Non masquable pour `Refusée`. Masquable pour `En litige`.        |
| `DOUBLE_FACT`      | `Double facture`                              | `Refusée`, `En litige`                                         | Proposé           | Non masquable pour `Refusée`. Masquable pour `En litige`.        |
| `CMD_ERR`          | `N° de COMMANDE incorrect ou manquant`        | `Refusée`, `Approuvée partiellement`, `En litige`, `Suspendue` | Proposé           | Non masquable pour `Refusée`. Masquable pour les autres statuts. |
| `ADR_ERR`          | `Adresse de facturation électronique erronée` | `Refusée`, `En litige`                                         | Proposé           | Non masquable pour `Refusée`. Masquable pour `En litige`.        |
| `REF_CT_ABSENT`    | `Référence contractuelle manquante`           | `Refusée`, `Approuvée partiellement`, `En litige`, `Suspendue` | Proposé           | Non masquable pour `Refusée`. Masquable pour les autres statuts. |
| `SIRET_ERR`        | `SIRET erroné ou absent`                      | `Approuvée partiellement`, `En litige`, `Suspendue`            | Proposé           | Masquable.                                                       |
| `CODE_ROUTAGE_ERR` | `CODE_ROUTAGE absent ou erroné`               | `Approuvée partiellement`, `En litige`, `Suspendue`            | Proposé           | Masquable.                                                       |
| `REF_ERR`          | `Référence incorrecte`                        | `Approuvée partiellement`, `En litige`, `Suspendue`            | Proposé           | Masquable.                                                       |
| `PU_ERR`           | `Prix unitaires incorrects`                   | `Approuvée partiellement`, `En litige`                         | Proposé           | Masquable.                                                       |
| `REM_ERR`          | `Remise erronée`                              | `Approuvée partiellement`, `En litige`                         | Proposé           | Masquable.                                                       |
| `QTE_ERR`          | `Quantité facturée incorrecte`                | `Approuvée partiellement`, `En litige`                         | Proposé           | Masquable.                                                       |
| `ART_ERR`          | `Article facturé incorrect`                   | `Approuvée partiellement`, `En litige`                         | Proposé           | Masquable.                                                       |
| `MODPAI_ERR`       | `Modalités de paiement incorrectes`           | `Approuvée partiellement`, `En litige`                         | Proposé           | Masquable.                                                       |
| `QUALITE_ERR`      | `Qualité d'article livré incorrecte`          | `Approuvée partiellement`, `En litige`                         | Proposé           | Masquable.                                                       |
| `LIVR_INCOMP`      | `Problème de livraison`                       | `Approuvée partiellement`, `En litige`                         | Proposé           | Masquable.                                                       |
| `COORD_BANC_ERR`   | `Erreur de coordonnées bancaires`             | `En litige`, `Suspendue`                                       | Proposé           | Masquable.                                                       |
| `JUSTIF_ABS`       | `Justificatif absent ou insuffisant`          | `Suspendue`                                                    | Proposé           | Masquable.                                                       |

## Notes

* **Nombre de codes par statut :** dans INGENEO PRECOMPTA, `Refusée` propose 13 codes motifs, `Approuvée partiellement` 13, `En litige` 25 et `Suspendue` 7.
* **Statuts sans code motif :** dans INGENEO PRECOMPTA, les statuts `Prise en charge`, `Approuvée` et `Paiement transmis` n'ont pas de code motif, comme le prévoit la réforme de la facturation électronique.
* **Origine des codes :** dans INGENEO PRECOMPTA, les codes motifs et leurs libellés viennent directement de la liste définie par la DGFiP pour la réforme de la facturation électronique.
* **Choix obligatoire :** dans INGENEO PRECOMPTA, le choix d'un code motif est obligatoire pour appliquer `Refusée`, `Approuvée partiellement`, `En litige` ou `Suspendue`. La fenêtre du statut affiche uniquement les libellés, pas les codes.
* **Commentaire de refus :** dans INGENEO PRECOMPTA, un commentaire facultatif peut accompagner le statut `Refusée`. Il est transmis au fournisseur avec le code motif.
* **Transmission au fournisseur :** dans INGENEO PRECOMPTA, les statuts `Refusée`, `Approuvée`, `Approuvée partiellement`, `En litige`, `Suspendue` et `Paiement transmis` sont transmis au fournisseur. Le statut `Prise en charge` n'est pas transmis.
* **Statut terminal :** dans INGENEO PRECOMPTA, seul le statut `Refusée` est terminal. Une facture refusée ne peut plus être émise de nouveau.
* **Masquage :** dans la `Configuration personnalisée pour cette entreprise`, les codes motifs de `Approuvée partiellement`, `En litige` et `Suspendue` peuvent être masqués. Les codes motifs de `Refusée` ne peuvent pas être modifiés. Tous les codes sont proposés dans la `Configuration par défaut`.

## Fiches liées

* [Comment configurer les statuts de la réforme ?](comment-configurer-les-statuts-de-la-reforme.md) : masquage des codes motifs dans la configuration personnalisée
* [Comment prendre en charge ou refuser une facture électronique dans INGENEO PRECOMPTA ?](../gestion-des-documents/comment-prendre-en-charge-ou-refuser-une-facture-electronique-dans-ingeneo-precompta.md) : choix du motif de refus
* [Comment donner les droits sur les statuts de facture ?](../administration/comment-donner-les-droits-sur-les-statuts-de-facture.md) : droits nécessaires pour appliquer chaque statut
