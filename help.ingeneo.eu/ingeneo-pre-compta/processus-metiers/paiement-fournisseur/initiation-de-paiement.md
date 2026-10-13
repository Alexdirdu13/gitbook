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

# Initiation de paiement

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un utilisateur avec le droit [**Mettre les factures au paiement**](../../administration/detail-des-droits.md) pourra initier un paiement.
{% endhint %}

{% hint style="success" %}
Seul un utilisateur avec le droit **Payer les factures au paiement** pourra initier un paiement.
{% endhint %}

{% hint style="success" %}
Seul un utilisateur avec le droit **Autoriser l’accès au paramétrage des processus métier** pourra configurer le paiement.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

Le paiement fournisseur permet d'automatiser le processus de validation et de règlement des factures directement depuis l'application. Cette fonctionnalité est adaptée aux entreprises ayant un [circuit de validation](../workflow/circuit-de-validation.md) structuré.

***

### <sup>**Vidéo interactive**</sup> :bulb:

Le paramétrage :

{% @arcade/embed url="https://app.arcade.software/share/ehoDQ1g59CRi3bFRcrlr" flowId="ehoDQ1g59CRi3bFRcrlr" %}

Edition du mode de paiement :

{% @arcade/embed url="https://app.arcade.software/share/9jHQs0sygZANQ7ZhVBI0" flowId="9jHQs0sygZANQ7ZhVBI0" %}

La mise au paiement :

{% @arcade/embed url="https://app.arcade.software/share/k9z0fwQF8aT9J3SrcFqS" flowId="k9z0fwQF8aT9J3SrcFqS" %}

Le paiement :

{% @arcade/embed url="https://app.arcade.software/share/Ed8W38ftSyveLJWKp2YI" flowId="Ed8W38ftSyveLJWKp2YI" %}

### <sup>**Préparer l'environnement**</sup>

{% hint style="warning" %}
Une mauvaise configuration des droits peut bloquer le processus de paiement ou donner des accès non autorisés.
{% endhint %}

**Critères obligatoires avant de commencer :**

* Entreprise avec numéro SIREN valide
* Compte tiers avec IBAN et BIC valide

***

### <sup>**Configurer le processus métier**</sup>

1. Depuis le **plan de classement** de l’**entreprise**
2. Sélectionnez **Processus métier**
3. Cliquez sur **Paiement fournisseurs**
4. Puis **+ Ajouter**
5. Sélectionnez un ou plusieurs classeurs
6. Renseignez **Initiation** de paiement

***

### <sup>**Mettre une facture au paiement**</sup>

1. Sélectionnez le document à mettre au paiement
2. Cliquez sur **Mettre au paiement**
3. Renseignez le champ de date de paiement souhaité
4. Cliquez sur **Enregistrer**

***

### <sup>**Effectuer le paiement**</sup>

1. Depuis le menu **Bannette** de l’entreprise ou la **cloche de notification**
2. Consultez vos **Actions / Notifications**
3. Cliquez sur l'icône **Œil** du document
4. Cliquez sur **Payer** pour valider le paiement
5. Une fenêtre s’ouvre pour effectuer un **paiement via Powens**
6. Suivez les instructions de **Powens** pour finaliser le paiement

***

### <sup>**Questions fréquentes**</sup>

**Vous souhaitez séparer les droits de mise au paiement et de paiement ?**

Créez deux profils d'entreprise distincts : un avec le droit "Mettre les factures au paiement" et un autre avec "Payer les factures au paiement". Affectez ensuite les utilisateurs appropriés à chaque profil.

**Vous ne voyez pas les notifications de paiement ?**

Vérifiez que votre profil utilisateur dispose des droits appropriés.

**Vous voulez configurer les droits au niveau des sites ?**

Rendez-vous dans **Paramètres**, puis **Profils de droits** et **Profils de sites** pour une configuration plus granulaire avec un profil administrateur.
