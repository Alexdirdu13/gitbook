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

# Engager une dépense

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un profil **initiateur** dans un [circuit de validation](../workflow/circuit-de-validation.md) d’engagement de dépenses peut initier un bon de commande.
{% endhint %}

***

### <sup>**Vidéo interactive**</sup> :bulb:

Saisir une dépense :

{% @arcade/embed url="https://app.arcade.software/share/uZ9fIQVmtfjSlUYz4Z2m" flowId="uZ9fIQVmtfjSlUYz4Z2m" %}

Valider un engagement de dépense :

{% @arcade/embed url="https://app.arcade.software/share/WwEGzzPsb9VA55bIod27" flowId="WwEGzzPsb9VA55bIod27" %}

### <sup>**Créer un engagement de dépenses**</sup>

{% hint style="info" %}
Vérifiez que le budget est suffisant avant de soumettre.
{% endhint %}

Procédez comme suit :

1. Depuis votre **Bannette** > **Formulaire** ou **Tableau de bord** > **Mes engagements de dépenses**.
2. Cliquez sur **+ Ajouter**
3. Complétez les informations générales (titre, fournisseur, dates, etc.)
4. Créez un nouveau contact fournisseur si nécessaire
5. Accédez à l'onglet **Commande**
6. Ajoutez les articles :
   * Utilisez **+ Ajouter** pour les articles existants
   * Utilisez **Annuaire des articles** pour créer de nouveaux articles
7. Définissez les quantités et ajoutez des commentaires si nécessaire
8. Joignez les pièces justificatives si nécessaire
9. Vérifiez l'état du budget avec le curseur visuel
10. Cliquez sur **Enregistrer et soumettre**

Le bon de commande est maintenant visible dans vos engagements avec son statut de validation.

{% hint style="info" %}
Vous pouvez créer les articles à la volée dans le tableau de la commande.
{% endhint %}

***

### <sup>**Valider ou refuser un engagement**</sup>

{% hint style="info" %}
Une validation fait passer l'engagement au niveau suivant et ne peut être annulée par l’initiateur.
{% endhint %}

Procédez comme suit :

1. Depuis **Bannette** > **Action / Notifications** ou **Tableau de bord** > **Engagements en attente**
2. Le valideur sélectionne l'engagement à traiter
3. Choisissez l'action :
   * **Valider** : Envoie au niveau suivant ou termine le processus
   * **Refuser** : Renvoie au niveau précédent (obligation de renseigner un commentaire)
   * **Modifier** : Permet les corrections avant validation
4. Consultez l'historique si nécessaire

{% hint style="info" %}
Les documents validés sont consultables dans le menu [**Rechercher**](../../gestion-des-documents/rechercher-un-document.md).
{% endhint %}

***

### <sup>**Questions fréquentes**</sup>

**Vous voulez modifier un engagement en cours de validation ?**

Seul le valideur actuel peut modifier l'engagement via l'option **Modifier l'engagement**.

**Vous ne trouvez plus votre engagement validé ?**

Les engagements terminés sont accessibles via le menu **Rechercher**.

**Vous souhaitez suivre l'avancement d'un engagement ?**

Consultez l'historique de validation disponible dans le détail de chaque engagement.

***

### <sup>**Avertissement**</sup>

{% hint style="warning" %}
Seuls les profils initiateurs peuvent créer des engagements de dépenses. Les valideurs sont définis dans le circuit de validation et reçoivent des notifications automatiques.
{% endhint %}

{% hint style="warning" %}
Une fois un engagement soumis, il ne peut être modifié que par les valideurs dans le circuit. Vérifiez toutes les informations avant soumission.
{% endhint %}
