---
description: >-
  Dans INGENEO PRECOMPTA, le menu Référentiels comptables > Comptabilité d'une
  entreprise gère ses journaux, comptes tiers, plan comptable, codes TVA et
  modes de règlement.
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

# Comment gérer les référentiels comptables d'une entreprise dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de créer, modifier, importer, synchroniser et supprimer les journaux, comptes tiers, comptes du plan comptable, codes TVA et modes de règlement d'une entreprise dans INGENEO PRECOMPTA, depuis `Entreprises > Editer > Entreprise > Référentiels comptables > Comptabilité`. Sa durée dépend de l'utilisateur qui fait l'action et du réseau. Elle nécessite le droit `Autoriser l'accès au paramétrage de la comptabilité`.

## Objectif

Dans INGENEO PRECOMPTA, les référentiels comptables sont la base de données comptable d'une entreprise. INGENEO PRECOMPTA s'en sert pour proposer des pré-saisies comptables complètes et automatisées, adaptées à l'activité de l'entreprise.

Le sous-menu `Comptabilité` du menu `Référentiels comptables` d'une entreprise contient cinq onglets :

* `Journaux` : journaux comptables (colonnes `Code`, `Intitulé`, `Type`, `Contrepartie`, `Actions`).
* `Comptes tiers` : comptes clients et fournisseurs (colonnes `Compte`, `Intitulé`, `Collectif`, `Type`, `Mode Règlement`, `Journal`, `Actif`, `Valid. auto.`, `Actions`).
* `Plan comptable` : comptes généraux (colonnes `Compte`, `Intitulé`, `Code TVA`, `Actions`).
* `Codes TVA` : taux et comptes de TVA (colonnes `Code`, `Intitulé`, `Taux`, `Compte déductible`, `Compte collecté`, `Compte immobilisation`, `Auto liquidation`, `Actions`).
* `Modes de règlement` : moyens de paiement (colonnes `Code`, `Intitulé`, `Actions`).

Utilisez cette procédure dans les cas suivants :

* configuration initiale d'une nouvelle entreprise ;
* mise à jour des référentiels comptables en cours d'exercice ;
* adaptation aux évolutions réglementaires (TVA, plan comptable) ;
* optimisation des automatisations de la pré-saisie comptable.

Dans INGENEO PRECOMPTA, ne modifiez pas les référentiels comptables d'une entreprise dans deux cas :

* pendant une clôture comptable, à cause du risque d'incohérence ;
* pour une correction ponctuelle : corrigez l'écriture dans l'écran de pré-saisie comptable du menu `Bannettes`, sans changer le référentiel comptable.

Le menu `Référentiels comptables` contient aussi les sous-menus `Analytiques`, `Banque` et `Structuration`. L'analytique est décrite dans [Paramétrer et saisir l'analytique](analytique.md). La banque est décrite dans [Connecter un compte bancaire avec Powens](../banque/connecteurs-tiers/parametrage-powens.md).

## Prérequis

* Droit : dans INGENEO PRECOMPTA, l'utilisateur doit avoir le droit `Autoriser l'accès au paramétrage de la comptabilité` pour gérer les référentiels comptables du sous-menu `Comptabilité`. Aucun droit par classeur n'est nécessaire. Le détail des droits est dans [Détail des droits](../administration/detail-des-droits.md).
* Synchronisation : dans INGENEO PRECOMPTA, le bouton `Synchroniser` n'apparaît que si le logiciel comptable de l'entreprise permet la synchronisation. Le logiciel comptable se choisit dans `Entreprises > Editer > Entreprise > Comptabilité > Paramétrage général`, décrit dans [Paramétrage général de la comptabilité](parametrage-comptabilite.md).
* Import FEC : préparez le fichier FEC de l'entreprise si vous voulez importer ses référentiels comptables.

{% hint style="warning" %}
Dans INGENEO PRECOMPTA, des référentiels comptables mal configurés dégradent les automatisations de la pré-saisie comptable. Ils peuvent imposer de nombreuses corrections manuelles des écritures. Toute modification des référentiels comptables doit rester cohérente avec les obligations comptables et fiscales de l'entreprise.
{% endhint %}

## Étapes

### Ouvrir les référentiels comptables de l'entreprise

1. Dans INGENEO PRECOMPTA, cliquez sur `Entreprises` dans le menu de gauche.
2. Sur l'écran `Entreprises`, sur la ligne de l'entreprise, cliquez sur `Editer`.
3. Dans l'onglet `Entreprise`, cliquez sur `Référentiels comptables`.
4. Cliquez sur le sous-menu `Comptabilité`.

L'onglet `Journaux` s'affiche. Les boutons `Synchroniser`, `Importer un FEC`, `Intégrer plan comptable générique` et `Réinitialiser l'apprentissage` sont en haut de l'écran.

