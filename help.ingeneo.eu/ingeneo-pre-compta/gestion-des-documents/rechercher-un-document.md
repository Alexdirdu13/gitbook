---
description: >-
  Rechercher un document dans INGENEO PRECOMPTA : mots-clés, statuts, exercice,
  date, filtres avancés et export CSV. Nécessite les droits de consultation sur
  les classeurs.
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

# Comment rechercher un document dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de retrouver un document d'une ou de plusieurs entreprises dans INGENEO PRECOMPTA, avec le menu `Rechercher`. Elle permet aussi d'exporter les résultats en CSV. La durée de la recherche dépend du nombre de résultats. Elle nécessite le droit `Consulter les documents enregistrés` sur les classeurs concernés.

## Objectif

Dans INGENEO PRECOMPTA, le menu `Rechercher` retrouve les documents des [classeurs comptables](../gestion-des-entreprises/classeurs-comptables.md) et du plan de classement d'une entreprise. Il cherche aussi dans les documents de toutes les entreprises de l'utilisateur.

Le menu `Rechercher` permet de :

* chercher un mot dans le contenu des documents, par exemple un article, une adresse ou un nom ;
* filtrer par statut du document, statut d'export, statut de facture électronique, exercice et date ;
* filtrer par ID, numéro de facture, numéro de pièce, compte tiers, montant TTC ou statut ;
* retrouver les documents déposés ou enregistrés par un utilisateur précis, pour contrôler ses actions ;
* exporter la liste des documents ou des écritures trouvés dans un fichier CSV.

## Prérequis

* Droits : dans INGENEO PRECOMPTA, les droits du menu `Rechercher` se donnent classeur par classeur. Exemple d'écran : `Entreprises > Editer > Administration > Profils d'entreprise`, onglet `Droits sur les classeurs`.
  * `Consulter les documents enregistrés` : voir tous les documents enregistrés du classeur.
  * `Consulter uniquement les documents enregistrés où j'ai eu une action` : voir seulement les documents enregistrés sur lesquels l'utilisateur a fait une action.
  * `Extraire les documents enregistrés` : utiliser `Exporter la liste des documents` et `Exporter la liste des écritures`.
  * `Accéder à l'historique des actions` : voir l'historique d'un document trouvé.
* Les documents aux statuts `En bannette` et `En validation` apparaissent dans les résultats sans droit particulier.
* Le détail des droits est dans [Détail des droits](../administration/detail-des-droits.md).
* Recherche dans le contenu : seuls les documents traités par OCRLAD sont trouvés par leur contenu. Un document déposé avec `Ne pas envoyer en OCRLAD` n'est pas trouvé par ce champ.

## Étapes

1. Dans INGENEO PRECOMPTA, cliquez sur `Rechercher` dans le menu de gauche.
2. Dans le bloc `Entreprises` du menu `Rechercher`, cliquez sur l'entreprise. Le champ `Rechercher une entreprise...` filtre la liste.
3. Pour limiter la recherche à un classeur, cliquez sur ce classeur dans le bloc `Classeurs`.
4. Dans la liste de la zone de recherche, sélectionnez `Entreprise en cours` ou `Toutes les entreprises`.
5. Dans le champ `Rechercher dans le contenu des documents et métadonnées...`, saisissez un ou plusieurs mots-clés. Avec `Toutes les entreprises`, ce champ est obligatoire.
6. Pour filtrer par statut, sélectionnez les valeurs voulues dans `Statut(s) du document` : `En bannette`, `En validation`, `Enregistré`, `Supprimé`.
7. Pour filtrer par statut d'export, sélectionnez les valeurs voulues dans `Statut(s) d'export` : `Ne pas exporter`, `En attente d'export`, `En erreur d'export`, `Exporté`, `Enregistré et non exporté`.
8. Pour filtrer par statut du cycle de vie de la facture électronique, sélectionnez une valeur dans `Statut - FE`, par exemple `Déposée`, `Prise en charge`, `Refusée` ou `Encaissée`.
9. Pour filtrer par exercice, sélectionnez l'exercice dans `Exercice`. La valeur par défaut est `Tous`.
10. Pour filtrer par date, sélectionnez le type de date dans `Date` : `Date du document`, `Date de dépôt`, `Date d'enregistrement`, `Date d'export` ou `Date d'échéance`.
11. Si un type de date est choisi, saisissez la période dans `Du` et `Au`.
12. Si un classeur est sélectionné et que vous voulez des filtres avancés, cliquez sur `Filtres`.
13. Dans le panneau `Filtres`, renseignez les filtres voulus :
    * `ID du document` ;
    * `Action d'un utilisateur` : `Déposé` ou `Enregistré`, puis l'utilisateur ;
    * `Méthode d'enregistrement` : `Saisie manuelle` ou `Validation automatique` ;
    * [`Statut`](../processus-metiers/workflow/configurer-les-statuts-de-documents.md) : un statut de la `Liste de statuts`, ou `Aucun statut` ;
    * `Numéro de facture` ;
    * `Numéro de pièce` ;
    * `Compte tiers` ;
    * `Montant TTC` : montant minimum dans `De` et maximum dans `Jusqu'à`.
14. Dans le panneau `Filtres`, cliquez sur `Appliquer`. `Réinitialiser les filtres` vide les filtres, `Retour` ferme le panneau.
15. Cliquez sur `Lancer la recherche`.

Pour exporter les résultats du menu `Rechercher` :

