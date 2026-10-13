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
  - ingeneo
---

# Paramétrage DematBox

## Prérequis / Permissions

{% hint style="info" %}
Seul un utilisateur ayant le droit « Autoriser l'accès au paramétrage de la collecte » peut créer un canal de collecte DématBox.
{% endhint %}

## Contexte / Recommandations

La DématBox permet de réceptionner des documents via un appareil SAGEMCOM dédié à une entreprise et un classeur défini. Ce canal permet uniquement le dépôt de document (canal unidirectionnel), il n'est pas possible d'échanger via celui-ci.

Quand l'utiliser :

* Pour automatiser la collecte de documents depuis un scanner SAGEMCOM
* Pour centraliser les dépôts de documents d'une entreprise spécifique

Limitations :

* Canal unidirectionnel (dépôt uniquement)
* Nécessite un appareil SAGEMCOM compatible
* Requiert la création d'un compte sur https://connect.dematbox.com/

## Préparer l'environnement

{% hint style="warning" %}
Une mauvaise configuration du canal peut empêcher la réception des documents. Assurez-vous d'avoir les bonnes permissions avant de commencer.
{% endhint %}

Critères obligatoires :

* Accès au menu Entreprise dans INGENEO pour créer le canal
* Appareil SAGEMCOM configuré et opérationnel
* Compte créé sur https://connect.dematbox.com/
* Jeton d'appairage récupéré depuis INGENEO

## Créer le canal de collecte Démat'Box

{% hint style="warning" %}
Le jeton d'appairage est unique et nécessaire pour connecter l'appareil SAGEMCOM. Ne le partagez pas.
{% endhint %}

Depuis votre compte INGENEO, rendez-vous dans le menu Entreprise :

* Sélectionner l'entreprise pour laquelle créer le canal
* Cliquer sur Collecte, puis sur Ajouter
* Dans le menu déroulant Type, sélectionner Dématbox
* Saisir un libellé pour identifier le canal
* Configurer les paramétrages automatiques si souhaité :
  * Rotation automatique des documents
  * Détection de page blanche
  * Découpe automatique
* Cliquer sur Enregistrer
* Copier le jeton d'appairage généré

✍️ Le jeton d'appairage sera nécessaire pour configurer le compte Démat'Box.

## Configurer le compte Démat'Box

{% hint style="warning" %}
Le Token INGENEO doit être saisi exactement tel que copié depuis INGENEO.
{% endhint %}

Depuis un navigateur Web, rendez-vous sur https://connect.dematbox.com/

### Création de modèle

* Se connecter ou créer un compte
* Aller dans le menu Mes modèles de dossiers
* Cliquer sur Créer un nouveau modèle
* Cliquer sur DEMAT'LINK
* Cliquer sur NEOExpert
* Valider le Pop-up par OK
* Cliquer sur la Flèche à côté de Modifier
* Sélectionner Modifier le modèle dans le menu déroulant

✍️ Configuration des alertes mail :

* Alerte client sur l'absence de dépôt de pièces (erreur de réception)
* Accusé de réception pour les documents scannés
* Accusé de réception pour les pièces collectées

### Ajout de classeurs de dépôt

* Cliquer sur Ajouter un service pour créer des classeurs supplémentaires
* Cliquer sur Paramètres pour chaque ligne à configurer

### Création de dossier

* Cliquer sur créer un nouveau dossier
* Sélectionner A partir d'un modèle
* Coller le Jeton d'appairage dans le champ Token INGENEO
* Cliquer sur Importer
* Vérifier que les informations remontent correctement :
  * Code cabinet
  * Cabinet
  * Dossier comptable
  * Clé d'API
* Cliquer sur Valider les informations
* Valider le Pop-up en cliquant sur Continuer

## Associer l'appareil SAGEMCOM

{% hint style="warning" %}
L'appairage doit être effectué dans l'ordre exact des étapes pour fonctionner.
{% endhint %}

* Depuis le menu Mes dossiers, cliquer sur Visualiser
* Sélectionner Associer Démat'Box dans le menu déroulant
* Sur l'appareil SAGEMCOM, appuyer simultanément sur les trois touches en face
* Suivre les instructions de l'appareil jusqu'à l'apparition du code d'appairage à l'écran
* Saisir le code d'appairage dans le site Démat'Box
* Cliquer sur Valider les modifications

✍️ L'entreprise et les classeurs de dépôt apparaissent maintenant sur l'écran de l'appareil SAGEMCOM.

## Utilisation

Une fois configuré, scanner un document depuis l'appareil SAGEMCOM. Le document sera automatiquement :

* Déposé dans la bannette de l'entreprise
* Traité par l'OCRLAD
* Envoyé par mail selon la configuration des alertes

## Questions fréquentes

<details>

<summary>Vous souhaitez ajouter des classeurs de dépôt supplémentaires ?</summary>

Depuis Mes modèles de dossiers, modifier le modèle existant et cliquer sur Ajouter un service.

</details>

<details>

<summary>Vous rencontrez des erreurs de réception ?</summary>

Vérifiez la configuration des alertes mail dans le modèle de dossier et consultez la documentation SAGEMCOM.

</details>

<details>

<summary>Vous voulez modifier les paramètres automatiques ?</summary>

Retournez dans INGENEO > Entreprise > Collecte et modifiez les paramètres du canal Démat'Box.

</details>

## Avertissement

{% hint style="danger" %}
En cas de message d'erreur sur l'appareil SAGEMCOM, consultez la documentation SAGEMCOM ou contactez le support Démat'Box : support.dematbox@plustek.fr
{% endhint %}
