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

# Valider un document

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un utilisateur avec un rôle de **valideur** dans un [circuit de validation](../processus-metiers/workflow/circuit-de-validation.md) peut valider des documents.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

La validation de documents dans un circuit permet de s'assurer qu'un processus d'approbation structuré est respecté avant la finalisation d'un document.

**Quand l'utiliser :** Lorsque vous êtes désigné comme valideur dans un circuit et qu'un document attend votre validation

**Quand NE PAS l'utiliser :** Si vous n'avez pas les permissions de validation ou si le document ne vous est pas assigné

**Alternatives disponibles :** Contacter l'administrateur pour obtenir les droits de validation si nécessaire

***

### <sup>Vidéo interactive 💡</sup>

{% @arcade/embed url="https://app.arcade.software/share/6OOceuIhp3mZr2ioeA49" flowId="6OOceuIhp3mZr2ioeA49" %}

### <sup>**Valider un document**</sup>

1. Accédez au menu **tableau de bord** ou **actions / notifications**
2. Sélectionnez le document à valider
3. Cliquez sur **valider** ou **refuser** le document

{% hint style="info" %}
L'action choisie changera le niveau et le statut du document dans le circuit de validation. Une notification est donnée à l'utilisateur suivant dans le circuit de validation.
{% endhint %}

{% hint style="warning" %}
Tout refus obligera l’utilisateur à renseigner un commentaire.
{% endhint %}

***

### <sup>**Questions fréquentes**</sup>

**Vous ne voyez pas le document à valider ?**

Vérifiez que vous avez bien les permissions de valideur et que le document vous est assigné à cette étape du circuit.

**Vous souhaitez valider plusieurs documents en même temps ?**

Chaque document doit être validé individuellement depuis la liste des documents en attente.
