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

# Paramétrage connecteur marchand

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un utilisateur ayant le droit [**Autoriser l’accès au paramétrage de la collecte**](../administration/detail-des-droits.md) peut créer un canal de collecte connecteur marchand.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

{% hint style="info" %}
Le connecteur marchand permet la récupération automatique de factures depuis les espaces clients fournisseur (aussi appelé "web scraping").
{% endhint %}

**Limitations :**

* Nécessite les identifiants de connexion
* Demande parfois une double authentification

***

### <sup>**Préparer l'environnement**</sup>

**Assurez-vous d'avoir les identifiants Dropbox avant de commencer la configuration. Sans ces informations, vous devrez faire une demande au propriétaire du compte.** **Critères obligatoires :**

* Utilisateur destinataire créé dans la plateforme
* Classeur de destination défini pour organiser les documents reçus

***

### <sup>**Créer un canal de collecte connecteur marchand**</sup>

1. Accédez au menu **Collecte** puis cliquez sur **+ Ajouter**
2. Sélectionnez **Connecteur marchand** comme type de canal
3. Saisissez un libellé
4. Choisissez le classeur de dépôt
5. Cliquez sur **POWENS** ou **envoyez la demande à un utilisateur**
6. Choisissez un fournisseur parmi la liste proposée
7. Saisissez les identifiants

***

**Gestion des collectes :**

La collecte automatique s'effectue **une fois par jour**.

**Consulter l'historique :**

Menu **Collecte > Historique** pour visualiser toutes les collectes effectuées

***

### <sup>**Questions fréquentes**</sup>

**Le fournisseur n'apparaît pas dans la liste POWENS ?**

Vérifiez que l'établissement est compatible avec le service POWENS ou contactez le support technique.

**L'utilisateur ne reçoit pas le mail d'invitation ?**

Vérifiez l'adresse mail renseignée dans son profil et consultez le dossier spam.
