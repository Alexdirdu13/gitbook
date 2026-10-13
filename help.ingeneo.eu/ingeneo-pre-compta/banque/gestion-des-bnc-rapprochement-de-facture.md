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

# Gestion des BNC - Rapprochement de facture

## 1 – Paramétrage du type de comptabilité

INGENEO vous permet de définir le type de comptabilité de votre entreprise : **comptabilité d'engagement** ou **comptabilité de trésorerie**.

Dans le paramétrage de l'entreprise concernée, rendez-vous dans **Comptabilité**, **Paramétrage général** et choisissez le type de comptabilité souhaité.

{% hint style="info" %}
Lorsque le type « Comptabilité de trésorerie » est sélectionné, la saisie n'est alors plus disponible dans votre classeur d'achat.
{% endhint %}

{% @arcade/embed flowId="e79LbAz94dvvxNKfGypP" url="https://app.arcade.software/share/e79LbAz94dvvxNKfGypP" %}

La collecte de la banque peut se réaliser par plusieurs canaux de collecte :

* Redirection des mouvements bancaires issus de votre compte **jedéclare.com** ;
* Connexion via **Powens** ;&#x20;
* Dépôt de fichiers bancaires aux formats CFONB, OFX, QIF ;

Une documentation dédiée à chaque canal est disponible dans le **centre d'aide**.&#x20;

***

## 2 – Rapprochement documentaire

Pour une comptabilité de trésorerie, l'enregistrement de la saisie passera par le classeur de banque, il faut donc un rapprochement documentaire en amont de la comptabilisation

{% hint style="warning" %}
**Attention** : une fois le document rapproché au mouvement, celui-ci est retiré du classeur d'achats, même s'il n'a pas encore été exporté.&#x20;
{% endhint %}

{% @arcade/embed flowId="eBGOj6sbwq4HEBGWy3Ve" url="https://app.arcade.software/share/eBGOj6sbwq4HEBGWy3Ve" %}

### 2.1 Suggestion automatique

La suggestion automatique peut s'effectuer jusqu'à la somme de 3 mouvements correspondant à un montant total d'une facture, et inversement.

Dans votre classeur de banque, cliquez sur le bouton de **rapprochement de facture**.

Le bouton de rapprochement utilise les codes couleur et repères visuels suivants :

* **Jaune** : indique le nombre de factures suggérées par la plateforme.
* **Orange** : indique le nombre de factures rapprochées mais le montant total n'est pas égal à celui du mouvement.
* **Vert** : indique le nombre de factures rapprochées, le montant total est égal à celui du mouvement.

Le compteur se met à jour automatiquement en fonction du montant de la ou des factures rapprochées.

### 2.2 Rapprochement manuel

Si aucune suggestion automatique n'est proposée, vous avez la possibilité de **visualiser l'ensemble des factures**.\
Sélectionnez ensuite le ou les documents à rapprocher, comme indiqué précédemment.

{% hint style="warning" %}
**Attention** : pour être visible, la date de la facture doit toujours être inférieure à celle du mouvement.&#x20;

Si votre compte fournisseur est reconnu par la plateforme vous avez la possibilité de l'utiliser comme filtre de recherche.
{% endhint %}

L'ensemble des mouvements après validation (manuelle, semi-automatique ou automatique) seront transférés en comptabilité avec le ou les justificatifs associés.

Vous pourrez également retrouver le mouvement et sa facture dans votre menu **Rechercher**.
