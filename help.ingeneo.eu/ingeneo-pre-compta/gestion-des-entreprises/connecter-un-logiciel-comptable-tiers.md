---
description: >-
  Dans INGENEO PRECOMPTA, connecter une entreprise à un logiciel comptable tiers
  (MyUnisoft, Pennylane, Fulll ou CEGID ONE CONNECT) active l'export automatique
  des documents et de leurs écritures.
---

# Comment connecter une entreprise à un logiciel comptable tiers dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de connecter une entreprise d'INGENEO PRECOMPTA à un logiciel comptable tiers : MyUnisoft, Pennylane, Fulll ou CEGID ONE CONNECT. Elle prend environ 4 minutes. Elle nécessite le droit `Autoriser l'accès au paramétrage de la comptabilité`.

## Objectif

Dans INGENEO PRECOMPTA, une entreprise peut être connectée par API à l'un des logiciels comptables tiers suivants : MyUnisoft, Pennylane, Fulll ou CEGID ONE CONNECT. La connexion se paramètre dans `Entreprises > Editer > Entreprise > Comptabilité`.

Une fois l'interconnexion active :

* les documents et leurs écritures sont exportés automatiquement vers le logiciel tiers après `Enregistrer` dans l'écran de pré-saisie comptable ;
* les référentiels de l'entreprise peuvent être synchronisés depuis `Référentiels comptables`, sauf avec CEGID ONE CONNECT.

Utilisez cette procédure à la création d'une entreprise ou au passage d'une entreprise vers l'un de ces logiciels comptables.

## Prérequis

* Droit INGENEO PRECOMPTA : l'utilisateur doit avoir le droit `Autoriser l'accès au paramétrage de la comptabilité`. Sans ce droit, le menu `Comptabilité` de l'entreprise est masqué.
* Compte dans le logiciel tiers : pour MyUnisoft, Pennylane et Fulll, l'utilisateur doit se connecter avec un compte du logiciel tiers qui a les droits nécessaires sur le dossier. Les droits requis sont décrits dans la documentation de chaque logiciel tiers.
* Clés CEGID ONE CONNECT : pour CEGID ONE CONNECT, récupérez la `Clé d'identification` et le `Secret d'identification` dans CEGID ONE CONNECT avant de commencer.
* Code dossier : la connexion à un logiciel tiers ne modifie pas le `Code dossier` de l'entreprise.

## Étapes

### Choisir le logiciel tiers

1. Dans INGENEO PRECOMPTA, cliquez sur `Entreprises` dans le menu de gauche.
2. Sur l'écran `Entreprises`, sur la ligne de l'entreprise, cliquez sur `Editer`.
3. Dans l'onglet `Entreprise`, cliquez sur `Comptabilité`.
4. Dans l'onglet `Paramétrage général`, bloc `LOGICIEL COMPTABLE`, ouvrez le champ `Logiciel`.
5. Sélectionnez le logiciel tiers : MyUnisoft, Pennylane, Fulll ou CEGID ONE CONNECT.
6. Cliquez sur `Enregistrer`.

Un nouvel onglet s'affiche à droite de l'onglet `Paramétrage avancé`. Par exemple, pour Pennylane, l'onglet s'appelle `Pennylane`.

### Lier un compte MyUnisoft, Pennylane ou Fulll

Dans INGENEO PRECOMPTA, l'onglet du logiciel tiers se trouve dans `Entreprises > Editer > Entreprise > Comptabilité`. Avant la connexion, son bloc `CONNEXION API AVEC LE LOGICIEL DE COMPTABILITÉ` affiche le message `Aucune liaison API paramétrée.`

1. Dans `Entreprises > Editer > Entreprise > Comptabilité`, cliquez sur l'onglet du logiciel tiers.
2. Cliquez sur `Lier un compte à ce dossier comptable`.
3. Sur la page du logiciel tiers qui s'ouvre, connectez-vous avec votre compte du logiciel tiers.
4. Autorisez l'accès demandé par le logiciel tiers.

De retour dans INGENEO PRECOMPTA, l'onglet du logiciel tiers affiche `Interconnexion active`.

### Renseigner les clés CEGID ONE CONNECT

Dans INGENEO PRECOMPTA, quand le champ `Logiciel` de l'entreprise est CEGID ONE CONNECT, l'onglet du logiciel tiers contient deux champs : `Clé d'identification` et `Secret d'identification`. Ces deux valeurs se récupèrent dans CEGID ONE CONNECT.

1. Dans `Entreprises > Editer > Entreprise > Comptabilité`, cliquez sur l'onglet du logiciel tiers.
2. Dans le champ `Clé d'identification`, saisissez la clé fournie par CEGID ONE CONNECT.
3. Dans le champ `Secret d'identification`, saisissez le secret fourni par CEGID ONE CONNECT.
4. Cliquez sur `Enregistrer`.

L'onglet du logiciel tiers affiche `Interconnexion active`.

### Synchroniser les référentiels

