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

# Générer une archive d'entreprise

{% hint style="info" %}
Seul l'utilisateur ayant accès à l'édition de l'entreprise peut générer une archive.
{% endhint %}

## Contexte / recommandation

Cette fonctionnalité permet de générer une archive depuis la fiche d'une entreprise.

* Quand l'utiliser\
  Pour créer une archive d'une entreprise depuis son espace d'administration.
* Quand NE PAS l'utiliser\
  Si vous n'avez pas accès au menu d'édition de l'entreprise.

### <sup>Vidéo interactive 💡</sup>

{% @arcade/embed flowId="fCLLxYD1QKWTJpBu5tpN" url="https://app.arcade.software/share/fCLLxYD1QKWTJpBu5tpN" %}

### Préparer l'accès à l'entreprise

{% hint style="warning" %}
L'archive ne peut être générée que depuis le menu d'administration de l'entreprise.
{% endhint %}

Critères obligatoires :

* Accéder au **menu entreprise** pour sélectionner l'entreprise concernée.
* Avoir accès à l'option **Éditer l'entreprise** pour ouvrir ses paramètres.
* Disposer du menu **Archivage** dans l'administration de l'entreprise.

## Action principale

### Générer une archive

{% hint style="warning" %}
Le lien de téléchargement n'est pas immédiat : il est envoyé par e-mail.
{% endhint %}

Depuis votre compte, rendez-vous dans **menu entreprise**.

{% stepper %}
{% step %}
### Ouvrir l'édition de l'entreprise
{% endstep %}

{% step %}
### Accéder à l'administration
{% endstep %}

{% step %}
### Ouvrir Archivage
{% endstep %}

{% step %}
### Lancer la génération

Cliquez sur **générer l'archive**, puis sur **générer**.
{% endstep %}

{% step %}
### Récupérer l'archive

Un lien de téléchargement de l'archive est envoyé à l'adresse e-mail de l'utilisateur ayant fait la demande.

Le téléchargement s'effectue uniquement via le lien reçu par e-mail.
{% endstep %}
{% endstepper %}

## Questions fréquentes

<details>

<summary>Vous ne recevez pas l'e-mail de téléchargement ?</summary>

Vérifiez que l'adresse e-mail de l'utilisateur ayant fait la demande est valide et surveillez votre boîte de réception.

</details>

## Avertissements finaux

{% hint style="warning" %}
* Le lien de téléchargement est envoyé uniquement à l'utilisateur ayant généré l'archive.
* L'archive doit être générée depuis le menu **Archivage** de l'administration de l'entreprise.
{% endhint %}
