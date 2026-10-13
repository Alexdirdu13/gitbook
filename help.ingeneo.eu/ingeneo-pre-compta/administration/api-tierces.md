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

# API tierces

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un utilisateur ayant le droit [**Autoriser l'accès à la configuration de la plateforme**](detail-des-droits.md) peut créer des clés d'API tierces.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

INGENEO permet de créer des clés d'API tierces pour des intercommunications avec des solutions externes telles que Welyb ou MyCompanyFile.

* Utiliser pour connecter des applications tierces à INGENEO
* Permet l'intercommunication sécurisée avec des plateformes externes
* Contrôle des permissions d'accès

***

### <sup>**Préparer la création**</sup>

**Critères obligatoires :**

* Identifier les besoins d'accès de l'application tierce
* Définir les restrictions d'entreprises si nécessaires

***

### <sup>**Créer la clé API**</sup>

1. Depuis votre compte INGENEO, rendez-vous dans **Paramètres** / **Administration** / **APIs** / **APIs externes**.
2. Cliquez sur **Ajouter**.
3. Saisissez un libellé descriptif pour identifier la clé.
4. Cliquez sur **Enregistrer**.
5. La clé d'API est générée automatiquement, copiez-la.

**Configurer les Permissions de la clé d'API :**

1. Activez les **Autorisations d'accès aux méthodes** nécessaires.
2. Configurez les **Restrictions d'accès aux entreprises** si besoin.

{% hint style="info" %}
Il est possible de régénérer la clé API et de la rendre inactive selon vos besoins.
{% endhint %}

***

### <sup>**Questions fréquentes**</sup>

**Vous souhaitez modifier les permissions d'une clé existante ?**

Rendez-vous dans les **Permissions de la clé d'API** pour ajuster les autorisations d'accès aux méthodes et les restrictions d'entreprises.

**Vous avez perdu votre clé API ?**

Utilisez la fonction de régénération pour créer une nouvelle clé. L'ancienne sera automatiquement invalidée.

**Vous voulez désactiver temporairement une clé ?**

Vous pouvez rendre la clé inactive sans la supprimer, permettant une réactivation ultérieure.

***

### <sup>**Avertissement**</sup>

{% hint style="warning" %}
Des liens vers la documentation **Développeur** et **SSO** sont disponibles dans l'interface pour vous accompagner dans l'intégration.
{% endhint %}