### Synchroniser les référentiels comptables avec le logiciel comptable

Dans INGENEO PRECOMPTA, le bouton `Synchroniser` de `Référentiels comptables > Comptabilité` récupère les référentiels comptables depuis le logiciel comptable de l'entreprise. La synchronisation ajoute les éléments manquants et met à jour les éléments existants. Les éléments présents seulement dans INGENEO PRECOMPTA sont conservés.

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Comptabilité`.
2. Cliquez sur `Synchroniser`.

La synchronisation se lance sans fenêtre de confirmation. Le bouton `Synchroniser` est absent si le logiciel comptable de l'entreprise ne permet pas la synchronisation.

### Importer les référentiels comptables depuis un FEC

Dans INGENEO PRECOMPTA, le bouton `Importer un FEC` de `Référentiels comptables > Comptabilité` crée les référentiels comptables à partir d'un fichier FEC. L'import ajoute les éléments manquants et met à jour les éléments existants. Les éléments absents du FEC sont conservés.

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Comptabilité`.
2. Cliquez sur `Importer un FEC`.
3. Sélectionnez `Depuis un nouveau fichier` pour importer un nouveau fichier FEC, ou `Depuis un fichier déjà importé` pour réutiliser le FEC importé à la création de l'entreprise.
4. Si vous avez choisi `Depuis un nouveau fichier`, sélectionnez le fichier FEC sur votre ordinateur.

### Intégrer le plan comptable général français

Dans INGENEO PRECOMPTA, le bouton `Intégrer plan comptable générique` de `Référentiels comptables > Comptabilité` ajoute les comptes du plan comptable général français dans l'onglet `Plan comptable`. Il n'ajoute ni journaux, ni codes TVA, ni modes de règlement.

L'intégration est impossible si l'entreprise contient déjà des comptes tiers ou des comptes du plan comptable. Le message `La présence de comptes tiers ou de comptes de plan comptable empêche l'intégration d'un plan comptable générique.` s'affiche alors.

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Comptabilité`.
2. Vérifiez que les onglets `Comptes tiers` et `Plan comptable` sont vides.
3. Cliquez sur `Intégrer plan comptable générique`.

### Réinitialiser l'apprentissage

{% hint style="danger" %}
Dans INGENEO PRECOMPTA, `Réinitialiser l'apprentissage` est irréversible. Le bouton supprime les occurrences apprises pour l'entreprise, issues des FEC et des pré-saisies comptables enregistrées. Après la réinitialisation, les propositions de pré-saisie comptable ne s'appuient plus sur cet historique.
{% endhint %}

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Comptabilité`.
2. Cliquez sur `Réinitialiser l'apprentissage`.

### Ajouter un élément de référentiel comptable

