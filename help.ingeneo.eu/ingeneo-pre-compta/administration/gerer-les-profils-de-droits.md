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

# Gérer les profils de droits

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un administrateur ayant accès aux Paramètres peut créer ou modifier des profils de droits d’administration et de sites.
{% endhint %}

**Profil d’administration :** permet l’administration et le paramétrage de la plateforme

**Profil de site** : permet la productivité sur un site

***

### <sup>**Contexte & Recommandations**</sup>

La gestion des profils de droits permet d’attribuer précisément les accès aux fonctionnalités de la plateforme pour différents types d’utilisateurs.

**Quand l'utiliser :** Lors de l’arrivée de nouveaux utilisateurs ou d’un changement de périmètre métier.

**Quand NE PAS l'utiliser :** Si l'utilisateur a uniquement besoin d'un accès temporaire, privilégiez alors un profil existant ou un profil d’entreprise.

***

### <sup>**Préparation**</sup>

**Préparer les profils de droits**

{% hint style="warning" %}
Une mauvaise configuration peut donner des accès non souhaités à des données sensibles.
{% endhint %}

* **Lister les rôles utilisateurs** pour anticiper les besoins d’accès.
* **Définir les périmètres fonctionnels** (ex : saisie comptable, paramétrages).
* **Créer une nomenclature claire des profils** (ex : "Admin Site", "Lecture Comptable").

***

### <sup>**Ajouter ou modifier un profil d'administration**</sup>

1. Dans la section **Profils d’administration**, cliquez sur **Ajouter**
2. Remplissez le champ **Intitulé** du profil
3. Sélectionnez les droits à accorder dans la liste proposée
4. Cliquez sur **Droits sur les classeurs** pour gérer les accès détaillés
5. Définissez les droits sur les classeurs : **Factures d’achats**, **Factures de ventes**, **Caisse**, **Banque**
6. Sélectionnez les droits souhaités pour chaque classeur
7. Cliquez sur **Enregistrer** pour valider

{% hint style="info" %}
Choisissez un intitulé explicite pour retrouver facilement le profil plus tard.
{% endhint %}

### <sup>**Ajouter ou modifier un profil de site**</sup>

1. Dans la section **Profils de site**, cliquez sur **Ajouter**
2. Remplissez le champ **Intitulé** du profil
3. Sélectionnez les droits à accorder dans la liste proposée
4. Cliquez sur **Droits sur les classeurs** pour gérer les accès détaillés
5. Définissez les droits sur les classeurs : **Factures d’achats**, **Factures de ventes**, **Caisse**, **Banque**
6. Sélectionnez les droits souhaités pour chaque classeur
7. Cliquez sur **Enregistrer** pour valider

***

### <sup>**Questions fréquentes**</sup>

**Vous souhaitez restreindre un utilisateur à un seul module ?**

Créez un profil avec uniquement les droits nécessaires, puis assignez-le à l’utilisateur.

**Vous ne voyez pas l’option pour ajouter un profil ?**

Vérifiez que vous êtes connecté en tant qu'administrateur avec les droits sur les paramètres.

***

### <sup>**Avertissement**</sup>

{% hint style="warning" %}
Les profils de droits s’appliquent immédiatement après enregistrement.
{% endhint %}

{% hint style="warning" %}
Évitez d'accorder tous les droits à un profil par défaut : préférez des droits minimums adaptés au poste.
{% endhint %}

{% hint style="warning" %}
Privilégiez une mise à jour régulière des profils pour garantir la sécurité d’accès.
{% endhint %}
