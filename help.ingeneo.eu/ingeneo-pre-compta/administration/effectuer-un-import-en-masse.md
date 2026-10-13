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
  - portail-de-service
---

# Effectuer un import en masse

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un utilisateur avec le droit [**Autoriser l’accès au déploiement en masse**](detail-des-droits.md) peut effectuer des imports en masse d'entreprises.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

L'import en masse permet de créer simultanément plusieurs entreprises sur INGENEO, particulièrement utile lors de migrations ou de déploiements importants.

***

**Quand utiliser cette fonctionnalité :**

* Déploiement initial pour un cabinet avec de nombreux clients
* Création groupée d'entreprises avec des paramètres similaires (utiliser les modèles d’entreprises)
* Intégration de nouveaux portefeuilles clients

***

### <sup>**Préparer l'environnement**</sup>

{% hint style="danger" %}
**Impact critique** : Un fichier mal renseigné peut provoquer l'échec de l'import complet et nécessiter une correction manuelle de chaque entreprise. **Critères obligatoires pour l'import :**
{% endhint %}

* **Fichier Excel conforme** : Utilisez exclusivement le modèle à jour fourni par INGENEO pour éviter les erreurs de format
* **Données complètes** : Vérifiez que tous les champs obligatoires sont renseignés
* **Format standardisé** : Respectez le format des données selon les spécifications du fichier
* **Cohérence des informations** : Contrôlez la validité des SIREN

***

### <sup>**Effectuer l'import en masse**</sup>

1. Depuis votre interface INGENEO
2. Sélectionnez **Déploiement** dans le menu déroulant
3. Sélectionnez **Importer un fichier ZIP**
4. Respectez les prérequis (Le nom de vos fichiers FEC doivent commencer par le numéro SIREN.)

{% hint style="info" %}
**Efficacité** : Cette approche permet d'initialiser un nombre d’entreprises important avec le plan comptable du FEC de l’entreprise ainsi que les occurrences pour proposer des écritures sans avoir fait de saisies préalables sur INGENEO.
{% endhint %}

***

### <sup>**Questions fréquentes**</sup>

**Votre import a échoué partiellement ?**

Consultez le rapport reçu par email pour identifier les entreprises en erreur. Corrigez les données problématiques et relancez l'import uniquement pour les entreprises échouées.

**Vous voulez modifier des entreprises après import ?**

Les entreprises importées peuvent être modifiées individuellement via les paramètres entreprise.

**Votre fichier Excel ne correspond pas au modèle ?**

Téléchargez toujours la dernière version du modèle depuis la plateforme. Les formats peuvent évoluer et l'utilisation d'anciens modèles provoque des erreurs d'import.

***

### <sup>**Avertissement**</sup>

{% hint style="warning" %}
**Limitation de synchronisation** : la disponibilité de la synchronisation automatique dépend de votre logiciel comptable. Tous les logiciels ne proposent pas cette fonctionnalité.
{% endhint %}

{% hint style="warning" %}
**Contrôle post-import** : vérifiez systématiquement le rapport d'import reçu par email et contrôlez manuellement quelques entreprises créées pour valider la cohérence des données importées.
{% endhint %}
