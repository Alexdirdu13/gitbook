---
description: >-
  Créer, modifier, dupliquer, supprimer et attribuer un profil d'administration
  ou un profil de site dans INGENEO PRECOMPTA.
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

# Comment créer ou modifier un profil de droits dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de créer, modifier, dupliquer, supprimer et attribuer un profil d'administration ou un profil de site dans INGENEO PRECOMPTA. Elle nécessite le droit `Autoriser l'accès à l'administration de la plateforme.` dans le profil d'administration de l'utilisateur.

## Objectif

Dans INGENEO PRECOMPTA, un profil de droits définit les fonctionnalités auxquelles un utilisateur a accès. Il existe deux types de profils de droits, gérés dans `Paramètres > Administration > Profils de droits` :

* **Profil d'administration** : droits sur l'administration et la configuration de la plateforme INGENEO PRECOMPTA. Un utilisateur a un seul profil d'administration.
* **Profil de site** : droits sur toutes les entreprises rattachées à un site, y compris les droits sur les classeurs comptables et les notifications par e-mail. Un utilisateur reçoit un profil de site pour chaque site.

Dans INGENEO PRECOMPTA, utilisez cette procédure à l'arrivée d'un nouvel utilisateur ou lors d'un changement de périmètre métier. Pour un accès temporaire, attribuez plutôt un profil existant ou un profil d'entreprise. Le profil d'entreprise donne des droits sur une seule entreprise et l'emporte sur le profil de site.

## Prérequis

* Dans INGENEO PRECOMPTA, l'utilisateur qui gère les profils de droits a le droit `Autoriser l'accès à l'administration de la plateforme.` dans son profil d'administration.
* Avant de créer des profils de droits dans INGENEO PRECOMPTA, listez les rôles des utilisateurs et leurs besoins d'accès.
* Définissez les périmètres fonctionnels de chaque profil (exemples : pré-saisie comptable, paramétrage).
* Choisissez une nomenclature claire pour les intitulés (exemples : « Admin Site », « Lecture Comptable »).
* Accordez à chaque profil les droits minimums adaptés au poste, et non tous les droits par défaut.

{% hint style="warning" %}
Dans INGENEO PRECOMPTA, un profil de droits mal configuré peut donner à des utilisateurs un accès non souhaité à des données sensibles. Vérifiez chaque droit activé avant d'enregistrer le profil.
{% endhint %}

## Étapes

### Créer un profil d'administration

1. Dans INGENEO PRECOMPTA, ouvrez `Paramètres > Administration > Profils de droits`.
2. Cliquez sur l'onglet `Profils d'administration`.
3. Cliquez sur `Ajouter`.
4. Dans le panneau `Profil de droit`, saisissez le nom du profil dans le champ `Intitulé`.
5. Activez les interrupteurs des droits à accorder. Ils sont répartis en 4 blocs : `PARAMÉTRAGE DE LA PLATEFORME`, `GESTION DES ENTREPRISES & AUTORISATIONS GLOBALES`, `STATISTIQUES DE LA PLATEFORME ET DES SITES`, `PORTAIL DE SERVICES`.
6. Cliquez sur `Enregistrer` en bas à droite du panneau `Profil de droit`.

Dans INGENEO PRECOMPTA, un profil d'administration ne contient pas de droits sur les classeurs comptables. Ces droits se règlent dans un profil de site ou un profil d'entreprise. Avec le droit `Autoriser la création d'entreprise.`, l'utilisateur doit aussi avoir au moins un profil de site, pour rattacher l'entreprise créée à un site.

### Créer un profil de site

Dans INGENEO PRECOMPTA, le panneau `Profil de droit` d'un profil de site comporte trois étapes : `Profil de site`, `Droits sur les classeurs` et `Notifications`.

1. Dans INGENEO PRECOMPTA, ouvrez `Paramètres > Administration > Profils de droits`.
2. Cliquez sur l'onglet `Profils de site`.
3. Cliquez sur `Ajouter`.
4. Dans le panneau `Profil de droit`, étape `Profil de site`, saisissez le nom du profil dans le champ `Intitulé`.
5. Activez les interrupteurs des droits à accorder. Ils sont répartis en 4 blocs : `PARAMÉTRAGE DE L'ENTREPRISE`, `TRAITEMENTS SUR L'ENTREPRISE`, `STATISTIQUES DES SITES ET DES ENTREPRISES`, `PORTAIL DE SERVICES`.
6. Cliquez sur l'étape `Droits sur les classeurs`.
7. Cliquez sur l'onglet d'un type de classeur : `Factures d'achat`, `Factures de vente`, `Caisse`, `Banque`, `Plan de classement`, `Notes de frais` ou `Autres documents`.
8. Activez les interrupteurs des droits à accorder pour ce type de classeur. Pour tout accorder, activez `Cocher tous les droits`.
9. Répétez les étapes 7 et 8 pour chaque type de classeur.
10. Si les utilisateurs du profil doivent recevoir des e-mails, cliquez sur l'étape `Notifications` et réglez les notifications voulues.
11. Cliquez sur `Enregistrer` en bas à droite du panneau `Profil de droit`.

