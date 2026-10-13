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

# Paramétrage engagement de dépense

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un utilisateur ayant le droit [**Autoriser l’accès au paramétrage des processus métier**](../../administration/detail-des-droits.md) pourra paramétrer les engagements de dépenses.
{% endhint %}

{% hint style="success" %}
Seul un profil **initiateur** dans un circuit de validation d’engagement de dépenses peut initier un bon de commande.
{% endhint %}

{% hint style="success" %}
**Un classeur de plan de classement** dédié doit obligatoirement être créé en amont.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

L'engagement de dépenses sur INGENEO permet à une structure de prendre formellement la décision de dépenser des fonds pour un achat.

Ce processus se concrétise par l'émission d'un bon de commande et inclut un [circuit de validation](../workflow/circuit-de-validation.md).

***

### Vidéo interactive :bulb:

Création du classeur :

{% @arcade/embed url="https://app.arcade.software/share/IFxgeNSC0o8YJn9Z1JiY" flowId="IFxgeNSC0o8YJn9Z1JiY" %}

Création d'un formulaire :

{% @arcade/embed url="https://app.arcade.software/share/VyLxt0pBx4jSaNiYozcd" flowId="VyLxt0pBx4jSaNiYozcd" %}

Création du circuit de validation :

{% @arcade/embed url="https://app.arcade.software/share/yDulI5LZhyDxCByXg4hn" flowId="yDulI5LZhyDxCByXg4hn" %}

***

Quand utiliser :

* Formaliser vos demandes d'achat
* Respecter les processus de validation interne
* Faciliter le rapprochement facture/bon de commande

**Quand ne pas l'utiliser :**

* Les achats d'urgence nécessitant une validation immédiate

***

### <sup>**Préparer l'environnement**</sup>

{% hint style="warning" %}
Une mauvaise configuration initiale peut bloquer tout le processus de validation.
{% endhint %}

**Éléments obligatoires à configurer :**

* **Classeur de plan de classement** (ex : bon de commande) pour organiser les documents

***

### <sup>**Configurer un engagement de dépense**</sup>

1. Accédez au module **Engagements de dépense**
2. Cliquez sur **Nouveau**
3. Sélectionnez le type d'engagement
4. Renseignez les informations requises (montant, bénéficiaire, etc.)
5. Ajoutez les pièces justificatives si nécessaire
6. Cliquez sur **Enregistrer**

***

### <sup>**Configurer le circuit de validation**</sup>

1. Depuis **Entreprise > Plan de classement > Processus métier**
2. Sélectionnez **Circuit de validation** puis **+ Ajouter**
3. Choisissez le type de circuit **Formulaire**
4. Sélectionnez le type de formulaire **engagement de dépenses**
5. Cliquez sur **Enregistrer**
6. Saisissez un **nom** pour le circuit de validation
7. Sélectionnez le formulaire **engagement de dépenses**
8. Cliquez sur **Enregistrer**
9. Ajoutez les niveaux de validation :
   * **Initiateur** : Toujours au niveau 1
   * **Valideur(s)** : Selon votre organisation
10. Cliquez sur **Enregistrer**

***

### <sup>**Avertissement**</sup>

{% hint style="warning" %}
Seuls les profils initiateurs peuvent créer des engagements de dépenses. Les valideurs sont définis dans le circuit de validation et reçoivent des notifications automatiques.
{% endhint %}

{% hint style="warning" %}
Une fois un engagement soumis, il ne peut être modifié que par les valideurs dans le circuit. Vérifiez toutes les informations avant soumission.
{% endhint %}
