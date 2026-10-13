---
hidden: true
---

# Validation automatique et semi automatique

### <sup>**Prérequis & Permissions**</sup>

{% hint style="warning" %}
Seul utilisateur ayant le droit **Autoriser l'accès au paramétrage de la comptabilité** peut configurer les modes de validation.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

La validation automatique permet de valider les documents sans intervention utilisateur, la validation semi-automatique nécessite une confirmation manuelle des écritures proposées par le système.

**Validation automatique - Quand l'utiliser :**

* Pour des fournisseurs récurrents avec des écritures standardisées
* Quand les critères de reconnaissance sont fiables à 100%
* Pour automatiser le traitement de gros volumes

**Validation semi-automatique - Quand l'utiliser :**

* Pour maintenir un contrôle sur les écritures proposées
* Avec des fournisseurs occasionnels ou variables
* Pour valider les propositions avant traitement définitif

**Quand NE PAS utiliser la validation automatique :**

* Avec des documents complexes nécessitant une analyse manuelle
* Pour des comptes sensibles nécessitant une validation humaine

***

### <sup>**Préparer la configuration**</sup>

{% hint style="warning" %}
La configuration s'applique par compte tiers : un mauvais paramétrage peut entraîner des validations non souhaitées
{% endhint %}

#### **Critères obligatoires :**

* Entreprise sélectionnée avec accès aux référentiels comptables
* Comptes tiers identifiés et paramétrés correctement
* Critères de validation définis et testés au préalable

***

### <sup>**Configurer depuis le menu Entreprise**</sup>

{% hint style="success" %}
Cette méthode permet de configurer un ou plusieurs comptes simultanément
{% endhint %}

1. Depuis le menu **Entreprise**, sélectionnez l'entreprise concernée.
2. Cliquez sur **éditer l'entreprise**
3. Accédez à l'onglet **Référentiels comptables**
4. Cliquez sur **Comptabilité**
5. Sélectionnez **Comptes tiers**

#### **Configurer un compte spécifique**

1. Sur la ligne du compte concerné, cliquez sur **éditer**
2. Cliquez sur **Options avancées**
3. Sélectionnez la méthode de validation souhaitée
4. Cliquez sur **Enregistrer**

#### **Configurer tous les comptes simultanément**

1. Cliquez sur **Tout sélectionner**
2. Effectuez un clic droit sur n'importe quelle ligne de compte
3. Sélectionnez **Validation automatique/semi-automatique**
4. Cochez la méthode de validation souhaitée
5. Enregistrez votre choix

{% hint style="warning" %}
Cette méthode applique la même configuration à tous les comptes tiers de l'entreprise.
{% endhint %}

***

### <sup>**Configurer depuis les Bannettes**</sup>

{% hint style="success" %}
Méthode rapide pour configurer un compte directement depuis la saisie
{% endhint %}

1. Depuis le menu **Bannettes**, sélectionnez l'entreprise concernée.
2. Cliquez sur la loupe au niveau du document concerné
3. Sur le formulaire de saisie, cliquez sur la première ligne
4. Tapez le raccourci clavier <kbd>**CTRL+Q**</kbd> pour ouvrir **éditer votre compte tiers**
5. Cliquez sur **Options avancées**
6. Sélectionnez la méthode de validation souhaitée
7. Cliquez sur **Enregistrer**

{% hint style="success" %}
Le raccourci CTRL+Q permet un accès rapide aux paramètres du compte tiers depuis la saisie.
{% endhint %}

***

### <sup>**Lancer la validation semi automatique**</sup>

1. Dans votre menu **Bannette** cliquez sur le bouton **Validation semi-automatique** pour lancer le mécanisme.
2. Une fenêtre s'ouvrira vous indiquant :
   * Les documents exportés avec succès
   * Les documents non exportés
   * Les raisons qui ont empêché la validation semi-automatique

Vous avez également la possibilité de récupérer le **Rapport d'automatisation** en cliquant sur le menu d'action diverse (trois traits horizontaux) sur la droite de l'écran.

***

### <sup>**La validation automatique**</sup>

{% hint style="success" %}
Si vous avez paramétré en **Validation automatique** les fournisseurs, aucune action n'est à mener, le document déposé dans la bannette est lu et directement envoyé en comptabilité.
{% endhint %}

***

### **Questions fréquentes**

**Vous souhaitez appliquer la même validation à tous vos fournisseurs ?**&#x20;

Utilisez la méthode de configuration en lot depuis **Entreprise** > **Référentiels comptables** avec **Tout sélectionner**.

**Vous voulez tester avant d'activer la validation automatique ?**&#x20;

Commencez par la validation semi-automatique pour vérifier les propositions du système avant de passer en mode entièrement automatique.

**Vous rencontrez des erreurs de validation automatique ?**&#x20;

Vérifiez les critères définis pour le compte tiers et repassez temporairement en validation semi-automatique pour identifier les problèmes.

***

### **Avertissement**

{% hint style="warning" %}
Validation automatique : Les documents seront validés sans contrôle manuel. Assurez-vous que les critères de reconnaissance sont fiables avant activation.
{% endhint %}

{% hint style="warning" %}
Configuration en lot : L'application de paramètres à tous les comptes tiers peut impacter l'ensemble de votre processus de validation. Testez d'abord sur quelques comptes.
{% endhint %}