16. Au-dessus de la liste des résultats, cliquez sur le bouton orange à 3 traits.
17. Cliquez sur `Exporter la liste des documents` ou sur `Exporter la liste des écritures`.
18. Ouvrez l'e-mail reçu à l'adresse de votre compte utilisateur.
19. Cliquez sur le lien de l'e-mail pour télécharger le fichier CSV.

## Résultat attendu

Dans INGENEO PRECOMPTA, après un clic sur `Lancer la recherche`, l'onglet `Résultats` affiche le nombre et la liste des documents trouvés. Les colonnes sont `ID`, `Date`, `Classeur` et `Document`. Les boutons `Tout sélectionner` et `Tout désélectionner` agissent sur la liste.

Les résultats du menu `Rechercher` sont perdus dans trois cas :

* l'utilisateur quitte le menu `Rechercher` pour un autre menu ;
* l'utilisateur recharge la page ;
* l'utilisateur ferme l'onglet du navigateur.

Pour garder les résultats, exportez-les. `Exporter la liste des documents` et `Exporter la liste des écritures` exportent tous les résultats de la recherche dans un fichier CSV. Le lien de téléchargement est envoyé par e-mail à l'utilisateur qui a demandé l'export.

La durée d'une recherche dans le menu `Rechercher` dépend du nombre de résultats.

## Erreurs fréquentes

**La recherche sur `Toutes les entreprises` ne fonctionne pas.** Dans le menu `Rechercher` d'INGENEO PRECOMPTA, une recherche sur `Toutes les entreprises` exige un texte dans `Rechercher dans le contenu des documents et métadonnées...`. Les filtres seuls ne suffisent pas.

**Le document recherché n'apparaît pas.** Dans le menu `Rechercher` d'INGENEO PRECOMPTA, vérifiez dans l'ordre :

1. l'entreprise sélectionnée dans le bloc `Entreprises` et la zone `Entreprise en cours` ou `Toutes les entreprises` ;
2. le classeur sélectionné dans le bloc `Classeurs` ;
3. les valeurs de `Statut(s) du document`, `Statut(s) d'export`, `Exercice` et `Date` ;
4. les mots-clés saisis ;
5. le mode de dépôt : un document déposé avec `Ne pas envoyer en OCRLAD` n'est pas trouvé par son contenu. Utilisez les filtres du panneau `Filtres`, par exemple `ID du document`.

**Les filtres avancés ne s'affichent pas.** Dans le menu `Rechercher` d'INGENEO PRECOMPTA, les filtres du panneau `Filtres` n'apparaissent que si un classeur est sélectionné dans le bloc `Classeurs`.

**Un classeur n'apparaît pas dans le bloc `Classeurs`.** Dans le menu `Rechercher` d'INGENEO PRECOMPTA, un classeur comptable ou du plan de classement n'apparaît que s'il contient des documents.

**L'utilisateur ne voit que ses propres documents enregistrés.** Dans INGENEO PRECOMPTA, l'utilisateur a le droit `Consulter uniquement les documents enregistrés où j'ai eu une action` sur ce classeur. Pour voir tous les documents enregistrés, il lui faut le droit `Consulter les documents enregistrés`.

**Les exports ne sont pas disponibles.** Dans le menu `Rechercher` d'INGENEO PRECOMPTA, `Exporter la liste des documents` et `Exporter la liste des écritures` nécessitent le droit `Extraire les documents enregistrés`.

**L'e-mail de l'export n'arrive pas.** Dans INGENEO PRECOMPTA, le lien de l'export CSV est envoyé à l'adresse e-mail du compte utilisateur qui a demandé l'export. Vérifiez le dossier spam ou courrier indésirable, puis l'adresse e-mail de ce compte.

**Les résultats ont disparu.** Dans INGENEO PRECOMPTA, les résultats du menu `Rechercher` sont perdus si l'utilisateur quitte le menu, recharge la page ou ferme l'onglet. Relancez la recherche avec `Lancer la recherche`.

## Fiches liées

* [Détail des droits](../administration/detail-des-droits.md) : droits sur les classeurs qui donnent accès aux résultats et aux exports du menu `Rechercher`.
* [Statut](../processus-metiers/workflow/configurer-les-statuts-de-documents.md) : statuts utilisés par le filtre `Statut` du panneau `Filtres`.
* [Comment faire la pré-saisie comptable d'un document dans INGENEO PRECOMPTA ?](la-saisie-comptable.md) : après `Enregistrer`, le document reste accessible avec le menu `Rechercher`.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-rechercher-document-ingeneo-precompta
* titre : Comment rechercher un document dans INGENEO PRECOMPTA ?
* titre\_menu : Rechercher un document
* type : procedure
* module : Gestion des documents
* version\_outil : 2.15.3 (version observée)
* roles\_concernes : utilisateur avec le droit `Consulter les documents enregistrés` ou `Consulter uniquement les documents enregistrés où j'ai eu une action` sur les classeurs
* tags : recherche, rechercher, filtres, export CSV, statut d'export, facture électronique
* formulations\_utilisateur : « Comment retrouver une facture déjà saisie ? » ; « Je ne trouve pas mon document » ; « Comment chercher dans toutes les entreprises ? » ; « Comment exporter la liste des documents trouvés ? » ; « Comment voir les documents en erreur d'export ? »
* sources : Refonte de la page GitBook ingeneo-pre-compta/gestion-des-documents/rechercher-un-document ; démo Arcade « Rechercher un document » ; observation de l'application INGENEO PRECOMPTA 2.15.3 (2026-10-29) ; réponses de l'expert 2026-10-29
* redacteur : CG
* relecteur :
* derniere\_verification : 2026-10-29
* statut : brouillon

</details>
