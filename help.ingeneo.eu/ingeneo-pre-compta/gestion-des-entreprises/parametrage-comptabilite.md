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

# Paramétrage comptabilité

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un utilisateur avec le droit [**Autoriser l’accès au paramétrage de la comptabilité**](../administration/detail-des-droits.md) peut configurer les informations comptables.
{% endhint %}

Ces configurations impactent directement les automatisations de vos saisies comptables.

***

**Quand utiliser cette configuration :**

* Configuration initiale après [création d'entreprise](creer-une-entreprise.md)
* Changement de logiciel comptable ou mise à jour majeure
* Modification du régime fiscal ou du type de comptabilité
* Optimisation des automatisations de saisie

**Quand NE PAS modifier ces paramètres :**

* En cours d'exercice sans validation préalable de l'expert-comptable
* Pendant les périodes de clôture ou déclarations fiscales

***

### <sup>**Préparer l'environnement**</sup>

{% hint style="danger" %}
**Impact critique** : Une mauvaise configuration peut compromettre l’export vers le logiciel comptable
{% endhint %}

**Critères obligatoires avant configuration :**

* **Code dossier identique** : Le code dossier INGENEO doit correspondre exactement à celui de votre logiciel comptable pour permettre l’export ou la synchronisation si le logiciel comptable le permet, pour certains logiciels comptables un menu déroulant sera proposé
* **Informations logiciel à jour** : Vérifiez la version et les paramètres de votre logiciel comptable avant configuration

***

### <sup>**Configurer les paramètres comptables**</sup>

1. Accédez au menu **Paramètres** de l'entreprise
2. Sélectionnez **Comptabilité**
3. Renseignez les champs obligatoires selon votre organisation (code dossier, plan comptable, etc.)
4. Configurez la politique de création automatique de compte tiers :
   * **Préfixe** : Définissez un préfixe (exemple : F pour fournisseurs)
   * **Mode d'auto-complétions** : Intitulé INSEE ou incrémentation numérique
   * **Longueur des comptes** : Spécifiez le nombre de caractères si le choix d’une incrémentation est fait
5. Paramétrez le plan comptable : possibilité de paramétrer les longueurs minimums et maximums et automatiser l’ajout de « 0 » pour atteindre la taille définie
6. Définissez les éléments à exporter en comptabilité (tampons, notes, surlignages)
7. Activez ou non l’ajout d’un deuxième compte de TVA identique, et la saisie à 0€ selon vos besoins

***

### <sup>**Questions fréquentes**</sup>

**Votre synchronisation échoue systématiquement ?**

Vérifiez que le **code dossier** est rigoureusement identique (attention aux espaces et caractères spéciaux), vérifiez les paramétrages de votre logiciel comptable.

**Vous voulez automatiser la création des comptes tiers ?**

Configurez la **politique de création des comptes fournisseurs** avec un préfixe cohérent et une longueur standardisée pour votre organisation.

**Vos périodes d'exercice se chevauchent de manière problématique ?**

Clôturez l'ancienne période avant d'ouvrir la troisième. INGENEO ne permet que deux périodes simultanées maximum.
