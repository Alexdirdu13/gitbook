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

# Modèles d'entreprises

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un utilisateur ayant le droit [**Autoriser l’accès au déploiement en masse**](detail-des-droits.md) peut créer et gérer les modèles d'entreprise.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

Les modèles d'entreprises permettent de standardiser la configuration comptable et organisationnelle lors de la création de nouvelles entreprises. Ils regroupent tous les paramètres essentiels : logiciel comptable, classeurs, référentiels, profils d’entreprise, etc.

***

**Quand l'utiliser :**

* Création récurrente d'entreprises avec des configurations similaires
* Standardisation des paramètres comptables par secteur d'activité
* Gain de temps lors des mises en production

**Quand NE PAS l'utiliser :**

* Pour des configurations d'entreprise très spécifiques ou uniques
* Si les paramètres changent fréquemment

***

### <sup>**Préparer l'environnement**</sup>

Préparez les fichiers d'import si nécessaire (plan comptable, FEC)

***

### <sup>**Créer le modèle d'entreprise**</sup>

1. Depuis le **Menu entreprise**
2. Cliquez sur le bouton **Actions multiples** (trois traits verticaux à droite de l’écran)
3. Sélectionnez **Modèles**, puis **Gestion des modèles générique**
4. Dans le menu **Modèles d'entreprise**, cliquez sur **Ajouter**
5. Saisissez un libellé explicite pour votre modèle
6. Complétez les paramètres selon vos besoins (logiciel comptable, profils, classeurs, etc.)
7. Cliquez sur **Enregistrer**

***

### <sup>**Gestion des modèles avancés**</sup>

* Pour créer des modèles de tampon adaptés aux différents classeurs, cliquez sur **Ajouter**
* Pour définir les types de frais standards, cliquez sur **Ajouter** dans **Modèles de nature de frais**

***

### <sup>**Gérer l'activation des modèles**</sup>

Vous pouvez **activer** ou **désactiver** les modèles selon vos besoins :

* Modèles actifs : disponibles lors de la création d'entreprises
* Modèles inactifs : conservés mais non utilisables

***

### <sup>**Questions fréquentes**</sup>

**Vous souhaitez modifier un modèle existant ?**

Accédez à **Menu entreprise** > **Actions multiples** > **Modèles** > **Gestion des modèles générique**, puis sélectionnez le modèle à modifier. Attention aux impacts sur les entreprises déjà créées.

**Vous ne voyez pas les classeurs dans les profils d'entreprise ?**

Vérifiez que vous avez créé les classeurs comptables et de GED avant de configurer les profils d'entreprise. Recréez les profils si nécessaire.

**Vous voulez dupliquer un modèle existant ?**

Depuis la liste des modèles, utilisez la fonction de duplication puis modifiez les paramètres spécifiques au nouveau modèle.

***

### <sup>**Avertissement**</sup>

{% hint style="warning" %}
**Les modèles d'entreprise impactent directement la configuration des nouvelles entreprises créées.**
{% endhint %}

{% hint style="warning" %}
**Testez toujours vos modèles sur un environnement de test avant activation en production.**
{% endhint %}
