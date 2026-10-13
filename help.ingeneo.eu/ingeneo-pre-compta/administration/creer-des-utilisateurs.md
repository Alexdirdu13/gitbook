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

# Créer des utilisateurs

### <sup>**Prérequis & Permissions**</sup>

**Permissions requises selon le type d'utilisateur :**

{% hint style="success" %}
**Utilisateur interne** : Seul un utilisateur ayant le droit [**Autoriser l’accès à l’administration de la plateforme**](detail-des-droits.md) peut créer un utilisateur interne
{% endhint %}

{% hint style="success" %}
**Utilisateur externe** : Un utilisateur ayant le droit **Autoriser l’accès à l’administration** (profil d'entreprise) peut créer un utilisateur externe.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

La plateforme distingue deux types d'utilisateurs avec des droits différents :

* **Utilisateur interne** : comptable, expert-comptable, personne interne à la structure
* **Utilisateur externe** : personne externe à votre structure (client, commissaire aux comptes...)

Les droits octroyés à chaque utilisateur sont paramétrables par [profils de site ou d’**entreprise**](gerer-les-profils-de-droits.md).

{% hint style="warning" %}
**Limitation importante** : Affectez un profil d'entreprise uniquement si l'utilisateur doit avoir accès à certaines entreprises spécifiques.
{% endhint %}

***

### Vidéo interactive :bulb:

Création utilisateur client :

{% @arcade/embed url="https://app.arcade.software/share/nFE5LGPWOKIUPOcl3O5s" flowId="nFE5LGPWOKIUPOcl3O5s" %}

Création utilisateur collaborateur :

{% @arcade/embed url="https://app.arcade.software/share/HRoqyR4NZW2v9htRUrDM" flowId="HRoqyR4NZW2v9htRUrDM" %}

***

### <sup>**Créer un utilisateur interne**</sup>

1. Cliquez sur le menu **Paramètres**
2. Sélectionnez l'onglet **Administration**
3. Choisissez **Utilisateurs** puis **Général**
4. Cliquez sur **+ Ajouter**
5. Saisissez l'adresse mail du nouvel utilisateur
6. Sélectionnez le **Type interne**
7. Renseignez les informations obligatoires
8. Attribuez le profil souhaité
9. Cliquez sur **Enregistrer**

***

### <sup>**Créer un utilisateur externe**</sup>

1. Cliquez sur le menu **Paramètres**
2. Sélectionnez l'onglet **Administration**
3. Choisissez **Utilisateurs** puis **Général**
4. Cliquez sur **+ Ajouter**
5. Saisissez l'adresse mail du nouvel utilisateur
6. Sélectionnez le **Type externe**
7. Renseignez les informations obligatoires
8. Attribuez le profil souhaité
9. Cliquez sur **Enregistrer**

***

### <sup>**Gestion des utilisateurs**</sup>

* Depuis la page **Utilisateurs**, vous pouvez :
  * Ajouter ou inviter des utilisateurs à un profil
  * Supprimer un utilisateur externe
  * Modifier les droits d'un utilisateur existant (bouton **Éditer**)
  * Supprimer un utilisateur (**Supprimer**)

***

### <sup>**Questions fréquentes**</sup>

**Vous voulez modifier les droits d'un utilisateur existant ?**

Utilisez le bouton **Éditer** à côté de l'utilisateur concerné pour ajuster ses profils de site ou d'entreprise.

**Vous souhaitez supprimer un utilisateur ?**

Utilisez le bouton **Supprimer** disponible dans la liste des utilisateurs. Cette action est irréversible.

**Quelle différence entre les différents profils de site et d’entreprise ?**

* Pour les profils de site : le gestionnaire dispose de plus de droits que le collaborateur sur l’entièreté du site (et donc des entreprises dans ce site).
* Pour les profils d’entreprise : le profil d’entreprise « collaborateur » pourra par défaut accéder à la saisie comptable, le profil d’entreprise « client » ne pourra que déposer et rechercher des documents et n’aura pas la possibilité de faire des saisies comptable.

***

### <sup>**Avertissement**</sup>

{% hint style="warning" %}
**Processus d'activation** : Tout nouvel utilisateur doit créer son mot de passe via le mail d'activation reçu avant de pouvoir accéder à la plateforme.
{% endhint %}

{% hint style="warning" %}
**Gestion des accès entreprise** : Un utilisateur externe peut avoir accès à plusieurs entreprises, mais l'accès doit être configuré individuellement depuis chaque entreprise.
{% endhint %}
