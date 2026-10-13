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

# Paramétrage POWENS

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Un utilisateur ayant le droit [**Autoriser l’accès au paramétrage de la comptabilité**](../../administration/detail-des-droits.md) peut configurer la connexion bancaire POWENS.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

POWENS permet la récupération automatique de mouvements bancaires.

**Limitations :**

* Nécessite les identifiants de connexion bancaire
* Demande une double authentification
* Tous les établissements bancaires ne sont pas compatibles
* Requiert l'accord explicite du détenteur du compte

***

### <sup>Vidéo interactive 💡</sup>

{% @arcade/embed url="https://app.arcade.software/share/wCQUeyBSdNjxFGKdkzda" flowId="wCQUeyBSdNjxFGKdkzda" %}

***

### <sup>**Ajouter une banque au référentiel**</sup>

**Cette étape doit être réalisée avant toute tentative de connexion**

1. Depuis votre compte **INGENEO**, rendez-vous dans le menu d’édition de l’**entreprise**.
2. Dans l'onglet **Entreprise**, sélectionnez **Référentiel comptable**
3. Cliquez sur **Banque**
4. Cliquez sur **+ Ajouter**
5. Saisissez le **Nom de la banque** dans le champ prévu
6. Cliquez sur **Enregistrer**

***

### <sup>**Configurer la récupération automatique**</sup>

{% hint style="info" %}
Deux méthodes sont disponibles selon que vous disposez ou non des identifiants bancaires.
{% endhint %}

#### **Option 1 : Vous avez les identifiants bancaires**

1. Depuis la fiche banque, cliquez sur **Connecter POWENS**
2. Saisissez les identifiants bancaires
3. Suivez les indications sur la page de connexion de la banque
4. Suivez le processus d’identification

#### **Option 2 : Vous n'avez pas les identifiants**

1. Cliquez sur l'icône **Gérer la récupération automatique**
2. Cliquez sur **Envoyer la requête de connexion à un utilisateur**
3. Recherchez et sélectionnez l'utilisateur détenteur du compte bancaire
4. Cliquez sur l'icône de la ligne utilisateur

**L'utilisateur recevra un mail d'invitation à se connecter à la plateforme. Il devra ensuite :**

* Se connecter à INGENEO
* Consulter ses notifications (icône cloche)
* Cliquer sur l'œil pour voir la demande
* Cliquer sur **POWENS**
* Sélectionner sa banque et saisir ses identifiants

***

### <sup>**Questions fréquentes**</sup>

**La banque n'apparaît pas dans la liste POWENS ?**

Vérifiez que l'établissement bancaire est compatible avec le service POWENS ou contactez le support technique.

**L'utilisateur ne reçoit pas le mail d'invitation ?**

Vérifiez l'adresse mail renseignée dans son profil et consultez le dossier spam.

***

### <sup>**Avertissement**</sup>

{% hint style="warning" %}
La connexion POWENS nécessite la transmission d'identifiants bancaires sensibles. Assurez-vous du consentement explicite de votre client et respectez les obligations RGPD en matière de protection des données financières.
{% endhint %}

{% hint style="warning" %}
La récupération des mouvements débutera 48-72 heures après la connexion.
{% endhint %}
