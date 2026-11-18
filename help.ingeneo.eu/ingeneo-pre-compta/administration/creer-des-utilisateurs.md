---
description: >-
  Cette procédure permet d'inviter un nouvel utilisateur sur INGENEO PRECOMPTA,
  depuis les paramètres ou depuis une entreprise, puis de lui attribuer un
  profil de droits.
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

# Comment créer un utilisateur dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet d'inviter un nouvel utilisateur sur la plateforme INGENEO PRECOMPTA, puis de lui attribuer un profil de droits. Elle nécessite le droit `Autoriser l'accès à l'administration de la plateforme.` ou, depuis une entreprise, le droit `Autoriser l'accès à l'administration.`.

## Objectif

Dans INGENEO PRECOMPTA, cette procédure donne accès à la plateforme à une nouvelle personne. Elle se fait de deux façons :

* depuis `Paramètres > Administration > Utilisateurs > Général`, pour un utilisateur qui a les droits d'administration de la plateforme ;
* depuis une entreprise (`Entreprises > Editer > Administration > Utilisateurs`), pour un utilisateur qui a les droits d'administration de cette entreprise.

Dans INGENEO PRECOMPTA, le champ `Type` du panneau d'invitation classe l'utilisateur. Ce choix n'a aucun effet sur ses droits :

* `Interne à la structure` : personne de la structure (exemples : comptable, expert-comptable).
* `Externe à la structure` : personne extérieure à la structure (exemples : client, commissaire aux comptes).

Dans INGENEO PRECOMPTA, les droits d'un utilisateur viennent de ses profils de droits :

* **Profil de site** : droits sur les entreprises d'un site. Attribuez un profil de site à un utilisateur qui doit voir toutes les entreprises d'un site. Les profils `Collaborateur du site` et `Gestionnaire du site` existent par défaut ; leurs droits se consultent dans `Paramètres > Administration > Profils de droits > Profils de site`.
* **Profil d'entreprise** : droits sur une entreprise. Attribuez un profil d'entreprise uniquement à un utilisateur qui doit accéder à une ou quelques entreprises. Deux profils existent par défaut : `Profil d'entreprise collaborateur`, qui donne accès à la pré-saisie comptable, et `Profil d'entreprise client`, qui permet seulement de déposer et de rechercher des documents.

Dans INGENEO PRECOMPTA, un même utilisateur peut cumuler un profil de site et des profils d'entreprise sur des entreprises d'autres sites.

## Prérequis

* Pour créer un utilisateur depuis `Paramètres > Administration > Utilisateurs` dans INGENEO PRECOMPTA, il faut le droit `Autoriser l'accès à l'administration de la plateforme.` dans son profil d'administration. Aucun autre droit n'est nécessaire.
* Pour créer un utilisateur depuis une entreprise dans INGENEO PRECOMPTA, il faut le droit `Autoriser l'accès à l'administration.` dans son profil de site ou dans son profil d'entreprise. Ce droit donne accès au menu `Administration` de l'entreprise.
* Préparez l'adresse e-mail du nouvel utilisateur et le profil de droits à lui attribuer.

## Étapes

### Créer un utilisateur depuis `Paramètres > Administration > Utilisateurs`

1. Dans INGENEO PRECOMPTA, ouvrez `Paramètres > Administration > Utilisateurs > Général`.
2. Cliquez sur `Ajouter` (icône +). Le panneau `Utilisateurs` s'ouvre.
3. Dans le champ `Adresse e-mail`, saisissez l'adresse e-mail du nouvel utilisateur.
4. Dans la liste `Type`, sélectionnez `Interne à la structure` ou `Externe à la structure`. La valeur par défaut est `Externe à la structure`.
5. Si l'utilisateur ne doit pas recevoir son lien de connexion tout de suite, désactivez l'interrupteur `Envoyer l'e-mail d'activation`. Il est activé par défaut.
6. Cliquez sur `Enregistrer`. Le nouvel utilisateur apparaît dans la liste des utilisateurs.
7. Sur la ligne du nouvel utilisateur, cliquez sur le bouton orange `Editer`.
8. Dans le panneau de l'utilisateur, attribuez ses profils de droits dans les onglets `Profil d'administration`, `Profils de site` et `Profils d'entreprise`.
9. Cliquez sur `Enregistrer`.

### Créer un utilisateur depuis une entreprise

1. Dans INGENEO PRECOMPTA, ouvrez `Entreprises`.
2. Sur la ligne de l'entreprise, cliquez sur `Editer`.
3. Cliquez sur l'onglet `Administration`.
4. Cliquez sur `Utilisateurs`.
5. Cliquez sur `Ajouter`. Le panneau `Profil d'entreprise` s'ouvre.
6. Si l'utilisateur existe déjà sur la plateforme, passez directement à l'étape 12.
7. Cliquez sur `Inviter`. Le panneau `Utilisateurs` s'ouvre.
8. Dans le champ `Adresse e-mail`, saisissez l'adresse e-mail du nouvel utilisateur.
9. Dans la liste `Type`, sélectionnez `Interne à la structure` ou `Externe à la structure`.
10. Si l'utilisateur ne doit pas recevoir son lien de connexion tout de suite, désactivez l'interrupteur `Envoyer l'e-mail d'activation`.
11. Cliquez sur `Enregistrer`. Le nouvel utilisateur n'est pas sélectionné automatiquement dans le panneau `Profil d'entreprise`.
12. Dans la liste `Utilisateur` du panneau `Profil d'entreprise`, sélectionnez l'utilisateur.
13. Dans la liste `Profil d'entreprise`, sélectionnez le profil à attribuer (exemples : `Profil d'entreprise client`, `Profil d'entreprise collaborateur`).
14. Cliquez sur `Enregistrer`.

