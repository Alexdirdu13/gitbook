---
description: >-
  Dans INGENEO PRECOMPTA, l'écran Administration > Archivage d'une entreprise
  génère une archive ZIP de ses documents. Le lien de téléchargement est envoyé
  par e-mail et reste valable 7 jours.
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

# Comment générer une archive des documents d'une entreprise dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de générer une archive ZIP des documents d'une entreprise dans INGENEO PRECOMPTA. Le lien de téléchargement est envoyé par e-mail à l'utilisateur qui lance la génération. La génération prend quelques minutes pour 100 Mo de documents. Elle nécessite le droit `Autoriser l'accès à l'administration`.

## Objectif

Dans INGENEO PRECOMPTA, l'écran `Archivage` de l'onglet `Administration` d'une entreprise génère une archive ZIP de ses documents. L'archive contient :

* les documents de tous les classeurs comptables de l'entreprise, enregistrés ou non ;
* les documents du plan de classement de l'entreprise.

L'archive ne contient pas les documents mis à la corbeille, ni les paramétrages de l'entreprise. La génération d'une archive ne supprime aucun document de l'entreprise.

Utilisez cette procédure pour conserver une copie des documents d'une entreprise, en particulier avant de la supprimer.

{% hint style="warning" %}
Dans INGENEO PRECOMPTA, la suppression d'une entreprise (`Administration > Suppression de l'entreprise`) efface définitivement ses paramétrages et ses documents. Générez une archive avant de supprimer l'entreprise. L'archive conserve les documents, mais pas les paramétrages.
{% endhint %}

## Prérequis

* Droit : dans INGENEO PRECOMPTA, la génération d'une archive nécessite seulement le droit `Autoriser l'accès à l'administration`. Ce droit donne accès à l'onglet `Administration` de l'entreprise, dont l'écran `Archivage`. Le détail des droits est dans [Détail des droits](../administration/detail-des-droits.md).
* Adresse e-mail : le lien de téléchargement est envoyé uniquement à l'adresse e-mail du compte utilisateur qui lance la génération. Vérifiez que cette adresse est valide.

## Étapes

1. Dans INGENEO PRECOMPTA, cliquez sur `Entreprises` dans le menu de gauche.
2. Sur l'écran `Entreprises`, sur la ligne de l'entreprise, cliquez sur `Editer` dans la colonne `Actions`.
3. Cliquez sur l'onglet `Administration`.
4. Cliquez sur `Archivage`.
5. Cliquez sur `Générer l'archive`. La fenêtre `Générer l'archive` s'ouvre.
6. Dans la fenêtre `Générer l'archive`, cliquez sur `Générer`.
7. Ouvrez l'e-mail contenant le lien de téléchargement, reçu à l'adresse de votre compte utilisateur.
8. Cliquez sur le lien de l'e-mail pour télécharger l'archive ZIP.

Dans la fenêtre `Générer l'archive`, le bouton `Retour` ferme la fenêtre sans générer d'archive.

## Résultat attendu

Dans INGENEO PRECOMPTA, après le clic sur `Générer` dans la fenêtre `Générer l'archive`, le message suivant s'affiche : `Le lien pour télécharger l'archive vous sera envoyé par e-mail dès qu'il sera disponible.`

L'e-mail arrive quand la génération est terminée, soit quelques minutes pour 100 Mo de documents. Le téléchargement se fait uniquement par le lien de l'e-mail.

Le lien reste valable 7 jours après la génération. Passé ce délai, l'archive est supprimée définitivement. Le lien reste valable pendant ces 7 jours même si l'entreprise est supprimée entre-temps.

Dans le fichier ZIP, les documents sont rangés selon l'arborescence `Classeur > Année de dépôt > ID - [numéro de pièce si existe -] Nom original du fichier`.

## Erreurs fréquentes

**L'e-mail contenant le lien de téléchargement n'arrive pas.** Dans INGENEO PRECOMPTA, le lien est envoyé à l'adresse e-mail du compte utilisateur qui a lancé la génération. Vérifiez dans l'ordre :

1. le dossier spam ou courrier indésirable de la messagerie ;
2. l'adresse e-mail du compte utilisateur avec lequel la génération a été lancée ;
3. les outils de filtrage ou de rétention des e-mails de l'entreprise, par exemple MailInBlack.

Si l'e-mail reste introuvable, relancez la génération depuis `Entreprises > Editer > Administration > Archivage`. Une nouvelle génération est sans risque pour les documents de l'entreprise.

**Le message `Le lien a expiré` s'affiche au clic sur le lien de l'e-mail.** Dans INGENEO PRECOMPTA, le lien de téléchargement d'une archive est valable 7 jours. Passé ce délai, générez une nouvelle archive depuis `Entreprises > Editer > Administration > Archivage`.

**L'écran `Archivage` n'est pas accessible.** Dans INGENEO PRECOMPTA, l'accès à l'écran `Administration > Archivage` d'une entreprise nécessite le droit `Autoriser l'accès à l'administration`. Vérifiez que ce droit figure dans le profil de droits de l'utilisateur.

**Des documents manquent dans l'archive ZIP.** Dans INGENEO PRECOMPTA, l'archive d'une entreprise ne contient pas les documents mis à la corbeille. Ce comportement est normal.

## Fiches liées

* [Détail des droits](../administration/detail-des-droits.md) : droit `Autoriser l'accès à l'administration`, qui donne accès à l'archivage.
* [Créer une entreprise](creer-une-entreprise.md) : création et accès à la fiche d'une entreprise.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-generer-archive-entreprise-ingeneo-precompta
* titre : Comment générer une archive des documents d'une entreprise dans INGENEO PRECOMPTA ?
* titre\_menu : Générer une archive des documents
* type : procedure
* module : Gestion des entreprises
* version\_outil : 2.11.0 (version observée)
* roles\_concernes : utilisateur avec le droit `Autoriser l'accès à l'administration`
* tags : archive, archivage, ZIP, téléchargement, suppression d'entreprise, documents
* formulations\_utilisateur : « Comment récupérer tous les documents d'une entreprise ? » ; « Je n'ai pas reçu le mail pour télécharger l'archive » ; « Le lien de l'archive a expiré » ; « Comment sauvegarder les documents avant de supprimer un dossier ? » ; « Où se trouve l'archivage d'une entreprise ? »
* sources : Refonte de la page GitBook ingeneo-pre-compta/gestion-des-entreprises/generer-une-archive-dentreprise ; démo Arcade « Création archives » (données de la démo) ; observation de l'application INGENEO PRECOMPTA 2.11.0 (2026-10-15) ; page GitBook « Détail des droits » ; réponses de l'expert 2026-10-15
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-15
* statut : brouillon

</details>