Dans INGENEO PRECOMPTA, la synchronisation des référentiels avec un logiciel tiers ne se lance pas automatiquement. Elle est disponible avec MyUnisoft, Pennylane et Fulll, mais pas avec CEGID ONE CONNECT.

1. Vérifiez que l'onglet du logiciel tiers, dans `Entreprises > Editer > Entreprise > Comptabilité`, affiche `Interconnexion active`.
2. Dans l'onglet `Entreprise`, cliquez sur `Référentiels comptables`.
3. Cliquez sur `Synchroniser`.

### Retirer l'interconnexion

Dans INGENEO PRECOMPTA, une interconnexion active avec un logiciel tiers se retire de deux façons, depuis `Entreprises > Editer > Entreprise > Comptabilité` :

* dans l'onglet du logiciel tiers, cliquez sur `Déconnecter` ;
* ou, dans l'onglet `Paramétrage général`, changez la valeur du champ `Logiciel`, puis cliquez sur `Enregistrer`.

Pour lier un autre compte du logiciel tiers, cliquez sur `Déconnecter`, puis cliquez sur `Lier un compte à ce dossier comptable`.

## Résultat attendu

Dans INGENEO PRECOMPTA, l'onglet du logiciel tiers de `Entreprises > Editer > Entreprise > Comptabilité` affiche `Interconnexion active`. Le `Code dossier` de l'entreprise reste inchangé.

* Après `Enregistrer` dans l'écran de pré-saisie comptable, les documents et leurs écritures partent automatiquement vers le logiciel tiers.
* Avec MyUnisoft, Pennylane et Fulll, un clic sur `Synchroniser` dans `Référentiels comptables` récupère les référentiels du logiciel tiers.

## Erreurs fréquentes

**Le menu `Comptabilité` de l'entreprise n'apparaît pas.** Dans INGENEO PRECOMPTA, le menu `Comptabilité` d'une entreprise n'est visible qu'avec le droit `Autoriser l'accès au paramétrage de la comptabilité`. Demandez à un administrateur d'ajouter ce droit à votre profil.

**Des documents sont en attente d'export ou en erreur d'export vers le logiciel tiers.** Dans INGENEO PRECOMPTA, le bouton `Alertes` (point d'exclamation, en haut à gauche de l'écran) liste les documents en attente d'export et en erreur d'export.

1. Dans `Entreprises > Editer > Entreprise > Comptabilité`, vérifiez que l'onglet du logiciel tiers affiche `Interconnexion active`.
2. Si l'onglet n'affiche pas `Interconnexion active`, liez de nouveau le compte du logiciel tiers ou ressaisissez les clés CEGID ONE CONNECT.
3. Dans le menu `Rechercher`, faites un clic droit sur le document.
4. Cliquez sur `Remettre à l'export`.

**Le message `Erreur de synchronisation` s'affiche.** Dans INGENEO PRECOMPTA, ce message s'affiche au lancement de `Synchroniser` dans `Référentiels comptables`. Il indique souvent la raison de l'erreur.

1. Lisez la raison indiquée dans le message `Erreur de synchronisation`.
2. Vérifiez que l'onglet du logiciel tiers, dans `Entreprises > Editer > Entreprise > Comptabilité`, affiche `Interconnexion active`.
3. Corrigez la cause indiquée par le message.
4. Dans `Référentiels comptables`, cliquez de nouveau sur `Synchroniser`.

## Fiches liées

* [Paramétrage général de la comptabilité](parametrage-comptabilite.md) : champ `Logiciel` et `Code dossier` du bloc `LOGICIEL COMPTABLE`.
* [Pré-saisie comptable d'un document](../gestion-des-documents/la-saisie-comptable.md) : enregistrement qui déclenche l'export automatique vers le logiciel tiers.
* [Référentiels comptables](referentiels-comptables.md) : synchronisation des référentiels avec le logiciel tiers.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-connecter-logiciel-comptable-tiers-ingeneo-precompta
* titre : Comment connecter une entreprise à un logiciel comptable tiers dans INGENEO PRECOMPTA ?
* titre\_menu : Connecter un logiciel comptable tiers
* type : procedure
* module : Gestion des entreprises
* version\_outil : 2.12.0 (version observée)
* roles\_concernes : utilisateur avec le droit `Autoriser l'accès au paramétrage de la comptabilité`
* tags : logiciel tiers, interconnexion, API, Pennylane, MyUnisoft, Fulll, CEGID ONE CONNECT
* formulations\_utilisateur : « Comment connecter Pennylane à INGENEO PRECOMPTA ? » ; « Comment lier un dossier à MyUnisoft ? » ; « Où mettre la clé API Cegid One Connect ? » ; « Mes documents ne partent pas dans Fulll » ; « J'ai une erreur de synchronisation avec Pennylane » ; « Comment déconnecter le logiciel comptable ? »
* sources : observation de l'application INGENEO PRECOMPTA 2.12.0, environnement de démonstration (2026-10-19) ; réponses de l'expert 2026-10-19
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-19
* statut : brouillon

</details>
