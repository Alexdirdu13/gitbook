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

# La saisie comptable

### <sup>**Prérequis & Permissions**</sup>

{% hint style="success" %}
Seul un utilisateur ayant le droit [Enregistrer les documents](../administration/detail-des-droits.md) peut effectuer la saisie comptable des documents.
{% endhint %}

***

### <sup>**Contexte & Recommandations**</sup>

La saisie comptable permet de traiter les documents présents dans les bannettes en leur attribuant les comptes et [éléments comptables](../gestion-des-entreprises/classeurs-comptables.md) appropriés.

Une fois la saisie faite, le document est exporté vers le logiciel comptable de façon automatique (à l’exception des exports « ON DEMAND »).

***

### <sup>**Préparer la saisie**</sup>

{% hint style="info" %}
Assurez-vous d'avoir sélectionné la bonne entreprise avant de commencer la saisie pour éviter les erreurs de comptabilisation.
{% endhint %}

**Critères obligatoires :**

* Avoir les droits d’accès à la saisie de l'entreprise concernée
* Connaître le plan comptable de l'entreprise pour une saisie précise
* Vérifier que les documents sont bien présents dans la bannette sélectionnée

***

### <sup>**Accéder à la saisie comptable**</sup>

Cliquer sur **Bannettes**, puis sélectionner l'entreprise concernée. Sélectionner ou rechercher le classeur de dépôt souhaité, puis cliquer sur la loupe en bout de ligne du document à saisir. Une fenêtre à 3 volets redimensionnables s'ouvre :

* Liste des documents présents dans la bannette
* Volet de saisie comptable du document
* Aperçu du document avec historique et notes

{% hint style="info" %}
Vous pouvez sélectionner un autre document de la bannette directement depuis cette interface.
{% endhint %}

***

### <sup>**Saisir les éléments comptables**</sup>

La plupart des éléments comptables seront renseignés grâce à l'analyse OCR. Par défaut les dates de facture et d'échéance, ainsi que le numéro de facture seront affichés.

Les paramétrages de vos [classeurs & référentiels](../gestion-des-entreprises/referentiels-comptables.md) vous permettrons d'afficher et de renseigner d'autres éléments comptables.

***

### <sup>**Saisir les comptes comptables**</sup>

**Compte tiers :**

Si le [compte tiers](../gestion-des-entreprises/referentiels-comptables.md) est présent dans le FEC, celui-ci peut être renseigné automatiquement si la plateforme a reconnu le fournisseur dans le document. Dans le cas où aucun compte tiers n'est pas renseigné, cliquer dans le champ **Compte** sur une ligne à renseigner :

* **Option 1 - Recherche par nom :** Saisissez les premières lettres du nom du compte tiers, puis sélectionnez le compte souhaité dans la liste qui s'affiche.
* **Option 2 - Recherche par libellé :** Saisissez les premières lettres du libellé du compte tiers, puis sélectionnez le compte souhaité dans la liste qui s'affiche.
* **Option 3 - Fenêtre de recherche :** tapez sur la touche **Entrée** de votre clavier pour ouvrir la fenêtre de recherche des comptes tiers, puis sélectionnez le compte souhaité et validez avec **Sélectionner**.
* **Option 4 - Création de compte tiers :**
  1. Saisissez le code du compte tiers, puis tapez sur la touche **Entrée** de votre clavier pour ouvrir la fenêtre de création de compte tiers
  2. Renseignez les différents champs pour la création du compte tiers
  3. Cliquez sur **Entreprise** pour compléter les informations du compte tiers
  4. Cliquez sur **Options avancées** pour sélectionner les différentes options proposées
  5. Cliquez sur **Masque de saisie** pour compléter les informations du compte tiers
  6. Cliquez sur **Enregistrer** en bas de la page. Seuls les **code** et **intitulé** du tiers sont obligatoires à la création, le tiers sera créé en comptabilité à l’intégration de l’écriture

### <sup>**Vidéo interactive**</sup> <sup>💡</sup>

{% @arcade/embed url="https://app.arcade.software/share/QKoNFPdDXr9oqr8YKxXU" flowId="QKoNFPdDXr9oqr8YKxXU" %}

### <sup>**Comptes de charges**</sup>

Saisissez les premières lettres ou chiffres des comptes ou un mot du libellé dans les champs des comptes de charges. Cliquez sur l'icône **plus** pour ajouter une ligne et sur l'icône **corbeille** pour supprimer une ligne.

### <sup>**Comptes de TVA**</sup>

Saisissez les premières lettres ou chiffres des comptes ou un mot du libellé dans les champs des comptes de TVA. Cliquez sur l'icône **plus** pour ajouter une ligne et sur l'icône **corbeille** pour supprimer une ligne. Cliquez sur **Enregistrer** pour valider la saisie.

{% hint style="success" %}
Une fois enregistré, le document est exporté et n'est plus visible dans la bannette.
{% endhint %}

***

### <sup>**Questions fréquentes**</sup>

**Vous ne trouvez plus votre document après saisie ?** Le document saisi est exporté et n'apparaît plus dans la bannette. Utilisez le menu **Rechercher** pour retrouver le document.

**Vous avez des informations importantes à vérifier ?** Consultez la zone **Vigilances** qui indique des informations importantes sur le document et sa saisie.

***

### <sup>**Avertissement**</sup>

{% hint style="warning" %}
Une fois la saisie enregistrée, le document passe en export et disparaît de la bannette. Vérifiez bien vos saisies avant de valider.
{% endhint %}

{% hint style="warning" %}
Consultez toujours la zone **Vigilances** pour vous assurer qu'aucune information importante n'a été omise lors de la saisie.
{% endhint %}
