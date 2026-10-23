---
description: >-
  Release notes d'INGENEO PRECOMPTA du mois d'octobre 2026 : versions 2.14.3,
  2.13.0, 2.12.0, 2.11.0, 2.10.4, 2.9.10.
icon: calendar
---

# Octobre - 2026

## Version 2.14.3 – 2026-10-23

### <i class="fa-sparkles">:sparkles:</i>Nouveautés

* **Affichage des prochains valideurs** (Réf. 7671) : dans INGENEO PRECOMPTA, dans le menu recherche, `Documents engagés dans un circuit de validation`, l'infobulle indique les prénoms et noms des prochains valideurs du document.

### <i class="fa-arrow-trend-up">:arrow-trend-up:</i>Améliorations

* **Disparition des notes de frais** (Réf. 6637) : dans INGENEO PRECOMPTA, certaines notes de frais ne disparaissent plus. Le correctif s'applique aux notes de frais créées à partir de la version 2.14.3 : les notes déjà disparues ne sont pas restaurées automatiquement.
* **Envoi par mail depuis `Extraire`** (Réf. 7643) : dans INGENEO PRECOMPTA, dans la recherche des documents, vous pouvez envoyer les documents par mail depuis le clic droit > `Extraire`.
* **Saisie de date minimum pour enrôlements systématiquement à J+1** (Réf. 7659) : dans INGENEO PRECOMPTA, dans le formulaire d'enrôlement unitaire, la date minimale saisie ne peut plus être antérieure à J+1. Cette restriction assure la cohérence des dates lors de la création des enrôlements.
* **Suppression des documents des classeurs `Autres documents`** (Réf. 7691) : dans INGENEO PRECOMPTA, dans la recherche, les documents supprimés des classeurs `Autres documents` ne s'affichent plus.
* **Déplacement des documents avec une sélection multiple depuis les classeurs `Autres documents`** (Réf. 7693) : dans INGENEO PRECOMPTA, dans l'onglet `Autres documents`, le clic droit sur une sélection multiple permet de déplacer les documents.
* **Apparition de lignes à 0 € dans la saisie des notes de frais** (Réf. 7739) : dans INGENEO PRECOMPTA, dans l'écran `Comptabilisation` des notes de frais, les lignes supplémentaires à 0 € ne s'affichent plus.
* **Découpage de fichier** (Réf. 7745) : dans INGENEO PRECOMPTA, dans la fonction `Découpage de fichier`, tous les documents sélectionnés sont traités. Le total n'est pas affecté et l'intégrité des données est préservée.

## Version 2.13.0 – 2026-10-19

### <i class="fa-sparkles">:sparkles:</i>Nouveautés

* **Ajout de la connexion banque depuis INGENEO ENTREPRISE** (Réf. 7140) : dans INGENEO PRECOMPTA, dans `Référentiels comptables > Banque`, vous pouvez rattacher une banque directement depuis INGENEO ENTREPRISE.
* **Indicateur sur l'onglet `Notes`** (Réf. 7550) : dans INGENEO PRECOMPTA, dans le panneau latéral du menu `Bannettes`, un indicateur apparaît à droite de l'onglet `Notes` dès qu'il contient des notes. Cet indicateur signale qu'un document comporte des informations supplémentaires.
* **Informations complètes dans les emails de demande d'enrôlement PA** (Réf. 7670) : dans INGENEO PRECOMPTA, l'email de notification d'une demande d'enrôlement à la Plateforme Agréée (PA) contient le nom, le prénom et l'adresse email du demandeur.

### <i class="fa-arrow-trend-up">:arrow-trend-up:</i>Améliorations

* **Défilement correct des documents** (Réf. 6004) : dans INGENEO PRECOMPTA, dans la liste des documents à valider, le défilement vertical fonctionne dès le chargement. Vous accédez directement au document souhaité.
* **Identification des doublons dans les mouvements bancaires** (Réf. 7548) : dans INGENEO PRECOMPTA, certains mouvements bancaires ne sont plus récupérés en double. La correction s'applique aux nouvelles récupérations : les doublons importés avant la version 2.13.0 ne sont pas supprimés automatiquement.

## Version 2.12.0 – 2026-10-15

### <i class="fa-sparkles">:sparkles:</i>Nouveautés

* **Mention d'IA dans le menu `Bannettes`** (Réf. 6102) : dans INGENEO PRECOMPTA, une mention dans le menu `Bannettes` informe que les données sont traitées par intelligence artificielle et doivent être validées. Cette mention respecte le règlement européen sur l'IA.
* **Traçabilité des enrôlements** (Réf. 7060) : dans INGENEO PRECOMPTA, vous pouvez consulter le journal de la plateforme, qui détaille chaque enrôlement réussi ou échoué.
* **Déplacement des documents par un initiateur** (Réf. 7554) : dans INGENEO PRECOMPTA, dans le menu de validation d'un document, l'initiateur d'une facture refusée peut la déplacer vers un autre classeur comptable. Ce déplacement permet de réinitialiser la validation sans effacer les historiques.