Dans INGENEO PRECOMPTA, chaque onglet de `Référentiels comptables > Comptabilité` a un bouton `Ajouter`. Ce bouton ouvre un panneau de création propre à l'onglet. Les champs marqués d'un astérisque sont obligatoires.

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Comptabilité`.
2. Cliquez sur l'onglet voulu : `Journaux`, `Comptes tiers`, `Plan comptable`, `Codes TVA` ou `Modes de règlement`.
3. Cliquez sur `Ajouter`.
4. Renseignez les champs du panneau de création.
5. Cliquez sur `Enregistrer`, en bas du panneau.

Champs des panneaux de création de `Référentiels comptables > Comptabilité` :

| Onglet               | Panneau                                                               | Champs                                                                                                                |
| -------------------- | --------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------- |
| `Journaux`           | `Créer votre journal`, bloc `PARAMÉTRAGE D'UN JOURNAL`                | `Code`\*, `Intitulé`\*, `Type`\* (`ACHAT`, `AUTRE`, `BANQUE`, `VENTE`), `Contrepartie`                                |
| `Plan comptable`     | `Créer un compte général`, bloc `PARAMÉTRAGE DU COMPTE`               | `Compte`\*, `Intitulé`\*, `Type`\* (`PLAN COMPTABLE`), `Code TVA`                                                     |
| `Codes TVA`          | `Créer un code TVA`, bloc `PARAMÉTRAGE DU CODE TVA`                   | `Code`\*, `Taux`\*, `Intitulé`\*, `Compte déductible`, `Compte collecté`, `Compte immobilisation`, `Auto-liquidation` |
| `Modes de règlement` | `Créer un mode de règlement`, bloc `PARAMÉTRAGE DU MODE DE RÈGLEMENT` | `Code`\*, `Intitulé`\*                                                                                                |

Dans INGENEO PRECOMPTA, le panneau `Créer votre compte tiers` de l'onglet `Comptes tiers` a trois étapes : `Compte tiers`, `Entreprise` et `Options avancées`. `Type`, `Compte` et `Intitulé` sont marqués obligatoires. Le champ `Type` propose `CLIENT` et `FOURNISSEUR`. Les règles de `Comptabilité > Paramétrage avancé` peuvent rendre d'autres champs obligatoires, comme décrit dans [Paramétrage avancé de la comptabilité](parametrage-comptabilite-avance.md). Le panneau contient les blocs et champs suivants :

* `COMPTABILITÉ` : `Type`, `Compte`, `Intitulé`, `Compte collectif`, `Mode de règlement`, `Journal`.
* `MODALITÉS D'ÉCHÉANCES` : `Détection de la date d'échéance sur la facture`, `Calcul des modalités d'échéances`, `Nombre de jour`, `Fin de mois`, `Paiement le`.
* `DEVISES` : `Code ISO`, `Gestion du taux` (`Automatique` ou `Fixe`).
* `OUTILS IA` : `Mode de reconnaissance (comptabilisation par ligne d'article)` (`Classique` ou `Par ligne d'article`), `Regrouper les lignes d'article de faible montant`, `Montant en dessous duquel les lignes sont regroupées`.
* `Information sur l'entreprise` : `Localisation` (`FRANCE`, `UE`, `AUTRES`), `Ville`, `Pays`, `SIREN`, `SIRET`, `DUNS`, `TVA Intracom`, `Forme juridique`, `Raison sociale`, `Date de création`.
* `Banque` : `Nom banque`, `IBAN`, `BIC`.
* `Options sur le compte tiers` : `Non assujetti à la TVA.`, `Pas de numéro de facture.`, `Pas de date d'échéance.`, `Ne pas proposer de comptes comptables en imputations dans la saisie malgré l'apprentissage.`, `Ne pas proposer d'analytiques dans la saisie malgré l'apprentissage.`, `Désactiver le contrôle de l'IBAN.`, `Désactiver le contrôle de la validité de l'entreprise.`, `Actif`.
* `Validation automatique` : `Méthode de validation automatique` (`Désactivé`, `Semi-automatique`, `Automatique`), `Valider uniquement les factures dont le montant est inférieur à : (laisser vide si aucune restriction)`, `Compte d'attente en cas de non-reconnaissance de la contrepartie`, `Circuit de validation`.
* `Conformité Facturation Électronique` : `Type de fournisseur` (`Non défini`, `Privé`, `Public`), `Type de client` (`Non défini`, `Privé`, `Public`, `Particulier`, `Non assujetti (Association)`), `Identifiant légal`.

