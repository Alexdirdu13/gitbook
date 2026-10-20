---
description: >-
  Dans INGENEO PRECOMPTA, connecter une banque d'une entreprise à Powens permet
  la récupération automatique des mouvements bancaires dans un classeur Banque.
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

# Comment connecter un compte bancaire avec Powens dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de connecter une banque d'une entreprise à Powens dans INGENEO PRECOMPTA, pour récupérer automatiquement ses mouvements bancaires. Elle prend environ 5 minutes. Elle nécessite le droit `Autoriser l'accès au paramétrage de la comptabilité`.

## Objectif

Dans INGENEO PRECOMPTA, Powens récupère automatiquement les mouvements bancaires d'une entreprise. La connexion se paramètre dans `Entreprises > Editer > Entreprise > Référentiels comptables > Banque`. Les mouvements bancaires arrivent dans le classeur comptable de type `Banque` lié au compte.

Deux méthodes de connexion existent dans INGENEO PRECOMPTA :

* vous avez les identifiants bancaires : vous connectez la banque vous-même avec `Connecter la banque avec Powens` ;
* vous n'avez pas les identifiants bancaires : vous envoyez une demande de connexion au détenteur du compte, avec `Envoyer la requête de connexion à un utilisateur.`.

Limites de Powens dans INGENEO PRECOMPTA :

* la connexion nécessite les identifiants de connexion bancaire ;
* la banque demande une double authentification ;
* tous les établissements bancaires ne sont pas compatibles avec Powens ;
* la connexion requiert l'accord explicite du détenteur du compte.

{% hint style="warning" %}
Dans INGENEO PRECOMPTA, la connexion Powens nécessite la transmission d'identifiants bancaires sensibles. Assurez-vous du consentement explicite de votre client. Respectez les obligations RGPD en matière de protection des données financières.
{% endhint %}

## Prérequis

* Droit INGENEO PRECOMPTA : l'utilisateur qui paramètre la connexion doit avoir le droit [`Autoriser l'accès au paramétrage de la comptabilité`](../../administration/detail-des-droits.md).
* Classeur `Banque` : l'entreprise doit avoir un classeur comptable de type `Banque`, pour y recevoir les mouvements bancaires. La création d'un classeur est décrite dans [Créer et paramétrer un classeur comptable](../../gestion-des-entreprises/classeurs-comptables.md).
* Identifiants bancaires : pour connecter la banque vous-même, munissez-vous des identifiants bancaires et de l'accès à la double authentification de la banque.
* Détenteur du compte : pour envoyer une demande de connexion, le détenteur du compte bancaire doit être un utilisateur d'INGENEO PRECOMPTA rattaché à l'entreprise.
* Comptes bancaires : ne créez pas les comptes à la main. La connexion Powens crée automatiquement les comptes de la banque.

## Étapes

### Ajouter la banque au référentiel

Dans INGENEO PRECOMPTA, la banque doit être ajoutée à `Référentiels comptables > Banque` avant toute connexion Powens.

1. Dans INGENEO PRECOMPTA, cliquez sur `Entreprises` dans le menu de gauche.
2. Sur l'écran `Entreprises`, sur la ligne de l'entreprise, cliquez sur `Editer`.
3. Dans l'onglet `Entreprise`, cliquez sur `Référentiels comptables`.
4. Cliquez sur `Banque`.
5. Cliquez sur `Ajouter`.
6. Dans le panneau `Création d'une banque`, saisissez le `Nom de la banque`.
7. Cliquez sur `Enregistrer`.

Le panneau `Création d'une banque` contient aussi le champ `BIC / SWIFT`, de 8 ou 11 caractères. La banque apparaît dans la liste, avec le badge `NON CONNECTÉ` dans la colonne `Récup. Auto.`.

### Connecter la banque avec les identifiants bancaires