## Version 2.11.0 – 2026-10-14

### <i class="fa-arrow-trend-up">:arrow-trend-up:</i>Améliorations

* **Impossibilité de créer un compte dans le plan comptable** (Réf. 7675) : dans INGENEO PRECOMPTA, la création d'un compte dans le plan comptable fonctionne de nouveau.
* **Erreur 503 lors de l'ajout d'une banque** (Réf. 7677) : dans INGENEO PRECOMPTA, dans la configuration des connecteurs bancaires, l'ajout d'une banque fonctionne de nouveau.
* **Problème avec Welyb** (Réf. 7689) : dans INGENEO PRECOMPTA, la connexion avec Welyb est de nouveau opérationnelle. Pour assurer la bonne réception de vos documents dans INGENEO PRECOMPTA, relancez leur envoi ou déposez-les à nouveau.

## Version 2.10.4 – 2026-10-12

### <i class="fa-sparkles">:sparkles:</i>Nouveautés

* **Déplacement de documents depuis la recherche** (Réf. 2515) : dans INGENEO PRECOMPTA, depuis le menu recherche, vous pouvez déplacer des documents non enregistrés vers un autre classeur.
* **Ajout de la colonne Montant HT dans l'export Excel** (Réf. 3035) : dans INGENEO PRECOMPTA, l'export Excel des documents contient une colonne Montant HT à côté du Montant TTC. Vous pouvez utiliser la virgule comme séparateur décimal.
* **Ajout d'un visuel des factures rattachées aux mouvements bancaires** (Réf. 4995) : dans INGENEO PRECOMPTA, le visuel de la facture rattachée à un mouvement bancaire s'affiche en un clic.
* **Ajout de LOGAIA dans la liste des logiciels comptables** (Réf. 7553) : dans INGENEO PRECOMPTA, les exports vers le logiciel comptable LOGAIA sont disponibles.

### <i class="fa-arrow-trend-up">:arrow-trend-up:</i>Améliorations

* **Mise à jour de la reconnaissance des mouvements bancaires** (Réf. 6415) : dans INGENEO PRECOMPTA, les chaînes de reconnaissance des mouvements bancaires sont ajustées aux libellés des mouvements. Elles évitent l'affectation incorrecte des comptes comptables.
* **Post-it et surlignages stabilisés** (Réf. 7240) : dans INGENEO PRECOMPTA, les post-it et surlignages restent visibles tout au long du circuit de validation, sans rechargement de la page. Les annotations ajoutées sont affichées et conservées.
* **Séparation des documents et gestion des notifications** (Réf. 7301) : dans INGENEO PRECOMPTA, les autres documents sont séparés des documents comptables. Vous pouvez sélectionner plusieurs documents pour les marquer comme à ne plus afficher.
* **Enregistrement en brouillon ne perturbe plus les fournisseurs et contacts** (Réf. 7431) : dans INGENEO PRECOMPTA, l'enregistrement d'un engagement de dépense en brouillon sauvegarde correctement les informations du fournisseur et du contact.
* **Restriction de fusion et modification des factures électroniques** (Réf. 7466) : dans INGENEO PRECOMPTA, menu `Bannettes`, vous ne pouvez plus fusionner ni modifier des factures électroniques. Cette restriction garantit leur intégrité.
* **Droits de facture électronique réparés sur classeurs dossiers en réception** (Réf. 7543) : dans INGENEO PRECOMPTA, les options de gestion de la facture électronique s'affichent dans les profils d'entreprises, même avec la réception partielle activée. Le paramétrage des droits est complet.

## Version 2.9.10 – 2026-10-06

### <i class="fa-wrench">:wrench:</i>Corrections

* **Circuit de validation : pas de tampon après validation** (Réf. 7568) : dans INGENEO PRECOMPTA, le tampon est de nouveau apposé après validation dans un circuit de validation.
* **Création compte de tiers depuis le menu `Bannettes` (avec préfixe et auto-complétion)** (Réf. 6429) : correction dans INGENEO PRECOMPTA.
* **Erreur lors de l'accès à la section autres documents dans le menu `Bannettes`** (Réf. 7583) : dans INGENEO PRECOMPTA, l'accès à la section autres documents du menu `Bannettes` ne génère plus d'erreur.
* **Facture électronique : droits `Application des statuts de la réforme` absents sur les classeurs des dossiers en réception** (Réf. 7543) : dans INGENEO PRECOMPTA, les droits `Application des statuts de la réforme` s'affichent sur les classeurs des dossiers en réception.
* **Suppression entreprise impossible** (Réf. 7580) : dans INGENEO PRECOMPTA, la suppression d'une entreprise est de nouveau possible.
