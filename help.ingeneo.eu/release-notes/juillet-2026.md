# Juillet - 2026

## **Version 2.8.1 - 17/07/2026**​

**Synchronisation et exports comptables**​

* ​✓ Correctif de synchronisation.
* ​🆕 Prise en charge du logiciel comptable **CEGID One Connect**.

​**Paramétrage des entreprises**​

* ​✓ Import en masse des entreprises.

​**Plateforme Agréée (PA) — mandats et enrôlements**​

* ​🆕 Dépôt manuel d’un mandat unitaire.
* ​✓ Import en masse des informations manquantes.
* ​✓ Fin des blocages des mandats en attente.
* ​✓ Fin des blocages d’enrôlement liés au signataire du cabinet.
* ​✓ Affichage dans Ingeneo des motifs de refus d’enrôlement de la PA.
* ​✓ Correctifs divers sur les mandats et les enrôlements.
* ​✓ Correctif des lignes dupliquées pour les mailles SIREN.
* ​✓ Réinitialisation des demandes d’enrôlement pour certaines plateformes

***

## **Version 2.8.0 - 13/07/2026**

**Mandats & Enrôlements PA**

* 🆕 Séparation en 2 workflows distincts : gestion des mandats / gestion des enrôlements
* 🆕 Revue de l'interface : coches de sélection, filtres, lisibilité (code dossier / raison sociale /  \
  SIREN)

🆕 **Mandats**

* Toutes les entreprises affichées, gestion par code dossier et non plus par SIREN
* Mise à jour des informations via formulaire (infos nécessaires au mandat et à l'enrôlement)
* Actions unitaires : envoi en signature, relance client, annulation de signature, suppression  \
  du mandat (si aucun enrôlement en cours), génération "mandat cabinet" (décharge la PA du  \
  KYC/KYB)
* Toutes les actions unitaires disponibles en masse via multi-sélection
* Actions globales :  \
  \- Signature unique cabinet pour toutes les signatures en attente sur YouSign  \
  \- Dépôt fichier .zip pour les mandats gérés hors Ingeneo  \
  \- Mise à jour des informations manquantes avec téléchargement d'un modèle prérempli  \
  (possibilité de renseigner plusieurs mailles pour une même entreprise)  \
  \- Export Excel des informations

&#x20;  🆕**Enrôlements**

* Affichage limité aux entreprises avec un mandat signé
* Actions unitaires : demande d'enrôlement, visualisation et modification des informations (si  \
  enrôlement non encore envoyé), annulation d'un enrôlement envoyé mais non finalisé
* Toutes les actions unitaires disponibles en masse via multi-sélection
* 2 dossiers avec le même SIREN peuvent désormais faire l'objet de 2 enrôlements distincts  \
  avec des mailles différentes.