Dans INGENEO PRECOMPTA, sur la ligne d'une banque de `Référentiels comptables > Banque`, l'icône de banque `Gérer la récupération automatique` ouvre le panneau `Gestion de la récupération automatique`.

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Banque`.
2. Sur la ligne de la banque, cliquez sur l'icône de banque `Gérer la récupération automatique`.
3. Dans le panneau `Gestion de la récupération automatique`, cliquez sur `Connecter la banque avec Powens`.
4. Dans la nouvelle fenêtre Powens, sélectionnez l'établissement bancaire.
5. Saisissez les identifiants bancaires.
6. Validez la double authentification demandée par la banque.
7. Sélectionnez les comptes bancaires à utiliser.
8. De retour dans le panneau `Gestion de la récupération automatique`, cliquez sur `Enregistrer`.

Le panneau affiche le message `Après avoir effectué une connexion, veuillez fermer puis ré-ouvrir cette fenêtre.`. Fermer puis rouvrir le panneau sert seulement à rafraîchir son affichage.

### Envoyer une demande de connexion au détenteur du compte

Dans INGENEO PRECOMPTA, si vous n'avez pas les identifiants bancaires, envoyez une demande de connexion au détenteur du compte. Seuls les utilisateurs rattachés à l'entreprise peuvent être choisis.

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Banque`.
2. Sur la ligne de la banque, cliquez sur l'icône de banque `Gérer la récupération automatique`.
3. Dans le panneau `Gestion de la récupération automatique`, cliquez sur `Envoyer la requête de connexion à un utilisateur.`.
4. Recherchez l'utilisateur détenteur du compte bancaire.
5. Sur la ligne de l'utilisateur, cliquez sur le bouton vert à coche.

L'utilisateur reçoit un e-mail d'invitation à se connecter à INGENEO PRECOMPTA.

### Connecter la banque depuis une demande reçue

Dans INGENEO PRECOMPTA, le détenteur du compte bancaire qui a reçu une demande de connexion Powens fait la connexion depuis ses notifications.

1. Connectez-vous à INGENEO PRECOMPTA.
2. Cliquez sur l'icône cloche des notifications.
3. Sur la demande de connexion, cliquez sur l'icône œil.
4. Cliquez sur `POWENS`.
5. Dans la fenêtre Powens, sélectionnez votre établissement bancaire.
6. Saisissez vos identifiants bancaires.
7. Sélectionnez les comptes bancaires à utiliser.

### Lier un classeur Banque au compte bancaire

Dans INGENEO PRECOMPTA, après la connexion Powens, aucun classeur n'est sélectionné par défaut pour les comptes créés. Liez à la main un classeur comptable de type `Banque` à chaque compte, pour y recevoir les mouvements bancaires.

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Banque`.
2. Sur la ligne du compte, cliquez sur le bouton d'édition (icône crayon orange).
3. Dans le champ `Classeur`, sélectionnez le classeur comptable de type `Banque`.
4. Cliquez sur `Enregistrer`, en bas à droite du panneau.

### Renouveler la connexion Powens

Dans INGENEO PRECOMPTA, la connexion Powens d'une banque doit être renouvelée environ tous les trois mois, quand la banque se déconnecte. INGENEO PRECOMPTA avertit l'utilisateur de deux façons :

* dans le classeur `Banque` du menu `Bannettes`, un bandeau orange affiche `Une ou plusieurs banques ne sont plus synchronisées avec Powens.`, avec le bouton `Consulter les banques` ;
* dans `Référentiels comptables > Banque`, le badge vert `CONNECTÉ` est remplacé par le badge orange `UNE ACTION EST REQUISE`.

Pour renouveler la connexion :

1. Dans le menu `Bannettes`, dans le classeur `Banque` de l'entreprise, cliquez sur `Consulter les banques`.
2.  Dans `Référentiels comptables > Banque`, sur la ligne marquée `UNE ACTION EST REQUISE`, cliquez sur l'icône de banque `Gérer la récupération automatique`.

    Le panneau `Gestion de la récupération automatique` affiche le bandeau orange `La synchronisation a échoué car les informations d'identification dont nous disposons sont invalides ou obsolètes.`.
3. Si vous avez les identifiants bancaires, cliquez sur `cliquez-ici pour renouveler la connexion`, puis suivez les écrans de Powens.
4. Si vous n'avez pas les identifiants bancaires, cliquez sur `Envoyer la requête à un utilisateur`.
5. Une fois la connexion renouvelée, cliquez sur `Enregistrer`.

### Désactiver la connexion ou supprimer le compte

Dans INGENEO PRECOMPTA, une connexion Powens se retire de deux façons, depuis `Entreprises > Editer > Entreprise > Référentiels comptables > Banque` :

* pour désactiver la connexion avec Powens, cliquez sur l'icône de banque `Gérer la récupération automatique`, puis sur le bouton rouge `Désactiver la connexion avec Powens` ;
* pour supprimer le compte, cliquez sur le bouton de suppression (icône corbeille rouge) à droite de la ligne du compte.

