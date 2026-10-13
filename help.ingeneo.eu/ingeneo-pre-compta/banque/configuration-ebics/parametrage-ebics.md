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

# Paramétrage EBICS

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un utilisateur interne ayant le droit [**Autoriser l’accès au paramétrage de la comptabilité**](../../administration/detail-des-droits.md) peut configurer un dépôt EBICS.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

Le paramétrage EBICS permet de configurer l’entreprise pour l'import de mouvements bancaires au format EBICS (cfonb ou OFX). Cette configuration lie un IBAN à l'entreprise et peut fonctionner en mode multi-entreprise.

***

### <sup>**Préparer l'environnement**</sup>

{% hint style="info" %}
Assurez-vous d'avoir les informations bancaires correctes avant de commencer. Une mauvaise configuration peut empêcher l'import des données.
{% endhint %}

**Critères obligatoires :**

* IBAN valide du compte bancaire
* BIC/SWIFT si disponible
* Classeur de banque créé

***

### <sup>Vidéo interactive 💡</sup>

{% @arcade/embed url="https://app.arcade.software/share/0MUKXJNUTLrF7wOJ4gvc" flowId="0MUKXJNUTLrF7wOJ4gvc" %}

***

### <sup>**Créer la banque**</sup>

{% hint style="info" %}
Le nom de la banque n'impacte pas l'import.
{% endhint %}

1. Depuis votre compte, rendez-vous dans l’édition de l’**entreprise**.
2. Cliquez sur **Banque**
3. Puis sur **+ Ajouter**
4. Saisissez le nom de la banque et cliquez sur **Enregistrer**

{% hint style="info" %}
Le BIC/SWIFT peut être ajouté lors de cette étape si vous le possédez.
{% endhint %}

***

### <sup>**Ajouter le compte bancaire**</sup>

{% hint style="warning" %}
L'IBAN doit être valide et correspondre exactement au compte bancaire concerné.
{% endhint %}

1. Cliquez sur **+** pour ajouter un compte à la banque créée, puis renseignez les informations suivantes :
   * Libellé du compte
   * Libellé personnalisé
   * Classeur de rattachement
   * IBAN complet
2. Cliquez sur **Enregistrer** pour finaliser la configuration

{% hint style="info" %}
La plateforme liera automatiquement cet IBAN à l'entreprise pour permettre les dépôts EBICS multi-entreprise.
{% endhint %}

***

### <sup>**Questions fréquentes**</sup>

**Vous souhaitez modifier un IBAN déjà configuré ?**

Accédez au menu **Entreprise > Banque**, sélectionnez le compte concerné et modifiez les informations nécessaires.

**Vous rencontrez une erreur lors de la validation de l'IBAN ?**

Vérifiez que l'IBAN est complet (27 caractères pour la France) et ne contient pas d'espaces.

**Vous voulez supprimer une banque ?**

Assurez-vous qu'aucun compte n'y est rattaché avant de procéder à la suppression.