### Créer un compte tiers ou un code TVA depuis l'écran de pré-saisie comptable

Dans INGENEO PRECOMPTA, un compte tiers ou un code TVA peut aussi être créé depuis l'écran de pré-saisie comptable du menu `Bannettes`, sans ouvrir `Référentiels comptables`.

1. Dans l'écran de pré-saisie comptable, saisissez un code inexistant dans le champ `Compte` (compte tiers) ou dans la colonne `Code TVA` d'une ligne d'écriture (code TVA).
2. Appuyez sur la touche `Entrée` du clavier.
3. Dans le panneau de création qui s'ouvre, renseignez les champs.
4. Cliquez sur `Enregistrer`.

La création d'un compte tiers depuis l'écran de pré-saisie comptable est détaillée dans [Faire la pré-saisie comptable](../gestion-des-documents/la-saisie-comptable.md).

### Modifier un élément de référentiel comptable

Dans INGENEO PRECOMPTA, le crayon de la colonne `Actions` d'un onglet de `Référentiels comptables > Comptabilité` ouvre le même panneau que `Ajouter`, avec les mêmes champs. Le `Code` ou le `Compte` reste modifiable après la création.

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Comptabilité`.
2. Cliquez sur l'onglet de l'élément.
3. Sur la ligne de l'élément, cliquez sur le crayon de la colonne `Actions`.
4. Modifiez les champs voulus.
5. Cliquez sur `Enregistrer`.

### Importer ou exporter un référentiel comptable

Dans INGENEO PRECOMPTA, le menu à 3 traits de chaque onglet de `Référentiels comptables > Comptabilité` propose `Importer / Exporter`. Le panneau `Importer / Exporter` contient les blocs `IMPORTER DES DONNÉES` et `EXPORTER LES DONNÉES`. Il affiche aussi les `Règles d'import` propres à l'onglet.

Pour importer des données :

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Comptabilité`.
2. Cliquez sur l'onglet voulu.
3. Cliquez sur le menu à 3 traits, à droite de `Ajouter`.
4. Cliquez sur `Importer / Exporter`.
5. Dans le bloc `IMPORTER DES DONNÉES`, cliquez sur `Télécharger le modèle`. Le modèle est un fichier Excel.
6. Remplissez le modèle en respectant les `Règles d'import` affichées dans le panneau.
7. Cliquez sur `Importer un document`.
8. Sélectionnez le modèle rempli sur votre ordinateur.

Exemple de `Règles d'import` de l'onglet `Journaux` : `Code`, `Intitulé` et `Type` sont obligatoires. `Type` accepte `ACHAT`, `AUTRE`, `BANQUE` ou `VENTE`. `Contrepartie` est obligatoire si le type est `BANQUE`, et doit exister dans le dossier comptable.

Pour exporter des données :

1. Ouvrez le panneau `Importer / Exporter` de l'onglet voulu.
2. Dans le bloc `EXPORTER LES DONNÉES`, cliquez sur `Exporter les données`.

L'utilisateur reçoit un e-mail avec un lien pour télécharger le fichier.

### Supprimer des éléments de référentiel comptable

{% hint style="danger" %}
Dans INGENEO PRECOMPTA, la suppression d'éléments de référentiel comptable avec `Tout supprimer` est définitive. Seuls `Synchroniser` ou un import FEC peuvent récupérer à nouveau les éléments supprimés.
{% endhint %}

Pour supprimer un seul élément, cliquez sur `Supprimer` dans la colonne `Actions` de sa ligne, dans l'onglet de `Référentiels comptables > Comptabilité`.

