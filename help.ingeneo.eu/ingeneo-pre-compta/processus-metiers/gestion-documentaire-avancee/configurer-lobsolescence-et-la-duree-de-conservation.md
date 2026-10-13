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

# Configurer l'Obsolescence et la Durée de conservation

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un utilisateur ayant le droit [**Autoriser l’accès au paramétrage des processus métier**](../../administration/detail-des-droits.md) peut configurer l'Obsolescence & Durée de conservation.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

La configuration de l'obsolescence et de la durée de conservation permet de gérer automatiquement le cycle de vie de vos documents.

***

### <sup>**Préparer l'environnement**</sup>

{% hint style="warning" %}
Une mauvaise configuration peut entraîner la suppression ou l'archivage non désiré de documents importants.
{% endhint %}

**Critères obligatoires :**

* Définissez précisément les durées d'obsolescence selon vos besoins métier
* Choisissez les critères de conservation appropriés pour éviter les pertes de données
* Renseignez-vous sur les durées légales de conservation ou archivage de document (un lien est proposé depuis INGENEO)

***

### <sup>**Configurer l'obsolescence et la conservation**</sup>

{% hint style="info" %}
Les paramètres d'obsolescence et de conservation ne pourront plus être modifiés une fois appliqués aux documents existants.
{% endhint %}

* **Obsolescence** : notifie automatiquement les utilisateurs X jours/mois/années avant l'expiration d'un document.
* **Durée de conservation** : définit l'action à exécuter (suppression ou archivage) X jours/mois/années après une date de référence (date du document ou dépôt du document).

1. Depuis votre compte, rendez-vous dans l'entreprise concernée, menu plan de classement, processus métier.
2. Sélectionnez un classeur
3. Activez l'option **obsolescence** et/ou le paramétrage de conservation des documents
4. **Configuration Obsolescence** : Choisissez une durée en jour, mois ou année
5. **Configuration Durée de conservation** : Choisissez une durée en jour, mois ou année, par rapport à des critères du document et de suppression ou d'archivage du document
6. Cliquez sur **enregistrer**

{% hint style="info" %}
Il est possible de créer plusieurs Obsolescence & Durée de conservation selon vos différents besoins.
{% endhint %}

***

### <sup>**Questions fréquentes**</sup>

**Vous souhaitez modifier une configuration existante ?**

Retournez dans le menu plan de classement, processus métier et modifiez les paramètres du classeur concerné.

**Vous voulez appliquer différentes règles selon le type de document ?**

Créez plusieurs configurations d'Obsolescence & Durée de conservation adaptées à chaque type de document.

**Vous hésitez entre suppression et archivage ?**

L'archivage conserve les documents dans le menu Rechercher, la suppression place le document dans la corbeille. Privilégiez l'archivage si vous pourriez avoir besoin de consulter les documents ultérieurement.

***

### <sup>**Avertissement**</sup>

{% hint style="warning" %}
La configuration de l'obsolescence et de la durée de conservation impact directement la gestion de vos documents.
{% endhint %}

{% hint style="warning" %}
Vérifiez soigneusement vos paramètres avant validation pour éviter toute perte de données non désirée.
{% endhint %}
