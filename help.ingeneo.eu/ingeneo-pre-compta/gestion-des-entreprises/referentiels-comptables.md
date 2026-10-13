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

# Référentiels comptables

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un utilisateur ayant le droit [**Autoriser l’accès au paramétrage de la comptabilité**](../administration/detail-des-droits.md) peut gérer les référentiels comptables.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

Les référentiels comptables constituent la base de données de votre entreprise permettant à INGENEO de proposer des saisies complètes et automatisées adaptées à votre activité.

***

**Quand utiliser cette fonctionnalité :**

* Configuration initiale d'une nouvelle entreprise
* Mise à jour des paramètres comptables en cours d'exercice
* Adaptation aux évolutions réglementaires (TVA, plan comptable)
* Optimisation des automatisations de saisie

**Quand NE PAS modifier les référentiels :**

* En cours de clôture comptable (risque d'incohérence)
* Pour des modifications ponctuelles (utilisez les saisies manuelles)

**Alternatives disponibles :** L'import de votre FEC ou la synchronisation avec certain logiciel comptable permettent de récupérer automatiquement vos référentiels existants.

***

### <sup>**Préparer l'environnement**</sup>

{% hint style="danger" %}
**Impact critique** : Des référentiels mal configurés peuvent compromettre la qualité des automatisations et nécessiter des corrections manuelles importantes sur vos saisies.
{% endhint %}

***

### <sup>**Accéder aux référentiels comptables**</sup>

**Navigation spécifique** : L'accès se fait depuis l'édition de votre entreprise

### <sup>**Paramétrer les référentiels**</sup>

1. Accédez à l’édition de l’entreprise concernée
2. Ouvrez l’onglet **Référentiel comptable**
3. Ajoutez, modifiez ou supprimez les éléments suivants selon vos besoins :
   * **Journaux comptables** : Ajoutez, modifiez ou supprimez vos journaux comptables
   * **Comptes tiers** : Gérez vos clients, fournisseurs et autres tiers (action possible aussi depuis la bannette)
   * **Plan comptable** : Administrez votre plan de comptes personnalisé
   * **Codes de TVA** : Configurez vos taux et règles de TVA (action possible aussi depuis la bannette)
   * **Modes de règlement** : Paramétrez vos moyens de paiement

{% hint style="warning" %}
Affichez et automatisez les éléments comptables dans les paramétrages des [classeurs comptables](classeurs-comptables.md)
{% endhint %}

***

### <sup>**Paramétrer l'analytique**</sup>

* **Axes analytiques**
* **Sections analytiques** (10 niveaux de sections maximum par axe)

{% hint style="warning" %}
Affichez et automatisez l'analytique dans les paramétrages des [classeurs comptables](classeurs-comptables.md)
{% endhint %}

***

### <sup>**Gérer les paramètres bancaires**</sup>

* **Comptes banque** : Ajoutez, modifiez ou supprimez vos éléments de banque
* **Intégration** : Ces paramètres sont utilisés pour vos saisies de banque

***

### <sup>**Questions fréquentes**</sup>

**Vous voulez ajouter des comptes tiers ou codes TVA rapidement ?**

Ces éléments peuvent être créés directement depuis votre saisie sans passer par les référentiels.

***

### <sup>**Avertissement**</sup>

**Cohérence des données** : Toute modification des référentiels doit être cohérente avec vos obligations comptables et fiscales.

**Limitation de synchronisation** : La synchronisation avec les logiciels comptables n'est disponible que si l'interconnexion est techniquement supportée pour votre logiciel spécifique.

### <sup>**Vidéo interactive**</sup> <sup>💡</sup>

{% @arcade/embed url="https://app.arcade.software/share/oDMS1sZpPjnSFvnF01Ha" flowId="oDMS1sZpPjnSFvnF01Ha" %}