Dans INGENEO PRECOMPTA, les droits d'un onglet de l'étape `Droits sur les classeurs` s'appliquent à tous les classeurs comptables de ce type. Exemple : les droits de l'onglet `Factures d'achat` s'appliquent à tous les classeurs de type `Factures d'achat`. Chaque onglet regroupe ses droits en blocs `GÉNÉRAL`, `TRAITEMENTS`, `ANNOTATIONS / NOTES / PIÈCES JOINTES` et `PROCESS MÉTIER`.

### Régler les notifications d'un profil de site

Dans INGENEO PRECOMPTA, l'étape `Notifications` du panneau `Profil de droit` d'un profil de site propose 3 notifications par e-mail. Elles sont envoyées aux utilisateurs rattachés à ce profil de site :

* `Activer les notifications des documents déposés sur les entreprises du site` ;
* `Activer les notifications des documents en attente de traitement sur les entreprises du site` ;
* `Activer les notifications des documents en attente de validation sur les entreprises du site`.

Pour chaque notification à envoyer :

1. Activez l'interrupteur de la notification.
2. Si l'e-mail doit partir une semaine sur deux, activez `Réception une semaine sur 2`. Sinon, l'e-mail part chaque semaine.
3. Sous `Jour(s) de réception`, activez l'interrupteur de chaque jour d'envoi (`Lun` à `Dim`).
4. Sous `Heure(s) de réception`, saisissez l'heure d'envoi.
5. Pour envoyer l'e-mail à plusieurs heures dans la journée, cliquez sur `+` et saisissez chaque heure supplémentaire. Un e-mail part à chaque heure saisie.

La croix rouge à droite d'une heure la retire. Cliquez sur `Enregistrer` en bas à droite du panneau `Profil de droit` pour valider les notifications.

### Modifier un profil de droits

1. Dans INGENEO PRECOMPTA, ouvrez `Paramètres > Administration > Profils de droits`.
2. Cliquez sur l'onglet `Profils d'administration` ou `Profils de site`.
3. Sur la ligne du profil, cliquez sur le bouton orange `Editer`.
4. Dans le panneau `Profil de droit`, modifiez l'intitulé ou les interrupteurs voulus.
5. Cliquez sur `Enregistrer` en bas à droite du panneau `Profil de droit`.

Dans INGENEO PRECOMPTA, la modification d'un profil de droits change les droits de tous les utilisateurs qui ont ce profil. La colonne `Utilisateurs` de la liste indique leur nombre.

### Dupliquer un profil de droits

1. Dans INGENEO PRECOMPTA, ouvrez `Paramètres > Administration > Profils de droits`.
2. Cliquez sur l'onglet `Profils d'administration` ou `Profils de site`.
3. Sur la ligne du profil à copier, cliquez sur le bouton bleu `Dupliquer`.
4. Dans la fenêtre `DUPLIQUER`, cliquez sur `Oui`.
5. Sur la nouvelle ligne créée dans la liste, cliquez sur le bouton orange `Editer`.
6. Dans le panneau `Profil de droit`, modifiez le champ `Intitulé` et les droits voulus.
7. Cliquez sur `Enregistrer`.

### Supprimer un profil de droits

Dans INGENEO PRECOMPTA, un profil de droits ne peut pas être supprimé tant qu'un utilisateur l'a. Avant la suppression, la colonne `Utilisateurs` du profil doit afficher `0`.

{% hint style="danger" %}
Dans INGENEO PRECOMPTA, la suppression d'un profil de droits est irréversible.
{% endhint %}

1. Dans INGENEO PRECOMPTA, ouvrez `Paramètres > Administration > Profils de droits`.
2. Cliquez sur l'onglet `Profils d'administration` ou `Profils de site`.
3. Sur la ligne du profil, cliquez sur le bouton rouge `Supprimer`.
4. Dans le bandeau `Confirmez-vous la suppression ?`, cliquez sur `Supprimer`.
5. Dans le panneau `Suppression critique`, saisissez l'intitulé du profil dans le champ `Pour confirmer, saisissez « … »`.
6. Dans le champ `Code de sécurité`, saisissez le code de votre application OTP.
7. Cliquez sur `Confirmer la suppression`.