Pour supprimer tous les éléments d'un onglet :

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Comptabilité`.
2. Cliquez sur l'onglet voulu.
3. Cliquez sur le menu à 3 traits, à droite de `Ajouter`.
4. Cliquez sur `Tout supprimer`. Le panneau `Suppression critique` s'ouvre.
5. Dans le champ `Pour confirmer, saisissez « … »`, saisissez le nom demandé (exemple : `Journal` pour l'onglet `Journaux`).
6. Dans le champ `Code de sécurité`, saisissez le code de votre application OTP.
7. Cliquez sur `Confirmer la suppression`.

`Tout supprimer` ne supprime que les éléments de l'onglet affiché.

## Résultat attendu

Dans INGENEO PRECOMPTA, les éléments ajoutés, modifiés, importés ou synchronisés apparaissent dans l'onglet correspondant de `Entreprises > Editer > Entreprise > Référentiels comptables > Comptabilité` : `Journaux`, `Comptes tiers`, `Plan comptable`, `Codes TVA` ou `Modes de règlement`.

L'affichage et l'automatisation des éléments comptables dans la pré-saisie comptable se règlent dans le paramétrage des classeurs comptables, décrit dans [Créer et paramétrer un classeur comptable](classeurs-comptables.md).

## Erreurs fréquentes

* **Bouton `Synchroniser` absent de `Référentiels comptables > Comptabilité` dans INGENEO PRECOMPTA.** Le logiciel comptable de l'entreprise ne permet pas la synchronisation. Importez les référentiels comptables avec `Importer un FEC`, ou créez-les avec `Ajouter`.
* **Message `Erreur de synchronisation` après un clic sur `Synchroniser` dans INGENEO PRECOMPTA.** La synchronisation avec le logiciel comptable a échoué. Le message indique la raison de l'échec. La connexion d'une entreprise à son logiciel comptable tiers est décrite dans [Connecter un logiciel comptable tiers](connecter-un-logiciel-comptable-tiers.md).
* **Message `La présence de comptes tiers ou de comptes de plan comptable empêche l'intégration d'un plan comptable générique.` dans INGENEO PRECOMPTA.** L'entreprise contient déjà des comptes tiers ou des comptes du plan comptable. Le bouton `Intégrer plan comptable générique` ne fonctionne que si les onglets `Comptes tiers` et `Plan comptable` sont vides.
* **Élément absent après une suppression avec `Tout supprimer` dans INGENEO PRECOMPTA.** La suppression est définitive. Récupérez les éléments avec `Synchroniser` ou par un import FEC.

## Fiches liées

* [Créer et paramétrer un classeur comptable](classeurs-comptables.md) : affichage et automatisation des éléments comptables dans la pré-saisie comptable.
* [Paramétrer et saisir l'analytique](analytique.md) : sous-menu `Analytiques` de `Référentiels comptables`.
* [Paramétrage avancé de la comptabilité](parametrage-comptabilite-avance.md) : règles de création des comptes tiers et longueur des comptes du plan comptable.
* [Faire la pré-saisie comptable](../gestion-des-documents/la-saisie-comptable.md) : création d'un compte tiers depuis l'écran de pré-saisie comptable.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-gerer-referentiels-comptables-ingeneo-precompta
* titre : Comment gérer les référentiels comptables d'une entreprise dans INGENEO PRECOMPTA ?
* titre\_menu : Gérer les référentiels comptables
* type : procedure
* module : Gestion des entreprises
* version\_outil : 2.16.0
* roles\_concernes : utilisateur ayant le droit `Autoriser l'accès au paramétrage de la comptabilité`
* tags : référentiels comptables, journaux, comptes tiers, plan comptable, codes TVA, synchronisation
* formulations\_utilisateur : « comment ajouter un journal comptable » ; « synchroniser les comptes avec mon logiciel comptable » ; « importer le plan comptable d'une entreprise » ; « créer un code TVA » ; « supprimer tous les comptes tiers »
* sources : Refonte de la page GitBook ingeneo-pre-compta/gestion-des-entreprises/referentiels-comptables ; démo Arcade « Synchronisation des référentiels comptable » ; observation de l'application 2.16.0 (2026-11-04) ; interview expert 2026-11-04 ; expert 2026-10-19 (message `Erreur de synchronisation`)
* redacteur : CG
* relecteur :
* derniere\_verification : 2026-11-04
* statut : brouillon

</details>
