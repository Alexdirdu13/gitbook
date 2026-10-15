---
description: >-
  Dans INGENEO ENTREPRISE, la case Masquer le contenu promotionnel (Paramètres
  du partenaire > Personnalisation) retire des espaces clients les menus des
  modules hors de leur pack.
---

# Comment afficher ou masquer le contenu promotionnel des plans entreprise dans INGENEO ENTREPRISE ?

**Résumé :** Cette procédure permet d'afficher ou de masquer, dans les espaces de vos clients, les pages de présentation des modules non inclus dans leur pack. Le réglage se fait une seule fois pour tous les clients de l'espace partenaire, dans `Paramètres du partenaire` > `Personnalisation`. Il s'applique dès l'enregistrement.

## Objectif

Dans INGENEO ENTREPRISE, le menu de gauche de l'espace d'un client affiche aussi les modules que son pack ne contient pas. Ces entrées de menu portent une icône de signet. Un clic ouvre une page de présentation du module, avec le bouton `Contactez mon expert →`. C'est le contenu promotionnel des plans entreprise.

Les entrées promotionnelles dépendent du pack du client. Exemples observés :

| Pack du client  | Entrées promotionnelles du menu                | Modules inclus affichés normalement                     |
| --------------- | ---------------------------------------------- | ------------------------------------------------------- |
| `Pack Standard` | `Compte Pro`, `Achats`, `Ventes`, `Trésorerie` | `Accueil`, `Gestion de documents`                       |
| `Pack Pro`      | `Compte Pro`, `Achats`, `Trésorerie`           | `Accueil`, `Gestion de documents`, `Contacts`, `Ventes` |

La case `Masquer le contenu promotionnel des plans entreprise pour vos clients` décide si ces entrées sont visibles :

* **Case décochée :** les entrées promotionnelles et leurs pages de présentation sont affichées dans les espaces clients.
* **Case cochée :** les entrées promotionnelles disparaissent du menu des espaces clients. Seuls les modules inclus dans le pack restent visibles.

Le réglage concerne tous les clients de l'espace partenaire. Il ne se règle pas client par client.

## Prérequis

* Dans INGENEO ENTREPRISE, l'utilisateur a le droit administrateur du Portail de services. Ce droit donne accès au menu `Paramètres du partenaire` de `Mon espace partenaire`.
* Le bouton `Enregistrer` enregistre tout l'onglet `Personnalisation` : `Nom de votre espace de travail`, logo, favicon, couleur principale et cases à cocher. Vérifiez ces champs avant d'enregistrer.

## Étapes

### Masquer le contenu promotionnel

1. Dans INGENEO ENTREPRISE, dans `Mon espace partenaire`, cliquez sur `Paramètres du partenaire`.
2. Cliquez sur l'onglet `Personnalisation`.
3. Faites défiler l'écran jusqu'au bloc `Apparence de l'application`.
4. Cochez la case `Masquer le contenu promotionnel des plans entreprise pour vos clients`.
5. Cliquez sur `Enregistrer`.

### Afficher de nouveau le contenu promotionnel

1. Dans INGENEO ENTREPRISE, dans `Mon espace partenaire`, cliquez sur `Paramètres du partenaire`.
2. Cliquez sur l'onglet `Personnalisation`.
3. Faites défiler l'écran jusqu'au bloc `Apparence de l'application`.
4. Décochez la case `Masquer le contenu promotionnel des plans entreprise pour vos clients`.
5. Cliquez sur `Enregistrer`.
6. Rechargez la page pour mettre à jour le menu de l'espace partenaire.

## Résultat attendu

Après un clic sur `Enregistrer`, le message `Mise à jour effectuée` s'affiche en bas de l'écran.

**Case cochée :**