Dans les deux cas, les mouvements bancaires déjà récupérés restent dans le classeur `Banque`, en attente de traitement.

## Résultat attendu

Dans INGENEO PRECOMPTA, `Entreprises > Editer > Entreprise > Référentiels comptables > Banque` affiche le badge vert `CONNECTÉ` dans la colonne `Récup. Auto.` de la banque. Les comptes bancaires sélectionnés dans Powens apparaissent dans la liste, chacun lié à un classeur `Banque` dans la colonne `Classeur`.

* La récupération des mouvements bancaires débute 48 à 72 heures après la connexion.
* Les mouvements bancaires arrivent dans le classeur `Banque` lié au compte, dans le menu `Bannettes`.
* La fréquence de récupération (quotidienne, hebdomadaire ou mensuelle) se choisit dans l'établissement bancaire, pas dans INGENEO PRECOMPTA.

## Erreurs fréquentes

**La banque n'apparaît pas dans la liste de Powens.** Dans INGENEO PRECOMPTA, la fenêtre Powens ne propose que les établissements bancaires compatibles avec Powens. Vérifiez que l'établissement bancaire est compatible avec Powens, ou contactez le support technique.

**Le détenteur du compte ne reçoit pas l'e-mail d'invitation.** Dans INGENEO PRECOMPTA, après une demande de connexion Powens, vérifiez l'adresse e-mail renseignée dans le profil de l'utilisateur. Demandez-lui de consulter son dossier de courriers indésirables.

**Le détenteur du compte n'apparaît pas dans la liste des utilisateurs.** Dans INGENEO PRECOMPTA, `Envoyer la requête de connexion à un utilisateur.` ne propose que les utilisateurs rattachés à l'entreprise. Le détenteur du compte doit être rattaché à l'entreprise pour recevoir la demande.

**Aucun mouvement bancaire n'arrive dans le classeur `Banque`.** Dans INGENEO PRECOMPTA, vérifiez trois points dans `Référentiels comptables > Banque` :

* la colonne `Récup. Auto.` affiche `CONNECTÉ` ;
* la colonne `Classeur` du compte indique un classeur de type `Banque` ;
* la connexion date de plus de 72 heures.

**Le badge `UNE ACTION EST REQUISE` s'affiche.** Dans INGENEO PRECOMPTA, la banque s'est déconnectée de Powens, en général après environ trois mois. Cliquez sur l'icône de banque `Gérer la récupération automatique`, puis sur `cliquez-ici pour renouveler la connexion`. Cliquez ensuite sur `Enregistrer`.

## Fiches liées

* [Créer et paramétrer un classeur comptable](../../gestion-des-entreprises/classeurs-comptables.md) : création du classeur `Banque` qui reçoit les mouvements bancaires.
* [Dépôt EBICS](../configuration-ebics/depot-ebics.md) : import de mouvements bancaires aux formats CFONB ou OFX, quand la connexion Powens n'est pas possible.
* [Paramétrage connecteur marchand](../../collecte-automatique/parametrage-connecteur-marchand.md) : autre canal de collecte qui utilise Powens.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-connecter-compte-bancaire-powens-ingeneo-precompta
* titre : Comment connecter un compte bancaire avec Powens dans INGENEO PRECOMPTA ?
* titre\_menu : Connecter un compte bancaire avec Powens
* type : procedure
* module : Banque
* version\_outil : 2.12.0 (version observée)
* roles\_concernes : utilisateur avec le droit `Autoriser l'accès au paramétrage de la comptabilité` ; détenteur du compte bancaire rattaché à l'entreprise
* tags : Powens, banque, récupération automatique, mouvements bancaires, classeur Banque, référentiels comptables
* formulations\_utilisateur : « Comment paramétrer Powens ? » ; « Comment connecter la banque de mon client ? » ; « Je n'ai pas les identifiants bancaires de mon client » ; « Les mouvements bancaires ne remontent pas » ; « Une action est requise sur ma banque » ; « Ma banque n'est plus synchronisée avec Powens »
* sources : Refonte de la page GitBook ingeneo-pre-compta/banque/connecteurs-tiers/parametrage-powens ; démo Arcade « Connexion via POWENS » (retirée) ; observation de l'application INGENEO PRECOMPTA 2.12.0 (2026-10-19) ; réponses de l'expert 2026-10-19 et 2026-10-20
* redacteur : CH
* relecteur :
* derniere\_verification : 2026-10-20
* statut : brouillon

</details>
