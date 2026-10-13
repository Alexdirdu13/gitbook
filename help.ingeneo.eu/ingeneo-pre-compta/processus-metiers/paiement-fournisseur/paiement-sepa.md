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

# Paiement SEPA

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Un utilisateur interne ayant un rôle de collaborateur / gestionnaire ou administrateur peut configurer le paiement SEPA et les droits associés.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

Le paiement par virement SEPA est un moyen de paiement sécurisé qui permet au titulaire d'un compte de transférer des fonds vers un autre compte, en France et dans l'ensemble des pays de l'espace SEPA.

Les droits des utilisateurs (**profils de site** ou d’**entreprise**) sont scindés en 2 : la **mise au paiement** et le **paiement**. Ces deux droits peuvent être donnés à un même utilisateur ou à des utilisateurs différents.

***

**Quand l'utiliser :**

* Pour les paiements fournisseurs sécurisés
* Pour les virements dans l'espace SEPA
* Pour payer plusieurs factures via un seul fichier SEPA

***

### <sup>**Préparer l'environnement**</sup>

**Critère obligatoire :**

* Entreprise avec numéro SIREN valide (obligatoire pour le paramétrage)

***

### <sup>**Paramétrer les classeurs**</sup>

{% hint style="warning" %}
Cette configuration détermine qui peut mettre au paiement et qui peut effectuer les paiements. Une mauvaise attribution des droits peut créer des risques de sécurité.
{% endhint %}

1. Depuis votre compte, rendez-vous dans le menu **Entreprise**.
2. Cliquez sur **Entreprise**, puis éditez l'entreprise où activer le paiement fournisseur.
3. Cliquez sur **Administration**, puis sur **Profils d'entreprise**.
4. Sélectionnez ou créez un profil avec les droits nécessaires.
5. Attribuez les droits de **mise au paiement** et/ou de **paiement** selon les besoins.

***

### <sup>**Générer un fichier SEPA**</sup>

1. Accédez au menu **Paiements**.
2. Filtrez si nécessaire par **Statut** ou par **mode de paiement**.
3. Pour une facture : sélectionnez la facture et cliquez sur **Générer le fichier SEPA**.
4. Pour plusieurs factures : faites un clic droit sur les factures sélectionnées, puis choisissez **Générer le fichier SEPA**.
5. Cliquez sur **Générer le fichier SEPA**.

{% hint style="info" %}
Un fichier nommé "sepa-facture.xml" ou "sepa-multifactures.xml" sera enregistré dans votre répertoire de téléchargement. Ce fichier devra être importé ou transféré à votre banque pour effectuer le paiement.
{% endhint %}

***

### <sup>**Questions fréquentes**</sup>

**Vous souhaitez séparer les droits de mise au paiement et de paiement ?**

Créez deux profils d'entreprise distincts : un avec le droit "Mettre les factures au paiement" et un autre avec "Payer les factures au paiement", puis affectez les utilisateurs selon leurs responsabilités.

**Vous ne pouvez pas configurer le paiement SEPA ?**

Vérifiez que votre entreprise dispose d'un numéro SIREN valide, condition obligatoire pour accéder au paramétrage.

**Vous voulez gérer les droits au niveau des sites ?**

Accédez aux profils de sites depuis le menu **Paramètres** > **Profils de droits** > **Profils de sites** avec un profil administrateur.

***

### <sup>**Avertissement**</sup>

{% hint style="warning" %}
La configuration des droits de paiement doit être effectuée avec précaution. Assurez-vous que seuls les utilisateurs autorisés ont accès aux fonctionnalités de paiement pour maintenir la sécurité financière de votre organisation.
{% endhint %}
