---
description: >-
  Choisir les statuts de la réforme et les codes motifs proposés pour une
  entreprise dans INGENEO PRECOMPTA.
---

# Comment configurer les statuts de la réforme ?

**Résumé :** Cette procédure permet de choisir les statuts de la réforme et les codes motifs proposés pour une entreprise dans INGENEO PRECOMPTA. Elle prend environ 3 minutes. Elle nécessite le droit `Autoriser l'accès au paramétrage de l'entreprise.` dans le profil de site.

## Objectif

Dans INGENEO PRECOMPTA, chaque entreprise a l'une de ces deux configurations des statuts de la réforme :

* `Configuration par défaut` : tous les statuts et tous les codes motifs sont proposés.
* `Configuration personnalisée pour cette entreprise` : certains statuts sont désactivés et certains codes motifs sont masqués.

La `Configuration par défaut` permet de traiter les factures électroniques sans autre paramétrage. Utilisez cette procédure uniquement pour retirer des statuts ou masquer des codes motifs.

Un statut désactivé n'est plus affiché dans l'encart de saisie, pour tous les utilisateurs de l'entreprise, même si leur profil l'autorise. Les statuts `Prise en charge` et `Refusée` ne peuvent pas être désactivés. Les codes motifs du statut `Refusée` ne peuvent pas être modifiés.

## Prérequis

* Dans INGENEO PRECOMPTA, votre profil de site inclut le droit `Autoriser l'accès au paramétrage de l'entreprise.`.
* L'entreprise est enrôlée sur la PA SEPTEO. Sinon, l'onglet `Facturation électronique` de l'entreprise affiche `Pas d'enrôlement effectif`.
* Si l'entreprise est en `Configuration personnalisée pour cette entreprise`, notez ses réglages avant de repasser en `Configuration par défaut`. Ce changement supprime tous les réglages personnalisés.

## Étapes

1. Dans INGENEO PRECOMPTA, cliquez sur le menu `Entreprise` dans le menu de gauche.
2. Cliquez sur le bouton crayon de l'entreprise concernée.
3. Cliquez sur l'onglet `Facturation électronique`.
4. Cliquez sur l'onglet `Statuts de la réforme`.
5. Sélectionnez `Configuration personnalisée pour cette entreprise`.
6. Pour chaque statut à retirer, désactivez l'interrupteur de la ligne du statut.
7. Si vous souhaitez masquer des codes motifs d'un statut autre que `Refusée`, cliquez sur `Sélectionner les codes motifs`, au bout de la ligne du statut. Un panneau latéral s'ouvre avec la liste des codes motifs, tous cochés par défaut.
8. Dans le panneau latéral, décochez chaque code motif à masquer.
9. Dans le panneau latéral, cliquez sur `Enregistrer`.
10. Dans l'onglet `Statuts de la réforme`, cliquez sur `Enregistrer`.

Pour revenir à la configuration standard, sélectionnez `Configuration par défaut` dans l'onglet `Statuts de la réforme`, puis cliquez sur `Enregistrer`. Tous les statuts et tous les codes motifs sont alors réactivés.

## Résultat attendu

Dans INGENEO PRECOMPTA, la configuration s'applique immédiatement après le clic sur `Enregistrer`. Dans l'encart de saisie des factures électroniques de l'entreprise, les statuts désactivés ne sont plus affichés.

Les codes motifs masqués ne sont plus proposés quand un utilisateur applique le statut concerné. Les factures qui portent déjà un statut désactivé ne sont pas modifiées.

## Erreurs fréquentes

* **Message `Pas d'enrôlement effectif` :** dans INGENEO PRECOMPTA, ce message s'affiche dans l'onglet `Facturation électronique` quand l'entreprise n'est pas enrôlée sur la PA SEPTEO. Les statuts de la réforme ne sont pas configurables tant que l'entreprise n'est pas enrôlée.
* **Bouton de statut disparu pour tous les utilisateurs :** dans INGENEO PRECOMPTA, le statut est désactivé dans la `Configuration personnalisée pour cette entreprise`. Réactivez l'interrupteur du statut dans l'onglet `Statuts de la réforme`, puis cliquez sur `Enregistrer`.
* **Réglages personnalisés perdus :** dans INGENEO PRECOMPTA, repasser en `Configuration par défaut` supprime tous les réglages personnalisés. Pour les retrouver, refaites la configuration personnalisée.
* **Interrupteur de `Prise en charge` ou `Refusée` absent :** dans INGENEO PRECOMPTA, les statuts `Prise en charge` et `Refusée` ne peuvent pas être retirés. Ce comportement est normal.
* **Codes motifs de `Refusée` non modifiables :** dans INGENEO PRECOMPTA, les codes motifs du statut `Refusée` ne peuvent pas être masqués. Ce comportement est normal.
* **Onglet `Statuts de la réforme` inaccessible :** dans INGENEO PRECOMPTA, le paramétrage d'une entreprise requiert le droit `Autoriser l'accès au paramétrage de l'entreprise.` dans le profil de site.

## Fiches liées

* [Comment donner les droits sur les statuts de facture ?](../administration/comment-donner-les-droits-sur-les-statuts-de-facture.md) : statuts autorisés par profil de site ou d'entreprise
* [Comment prendre en charge ou refuser une facture électronique dans INGENEO PRECOMPTA ?](../gestion-des-documents/comment-prendre-en-charge-ou-refuser-une-facture-electronique-dans-ingeneo-precompta.md) : utilisation des boutons de statut dans l'encart de saisie
* [Référence : codes motifs des statuts de la réforme](codes-motifs-des-statuts-de-la-reforme.md) : liste des codes motifs de chaque statut
