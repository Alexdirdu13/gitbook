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

# Classeurs & éléments comptables

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un utilisateur ayant le droit [**Autoriser l’accès au paramétrage de la comptabilité** ](../administration/detail-des-droits.md)peut créer et configurer des classeurs comptables.
{% endhint %}

Il sera nécessaire, un fois le classeur créé, d'attribuer le droit sur ce dernier **Gérer les référentiels associés (ajouter, modifier, supprimer)**

***

### <sup>**Contexte & Recommandations**</sup>

Les paramétrages des classeurs comptables permettent d'activer les éléments comptables dans la fenêtre de saisie, il sera également possible de les rendre obligatoire.

***

### <sup>Les éléments comptables</sup>

| Libellé d'écriture | Numéro de facture          |
| ------------------ | -------------------------- |
| Date de facture    | Date d'échéance            |
| Numéro de pièce    | Mode de règlement          |
| Collectif          | Devise                     |
| Périodicité        | Codes de TVA               |
| Analytique         | Libellé de pièce           |
| Quantité #1 et #2  | Information complémentaire |

{% hint style="info" %}
Créer plusieurs classeurs comptable permet également d’automatiser des éléments comptable pour certains besoins.
{% endhint %}

***

### <sup>Vidéo interactive 💡</sup>

{% @arcade/embed url="https://app.arcade.software/share/ju5pEnAEOySPw1pj9bYh" flowId="ju5pEnAEOySPw1pj9bYh" %}

***

### <sup>**Préparer l'environnement**</sup>

{% hint style="warning" %}
Une mauvaise configuration du classeur peut impacter l'organisation de vos données comptables.
{% endhint %}

**Critères obligatoires :**

* Définir le nom du classeur de manière claire et explicite
* Choisir le type de classeur correspondant à votre usage pour assurer une configuration appropriée
* Vérifier vos permissions d'accès au menu entreprise

***

### <sup>**Créer un classeur comptable**</sup>

{% hint style="info" %}
Le type de classeur ne pourra pas être modifié après création.
{% endhint %}

1. Depuis votre compte, rendez-vous dans le menu **entreprise** – **Classeurs comptables**.
2. Cliquez sur **Ajouter**.
3. Saisissez un nom pour le classeur.
4. Sélectionnez un type de classeur correspondant à votre usage.
5. Cliquez sur **Enregistrer**
6. Dans l'onglet **Configuration** vous pourrez :
   1. Choisir l'ordre d'affichage
   2. Éditer le nom
   3. Choisir un journal par défaut
7. Dans l'onglet [**Éléments comptables**](classeurs-comptables.md#les-elements-comptables) vous pourrez activer ou non les éléments souhaités
8. Cliquez sur **Enregistrer** pour valider vos paramétrages

***

### <sup>**Éditer un classeur comptable**</sup>

{% hint style="info" %}
Éditez un classeur afin d'adapter vos éléments com
{% endhint %}

1. Depuis votre compte, rendez-vous dans le menu **entreprise** – **Classeurs comptables**.
2. Editez un classeur comptable.
3. Assurez vous d'avoir un **journal** par défaut
4. Dans l'onglet **Configuration** vous pourrez :
   1. Choisir l'ordre d'affichage
   2. Éditer le nom
   3. Choisir un journal par défaut
5. Dans l'onglet [**Éléments comptables**](classeurs-comptables.md#les-elements-comptables) vous pourrez activer ou non les éléments souhaités
6. Cliquez sur **Enregistrer** pour valider vos paramétrages

***

### <sup>**Paramétrage avancé**</sup>

* Activer/désactiver la fonction « Ne pas exporter »
* Alerter si la date de facture supérieure à la date d’échéance
* Afficher la validité de l’entreprise
* Afficher les fenêtres d'avertissements lors de la détection d'une incohérence sur les lignes de TVA
* Contrôle IBAN sur les factures
* Afficher la fenêtre d'avertissement lorsque la date de facture n'est pas comprise dans la période d'exercice en cours
* Choix d’un circuit de validation obligatoire pour tous les documents

{% hint style="info" %}
Vérifiez que toutes les configurations correspondent à vos besoins avant validation.
{% endhint %}

***

### <sup>**Questions fréquentes**</sup>

**Vous souhaitez modifier le type de classeur après création ?**

Le type de classeur ne peut pas être modifié après création. Il faut créer un nouveau classeur avec le bon type.

**Vous avez des doublons non repérés dans votre classeur ?**

Vérifiez la configuration du contrôle des doublons dans le menu paramétrage général.

**Vous voulez désactiver une fonction avancée ?**

Rendez-vous dans le menu paramétrage avancé et désactivez les fonctions non désirées.

{% hint style="warning" %}
La configuration des classeurs comptables impacte directement l'organisation de vos données comptables.
{% endhint %}

{% hint style="warning" %}
Assurez-vous de bien définir tous les paramètres avant de commencer à utiliser le classeur.
{% endhint %}
