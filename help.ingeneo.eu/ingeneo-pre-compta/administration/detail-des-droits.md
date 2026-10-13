---
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

# Détail des droits

La [gestion des profils](gerer-les-profils-de-droits.md) de droits est essentielle pour contrôler les droits d'accès des utilisateurs sur la plateforme INGENEO.

Vous retrouverez ci-dessous le détail de chaque droit :

### <sup>Paramétrage de l'entreprise</sup>

| Droit                                                       | Description                                                                                                                                                                         |
| ----------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Autoriser l'accès au paramétrage de l'entreprise            | Active l'ensemble des droits liés au paramétrage de l'entreprise                                                                                                                    |
| Autoriser l'accès au paramétrage des informations générales | Autorise l'utilisateur à la modification des informations générales (Nom de l'entreprise, SIREN, coordonnés…)                                                                       |
| Autoriser l'accès au paramétrage de la comptabilité         | Autorise l'utilisateur à modifier le paramétrage des éléments comptable (logiciel, code dossier, paramétrage général et date d'exercice…) et au paramétrage des classeurs comptable |
| Autoriser l'accès au paramétrage du plan classement         | Autorise l'utilisateur à la création et l'édition des classeurs de plan de classement                                                                                               |
| Autoriser l'accès au paramétrage des processus métier       | Autorise l'utilisateur à la création et à l'édition de l'ensemble des processus métier présents sur la plateforme                                                                   |
| Autoriser l'accès au paramétrage de la collecte             | Autorise l'utilisateur à la création et à l'édition de l'ensemble des canaux de collecte présents sur la plateforme                                                                 |
| Autoriser l'accès à l'administration                        | Autorise l'utilisateur à accéder et modifier le paramétrage des utilisateurs de la plateforme, les profils d'entreprises et donne l'accès à l'archivage de l'entreprise             |

### <sup>Traitements sur l'entreprise</sup>

| Droit                                                                         | Description                                                                                                                                                                                                                                                                                     |
| ----------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Autoriser le lancement de la synchronisation et l'import de FEC.              | Si votre logiciel le permet, autorise l'utilisateur à lancer la synchronisation permettant la récupération des éléments comptables tels que les codes de TVA, les modes de règlement et l'analytique. Autorise également l'utilisateur à réimporter un FEC depuis le paramétrage d'un dossier.  |
| Autoriser l'accès à la génération d'écritures à la demande                    | Si votre logiciel est paramétré pour générer des écritures on Demand, autorise l'utilisateur à générer et télécharger ces écritures                                                                                                                                                             |
| Autoriser la clôture d'exercice ou par situation                              | Autorise l'utilisateur à clôturer une période d'exercice ou a sélectionner l'option de la clôture par situation                                                                                                                                                                                 |
| Autoriser l'accès à la gestion des mots-clés sur les tiers                    | Permet à l'utilisateur d'accéder au paramétrage avancé et de définir des mots-clés pour faciliter la reconnaissance du tiers                                                                                                                                                                    |
| Pas d'apprentissage pour l'utilisateur                                        | Empêche les suggestions automatiques basées sur l'activité de l'utilisateur                                                                                                                                                                                                                     |
| Afficher les propriétés comptables des documents                              | L'activation de ce droit permet notamment la recherche par statut dans le menu Rechercher                                                                                                                                                                                                       |
| Autoriser l'accès au paramétrage des informations bancaires des comptes tiers | Autorise la modification des informations                                                                                                                                                                                                                                                       |

### <sup>Statistiques des sites et des entreprises</sup>

| Droit                                                                                                     | Description                                                                                                                             |
| --------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------- |
| Autoriser l'accès aux statistiques de productivité des entreprises                                        | Permet à l'utilisateur de visualiser les statistiques des entreprises auxquelles il a accès                                             |
| Autoriser l'accès aux statistiques de productivité des sites                                              | Permet à l'utilisateur de visualiser les statistiques des sites auxquels il a accès                                                     |
| Autoriser la création de tableaux de bord personnels sur les statistiques de productivité des entreprises | Donne le droit à l'utilisateur de créer des tableaux de bord sur les statistiques de productivité des entreprises auxquelles il a accès |
| Autoriser la création de tableaux de bord personnels sur les statistiques de productivité des sites       | Donne le droit à l'utilisateur de créer des tableaux de bord sur les statistiques de productivité des sites auxquels il a accès         |

### <sup>Droits sur les classeurs</sup>

Général

| Droit                                                          | Description                                                                                                                 |
| -------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------- |
| Gérer les référentiels associés (ajouter, modifier, supprimer) | Permet à l'utilisateur de gérer les référentiels de l'entreprise (comptes tiers, plan comptable, code TVA, analytique, etc) |
| Accéder à l'historique des actions                             | Voir les actions effectuées dans le classeur                                                                                |

Traitements

| Droit                                                                | Description                                                                                  |
| -------------------------------------------------------------------- | -------------------------------------------------------------------------------------------- |
| Déposer des documents                                                | Déposer des pièces dans les classeurs                                                        |
| Enregistrer les documents                                            | Confirmer l'enregistrement définitif d'un document (le document est exporté en comptabilité) |
| Consulter les documents enregistrés                                  | Voir l'ensemble des documents enregistrés                                                    |
| Consulter uniquement les documents enregistrés où j'ai eu une action | Limite d'accès, restreint la vue aux pièces personnelles                                     |
| Modifier les documents enregistrés                                   | Corriger ou compléter un document validé                                                     |
| Extraire les documents enregistrés                                   | Permet à l'utilisateur de télécharger ou exporter les pièces enregistrées                    |
| Supprimer les documents enregistrés                                  | Permet à l'utilisateur de supprimer une pièce enregistrée                                    |

Annotations / Notes / Pièces jointes

| Droit                                                                             | Description                                                                            |
| --------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------- |
| Ajouter, modifier, supprimer mes annotations (surlignage, post-it, tampon)        | Permet à l'utilisateur de gérer uniquement ses propres annotations                     |
| Ajouter, modifier, supprimer toutes les annotations (surlignage, post-it, tampon) | Permet à l'utilisateur d'avoir une action sur l'ensemble des annotations d'un document |
| Accéder aux notes                                                                 | Permet à l'utilisateur de visualiser les notes                                         |
| Ajouter, modifier, supprimer mes notes                                            | Permet à l'utilisateur de supprimer ses notes personnelles                             |
| Ajouter, modifier, supprimer toutes les notes                                     | Permet à l'utilisateur de supprimer ou modifier l'ensemble des notes                   |
| Accéder aux pièces jointes                                                        | Donne l'accès aux pièces jointes                                                       |
| Ajouter, modifier, supprimer mes pièces jointes                                   | Autorise l'utilisateur des actions sur ses pièces jointes                              |
| Ajouter, modifier, supprimer toutes les pièces jointes                            | Autorise l'utilisateur des actions sur toutes les pièces jointes                       |

Process métier

| Droit                           | Description                                                                           |
| ------------------------------- | ------------------------------------------------------------------------------------- |
| Appliquer les statuts           | Permet à l'utilisateur d'appliquer un statut sur un document présent dans un classeur |
| Mettre les factures au paiement |                                                                                       |
| Payer les factures au paiement  |                                                                                       |