* Dans l'espace de chaque client, le menu de gauche n'affiche plus les entrées promotionnelles (`Compte Pro`, `Achats`, `Ventes`, `Trésorerie` selon le pack). Les modules inclus dans le pack restent affichés.
* Le masquage s'applique aussi quand un utilisateur partenaire ouvre l'espace d'un client depuis `Liste des clients`.
* Dans l'espace partenaire, le menu `Suivi des opportunités` n'est plus affiché.

**Case décochée :**

* Les entrées promotionnelles réapparaissent dans le menu des espaces clients, avec leurs pages de présentation et le bouton `Contactez mon expert →`.
* Le menu `Suivi des opportunités` réapparaît dans `Mon espace partenaire`, après rechargement de la page.

## Erreurs fréquentes

* **Les clients voient toujours les pages promotionnelles.** Cause : la case a été cochée sans cliquer sur `Enregistrer`. Solution : cochez la case, cliquez sur `Enregistrer`, puis attendez le message `Mise à jour effectuée`.
* **Le menu `Suivi des opportunités` a disparu de l'espace partenaire.** Cause : la case `Masquer le contenu promotionnel des plans entreprise pour vos clients` est cochée. Solution : si vous avez besoin de ce menu, décochez la case, cliquez sur `Enregistrer`, puis rechargez la page.
* **Le menu `Suivi des opportunités` ne revient pas après avoir décoché la case.** Cause : le menu de l'espace partenaire n'est pas mis à jour tout de suite. Solution : rechargez la page.
* **Un client ne trouve plus un module dans son menu.** Cause : le module n'est pas inclus dans son pack et la case est cochée, donc son entrée promotionnelle est masquée. Solution : vérifiez le pack du client dans la colonne `Offre` de `Liste des clients`. Pour donner accès au module, changez l'offre avec `Modifier l'offre commerciale`.

## Fiches liées

* [Guide de démarrage](guide-de-demarrage.md) : choix de l'offre client (standard, pro, business ou premium), qui fixe les modules inclus.
* Comment mettre à jour l'offre commerciale dans INGENEO ENTREPRISE ? (fiche à créer) : bouton `Modifier l'offre commerciale` de `Liste des clients`.
* Comment personnaliser l'apparence de l'espace partenaire dans INGENEO ENTREPRISE ? (fiche à créer) : logo, favicon, couleur principale et case `Appliquer ce thème pour les clients du cabinet` du même onglet `Personnalisation`.
* [Comprendre votre espace entreprise](../cote-entreprise/accueil-et-gestion-des-factures/comprendre-votre-espace-entreprise.md) : menus de l'espace client.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-afficher-masquer-contenu-promotionnel-plans-entreprise-ingeneo-entreprise
* titre : Comment afficher ou masquer le contenu promotionnel des plans entreprise dans INGENEO ENTREPRISE ?
* titre\_menu : Afficher ou masquer le contenu promotionnel
* type : procedure
* module : Paramètres du partenaire > Personnalisation
* version\_outil : toutes
* roles\_concernes : utilisateur partenaire administrateur du Portail de services
* tags : contenu promotionnel, plans entreprise, pack, personnalisation, paramètres du partenaire, Contactez mon expert, Suivi des opportunités
* formulations\_utilisateur : « Comment enlever Achats, Trésorerie et Compte Pro du menu de mes clients ? » ; « Mon client voit des modules qu'il n'a pas dans son pack » ; « Comment retirer le bouton Contactez mon expert ? » ; « Mes clients voient de la publicité pour les packs » ; « Le menu Suivi des opportunités a disparu »
* sources : observation de l'interface et test sur l'espace partenaire Assistance (PRODUCTION) 2026-10-15, dossiers TEST QA (Pack Standard) et DOSSIER TUNIS (Pack Pro) ; case remise dans son état d'origine (décochée) après le test ; réponses de l'expert 2026-10-15 (droit administrateur du Portail de services)
* redacteur : SL
* relecteur :
* derniere\_verification : 2026-10-15
* statut : brouillon

</details>