### Attribuer un profil de droits à un utilisateur

1. Dans INGENEO PRECOMPTA, ouvrez `Paramètres > Administration > Utilisateurs`.
2. Sur la ligne de l'utilisateur, cliquez sur le bouton orange d'édition.
3. Pour le profil d'administration, cliquez sur l'onglet `Profil d'administration` et choisissez le profil dans la liste `Profil d'administration`.
4. Pour un profil de site, cliquez sur l'onglet `Profils de site`.
5. Dans le champ `Site`, choisissez le site.
6. Dans la liste `Profil de droit`, choisissez le profil de site.
7. Cliquez sur `Ajouter`.
8. Cliquez sur `Enregistrer` en bas à droite du panneau `Utilisateurs`.

Dans INGENEO PRECOMPTA, un utilisateur qui a un profil de site pour un site reçoit les droits de ce profil sur toutes les entreprises de ce site. Le troisième onglet du panneau `Utilisateurs`, `Profils d'entreprise`, sert à attribuer des droits sur une seule entreprise.

## Résultat attendu

Dans INGENEO PRECOMPTA, le profil créé ou modifié apparaît dans `Paramètres > Administration > Profils de droits`, dans l'onglet de son type. Sa ligne indique son `Libelle`, son `Type` et le nombre d'`Utilisateurs` qui l'ont.

Un utilisateur déjà connecté reçoit ses nouveaux droits après s'être déconnecté puis reconnecté, ou après avoir rechargé la page.

## Erreurs fréquentes

* **Le menu `Paramètres` ou le bouton `Ajouter` des profils de droits n'apparaît pas.** Cause : il manque le droit `Autoriser l'accès à l'administration de la plateforme.` dans le profil d'administration de l'utilisateur. Solution : demandez à un administrateur d'activer ce droit dans `Paramètres > Administration > Profils de droits > Profils d'administration`.
* **Après une modification de son profil de droits, un utilisateur n'a pas ses nouveaux droits dans INGENEO PRECOMPTA.** Cause : la session de l'utilisateur a été ouverte avant l'enregistrement du profil. Solution : l'utilisateur se déconnecte puis se reconnecte, ou recharge la page.
* **La suppression d'un profil de droits est impossible dans INGENEO PRECOMPTA.** Cause : au moins un utilisateur a encore ce profil (colonne `Utilisateurs` supérieure à `0`). Solution : dans `Paramètres > Administration > Utilisateurs`, attribuez un autre profil à chacun de ces utilisateurs, puis relancez la suppression.
* **Un utilisateur ne voit pas un classeur comptable ou ne peut pas agir dessus dans INGENEO PRECOMPTA.** Cause : son profil de site n'accorde pas les droits voulus sur ce type de classeur, ou un profil d'entreprise s'applique à la place du profil de site. Solution : vérifiez l'onglet du type de classeur dans l'étape `Droits sur les classeurs` de son profil de site, puis l'onglet `Profils d'entreprise` de l'utilisateur.
* **Un utilisateur qui a le droit `Autoriser la création d'entreprise.` ne peut pas rattacher l'entreprise créée à un site dans INGENEO PRECOMPTA.** Cause : il n'a aucun profil de site. Solution : attribuez-lui au moins un profil de site dans `Paramètres > Administration > Utilisateurs`.

## Fiches liées

* [Détail des droits](detail-des-droits.md) : liste et effet des droits des profils de droits d'INGENEO PRECOMPTA

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-gerer-profils-droits-ingeneo-precompta
* titre : Comment créer ou modifier un profil de droits dans INGENEO PRECOMPTA ?
* titre\_menu : Créer ou modifier un profil de droits
* type : procedure
* module : Administration
* version\_outil : 2.16.0 (version observée le 2026-11-06)
* roles\_concernes : administrateur
* tags : profil de droits, profil d'administration, profil de site, droits sur les classeurs, notifications, utilisateurs
* formulations\_utilisateur : « comment donner les droits sur le classeur achat à un collaborateur » ; « comment donner accès à un nouveau collaborateur » ; « comment faire pour voir le classeur comptable » ; « comment donner des droits supérieurs ou inférieurs »
* sources : Refonte de la page GitBook ingeneo-pre-compta/administration/gerer-les-profils-de-droits ; observation de l'application 2.16.0 (2026-11-06) ; réponses de l'expert (2026-11-06)
* redacteur : CG
* relecteur :
* derniere\_verification : 2026-11-06
* statut : brouillon

</details>
