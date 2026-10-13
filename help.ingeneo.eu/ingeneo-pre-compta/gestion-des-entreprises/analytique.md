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

# Analytique

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
✍️ Seuls les utilisateurs ayant le droit [**Autoriser l’accès au paramétrage de la comptabilité**](../administration/detail-des-droits.md) peuvent effectuer cette opération.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

L’analytique permet de ventiler des écritures comptables selon des axes analytiques définis. Cette configuration est utile pour suivre des budgets, projets ou centres de coûts.

***

### Vidéo interactive :bulb:

{% @arcade/embed flowId="y88T2WqDzHlwcEPmJzP3" url="https://app.arcade.software/share/y88T2WqDzHlwcEPmJzP3" %}

{% @arcade/embed flowId="oWmgW7kNYFL36UCFhx7v" url="https://app.arcade.software/share/oWmgW7kNYFL36UCFhx7v" %}

***

### <sup>**Préparer l’environnement**</sup>

{% hint style="warning" %}
⚠️ Sans activation de l’analytique dans les classeurs, aucune ventilation analytique ne sera proposée lors des saisies comptables.
{% endhint %}

### <sup>**Critères obligatoires :**</sup>

* Avoir défini les axes et sections nécessaires selon votre organisation interne
* Vérifier que le logiciel comptable permet l’intégration des lignes analytiques

***

### <sup>**Créer un plan analytique**</sup>

{% hint style="warning" %}
⚠️ Toute création de **Section** analytique nécessite un **Axe** analytique, si le logiciel comptable ne dispose pas d’axe analytique, il faudra créer un **axe par défaut**.
{% endhint %}

Depuis le menu principal, procédez comme suit :

1. Rendez-vous dans Entreprise > Référentiels comptables > Analytiques.
2. Cliquez sur **+ Ajouter** pour créer un axe.
3. Renseignez le champ **Code**.
4. Renseignez le champ **Intitulé**.
5. Cliquez sur **Enregistrer**.
6. Cliquez ensuite sur **Sections analytiques**.
7. Cliquez sur **+ Ajouter** pour créer une section.
8. Sélectionnez l’axe créé.
9. Renseignez les champs **code** et **intitulé**.
10. Cliquez sur **Enregistrer**.

✍️ Vous pouvez synchroniser votre plan comptable s’il est compatible en cliquant sur le bouton **Synchroniser**.

***

### <sup>**Activer l’analytique dans vos classeurs**</sup>

{% hint style="warning" %}
⚠️ L’analytique ne sera pas proposé à la saisie tant qu’il n’est pas activé sur chaque classeur concerné.
{% endhint %}

Pour chaque classeur concerné :

1. Rendez-vous dans Entreprise > Classeurs comptables.
2. Cliquez sur le classeur souhaité pour l’éditer.
3. Cliquez sur **éléments comptables**.
4. Cochez la case **Analytiques**.
5. Sélectionnez un **axe par défaut** si nécessaire.
6. Cliquez sur **Enregistrer**.

✍️ L’axe par défaut peut être modifié à tout moment selon les besoins.

***

### <sup>**Questions fréquentes**</sup>

#### **Vous ne voyez pas d’axe disponible dans un classeur ?**

Assurez-vous qu’au moins un axe a bien été créé dans le menu Analytiques.

#### **Vous souhaitez modifier une section existante ?**

Rendez-vous dans Entreprise > Référentiels comptables > Analytiques > Sections analytiques, puis cliquez sur l’icône d’édition à côté de la section concernée.

#### **Vous ne souhaitez plus utiliser l’analytique ?**

Décochez simplement l’option **Analytiques** dans l’édition du classeur concerné.

***

**Avertissement**

{% hint style="danger" %}
⚠️ L’activation de l’analytique modifie les options de saisie comptable. Toute modification en cours d’exercice peut avoir des conséquences sur la cohérence de vos suivis analytiques.
{% endhint %}
