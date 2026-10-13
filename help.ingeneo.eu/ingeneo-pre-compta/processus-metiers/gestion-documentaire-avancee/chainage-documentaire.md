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

# Chaînage documentaire

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Un utilisateur ayant le droit [**Autoriser l’accès au paramétrage des processus métier**](../../administration/detail-des-droits.md) peut configurer le chaînage documentaire.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

Le chaînage documentaire vous permet de rapprocher automatiquement deux documents, comme une facture et son bon de commande.

**Quand l'utiliser :**

* Pour automatiser le rapprochement facture bon de commande
* Contrôler des divergences de montants
* Pour réduire les erreurs de saisie manuelle

***

### <sup>**Préparer l'environnement**</sup>

{% hint style="info" %}
Assurez-vous d'avoir correctement configuré vos classeurs avant de procéder au chaînage
{% endhint %}

**Critères obligatoires :**

* Disposer des droits pour créer des classeurs
* Avoir identifié les types de documents à chaîner
* Connaître la structure des numéros de commande à reconnaître

***

### Vidéo interactive :bulb:

Paramétrage :

{% @arcade/embed url="https://app.arcade.software/share/auFxRu9jM50djA93UQ25" flowId="auFxRu9jM50djA93UQ25" %}

Rapprochement :

{% @arcade/embed url="https://app.arcade.software/share/dYhtZeHon6LGY9xlNwPj" flowId="dYhtZeHon6LGY9xlNwPj" %}

***

### <sup>**Créer un classeur de plan de classement**</sup>

{% hint style="warning" %}
Cette étape est indispensable avant toute configuration de chaînage
{% endhint %}

1. Depuis votre compte, rendez-vous dans **Entreprises**, puis dans l'édition de l'entreprise concernée.
2. Sélectionnez **Plan de classement**, puis cliquez sur le bouton **+ Ajouter** pour créer un nouveau classeur.
3. Renseignez le nom du classeur (exemple : Bon de commande) et ajoutez la liste des types de documents se trouvant dans le classeur (en utilisant le +).
4. Configurez les options qui vous intéressent, puis enregistrez votre classeur.

{% hint style="warning" %}
Votre bon de commande doit être présent dans le classeur de plan de classement avant traitement
{% endhint %}

***

### <sup>**Traitement du bon de commande**</sup>

1. Déposez votre bon de commande dans le classeur de plan de classement.
2. Entrez dans la visualisation du document.
3. Renseignez les éléments nécessaires ainsi que le compte tiers.
4. Le numéro de commande et le montant TTC seront automatiquement reconnus.
5. Ajoutez un commentaire si nécessaire avant enregistrement.

***

### <sup>**Traitement de la facture**</sup>

1. Ouvrez la facture concernée depuis le **classeur comptable**.
2. La plateforme confirme ou non si la somme totale des bons de commande correspond au montant de la facture.
3. Cliquez sur l'icône en forme d'œil pour visualiser le bon de commande rapproché automatiquement.

***

### <sup>**Questions fréquentes**</sup>

**Vous souhaitez modifier un chaînage existant ?**

Rendez-vous dans **Processus métier** > **Chaînage documentaire**, sélectionnez le chaînage à modifier et apportez vos changements.

**Vous rencontrez des erreurs de reconnaissance automatique ?**

Vérifiez la configuration de votre masque de reconnaissance et assurez-vous que la structure définie correspond bien au format de vos documents.

**Vous voulez supprimer un chaînage ?**

Depuis la liste des chaînages documentaires, sélectionnez le chaînage concerné et utilisez la fonction de suppression.