Pour donner à l'utilisateur l'accès à une autre entreprise dans INGENEO PRECOMPTA, refaites les étapes 1 à 5 puis 12 à 14 dans cette entreprise. Un utilisateur qui a le droit `Autoriser l'accès à l'administration de la plateforme.` peut aussi attribuer des profils d'entreprise depuis l'onglet `Profils d'entreprise` du panneau `Editer`, dans `Paramètres > Administration > Utilisateurs`.

## Résultat attendu

Dans INGENEO PRECOMPTA, le nouvel utilisateur apparaît dans `Paramètres > Administration > Utilisateurs > Général`, avec le badge `Interne` ou `Externe` et le badge de ses profils. Un utilisateur créé depuis une entreprise apparaît aussi dans `Entreprises > Editer > Administration > Utilisateurs`, avec son profil dans la colonne `Profil d'entreprise`.

Si `Envoyer l'e-mail d'activation` était activé, l'utilisateur reçoit un e-mail d'activation. Il doit créer son mot de passe depuis cet e-mail avant de pouvoir accéder à INGENEO PRECOMPTA.

## Erreurs fréquentes

* **Le message `Cet utilisateur a déjà été invité.` s'affiche à l'enregistrement du panneau `Utilisateurs`.** Cause : l'adresse e-mail appartient déjà à un utilisateur de la plateforme INGENEO PRECOMPTA. Solution : n'invitez pas l'utilisateur une seconde fois ; attribuez-lui un profil avec le bouton `Editer` de `Paramètres > Administration > Utilisateurs > Général`, ou avec la liste `Utilisateur` du panneau `Profil d'entreprise` de l'entreprise.
* **L'utilisateur n'a pas reçu son lien de connexion, ou a été créé sans e-mail d'activation.** Solution : dans INGENEO PRECOMPTA, ouvrez `Paramètres > Administration > Utilisateurs > Général`, cliquez sur le bouton orange `Editer` de sa ligne, puis cliquez sur `Renvoyer le lien de connexion`.
* **Après `Inviter` dans une entreprise, le nouvel utilisateur n'a pas de profil d'entreprise.** Cause : dans INGENEO PRECOMPTA, l'invitation ne sélectionne pas l'utilisateur dans le panneau `Profil d'entreprise`. Solution : sélectionnez-le dans la liste `Utilisateur`, choisissez le `Profil d'entreprise`, puis cliquez sur `Enregistrer`.
* **L'écran `Paramètres > Administration > Utilisateurs` n'est pas accessible.** Cause : il manque le droit `Autoriser l'accès à l'administration de la plateforme.` dans le profil d'administration de l'utilisateur connecté. Solution : demandez à un administrateur de la plateforme INGENEO PRECOMPTA d'activer ce droit, ou créez l'utilisateur depuis l'entreprise.
* **Le menu `Administration` d'une entreprise n'est pas accessible.** Cause : il manque le droit `Autoriser l'accès à l'administration.` dans le profil de site ou le profil d'entreprise de l'utilisateur connecté. Solution : demandez à un administrateur de la plateforme INGENEO PRECOMPTA d'ajouter ce droit à l'un de ces profils.

## Fiches liées

* [Créer ou modifier un profil de droits](gerer-les-profils-de-droits.md) : création des profils d'administration et de site, et attribution des profils dans `Paramètres > Administration > Utilisateurs`
* [Détail des droits](detail-des-droits.md) : liste et effet des droits des profils de droits d'INGENEO PRECOMPTA

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-creer-utilisateur-ingeneo-precompta
* titre : Comment créer un utilisateur dans INGENEO PRECOMPTA ?
* titre\_menu : Créer des utilisateurs
* type : procedure
* module : Administration
* version\_outil : observé en 2.19.2
* roles\_concernes : administrateur de la plateforme, administrateur d'entreprise
* tags : utilisateur, invitation, profil de site, profil d'entreprise, e-mail d'activation
* formulations\_utilisateur : « Créer des utilisateurs » ; « Créer un utilisateur interne » ; « Créer un utilisateur externe » ; « Création utilisateur client » ; « Création utilisateur collaborateur »
* sources : Refonte de la page GitBook ingeneo-pre-compta/administration/creer-des-utilisateurs ; observation de l'application INGENEO PRECOMPTA 2.19.2 (2026-11-18) ; réponses de l'expert 2026-11-18
* redacteur : CG
* relecteur :
* derniere\_verification : 2026-11-18
* statut : brouillon

</details>
