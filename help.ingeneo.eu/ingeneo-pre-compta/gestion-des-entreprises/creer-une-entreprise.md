---
description: >-
  Cette procédure permet de créer une entreprise dans INGENEO PRECOMPTA. Elle
  prend environ 3 minutes et nécessite le droit Autoriser la création
  d'entreprise.
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

# Comment créer une entreprise dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de créer une entreprise dans INGENEO PRECOMPTA, depuis le menu `Entreprises`. Elle prend environ 3 minutes et nécessite le droit `Autoriser la création d'entreprise`.

## Objectif

Dans INGENEO PRECOMPTA, la création d'une entreprise initialise un nouveau dossier comptable. Elle est obligatoire avant de traiter les factures de cette entreprise. Elle est aussi obligatoire avant d'accéder aux paramètres avancés de l'entreprise.

Les utilisateurs d'INGENEO PRECOMPTA appellent souvent une entreprise un « dossier ».

## Prérequis

* L'utilisateur d'INGENEO PRECOMPTA doit avoir le droit [`Autoriser la création d'entreprise`](../administration/detail-des-droits.md). Par défaut, les profils `Collaborateur de site` et `Gestionnaire de site` ont ce droit.
* Le code dossier de l'entreprise dans le logiciel comptable doit être connu.
* Le SIREN et la raison sociale de l'entreprise doivent être connus.
* Si vous importez un fichier FEC, préparez un fichier FEC à jour au format `.txt`. Les FEC provisoires sont acceptés.
* Si vous utilisez un modèle d'entreprise, un administrateur doit avoir [créé ce modèle](../administration/modeles-dentreprises.md) avant la création de l'entreprise dans INGENEO PRECOMPTA. Le modèle doit être activé.

## Étapes

{% hint style="danger" %}
Dans INGENEO PRECOMPTA, le champ `Code dossier` d'une entreprise doit être identique au code dossier du logiciel comptable. Si les deux codes diffèrent, la synchronisation ne se fait pas. Les écritures et les documents ne sont alors pas intégrés en comptabilité.
{% endhint %}

1. Dans INGENEO PRECOMPTA, dans le menu de gauche, cliquez sur `Entreprises`.
2. Cliquez sur `+ Ajouter`.
3. Dans la page `Généralités`, renseignez le champ `SIREN`.
4. Renseignez le champ `Raison sociale`.
5. Si le logiciel comptable n'est pas interconnecté par API avec INGENEO PRECOMPTA, saisissez dans le champ `Code dossier` le code dossier du logiciel comptable.
6. Si le logiciel comptable est interconnecté par API avec INGENEO PRECOMPTA, sélectionnez le code dossier dans la liste déroulante du champ `Code dossier`.
7. Dans le champ `Site`, sélectionnez le ou les sites de l'entreprise.
8. Si vous n'avez pas créé de site, sélectionnez `site par défaut` dans le champ `Site`.
9. Cliquez sur `Suivant`.
10. Si vous utilisez un modèle d'entreprise, sélectionnez-le dans la liste déroulante `Sélectionner un modèle`.
11. Si vous avez sélectionné un modèle d'entreprise, activez les imports souhaités parmi : `Importer les classeurs comptables`, `Importer les référentiels comptables`, `Importer les référentiels analytiques`, `Importer le plan de classement`, `Importer les processus métier`, `Importer les profils d'entreprise` et `Importer la comptabilité`.
12. Dans la zone `Importer un fichier FEC`, cliquez sur `Parcourir` (recommandé).
13. Sélectionnez le fichier FEC au format `.txt`.
14. Vérifiez les libellés d'écriture proposés par défaut : `[Intitulé Tiers]` pour les achats et `[Numéro Facture]` pour les ventes.
15. Si vous souhaitez changer un libellé d'écriture, faites un clic droit dans son champ et choisissez une autre variable d'automatisation.
16. Cliquez sur `Enregistrer` en bas de page.
17. Sélectionnez l'action souhaitée parmi les trois proposées : `+... puis créer une nouvelle entreprise`, `+... puis traiter les factures` ou `+... puis accéder aux paramètres avancés`.

Dans INGENEO PRECOMPTA, l'import d'un fichier FEC crée les [référentiels comptables](referentiels-comptables.md) de l'entreprise : codes journaux, comptes de tiers et comptes comptables. Il récupère aussi les occurrences, ce qui permet à INGENEO PRECOMPTA de proposer des saisies adaptées dès le démarrage. L'import FEC n'importe pas les écritures comptables.

## Résultat attendu

Dans INGENEO PRECOMPTA, l'entreprise créée apparaît dans le menu `Entreprises`, associée au ou aux sites sélectionnés. L'action choisie après `Enregistrer` s'ouvre.

Les paramètres de l'entreprise restent modifiables après la création, dans les paramètres avancés de l'entreprise. Les paramètres avancés regroupent : [Informations générales](parametrages-generaux.md), comptabilité, [classeurs comptables](classeurs-comptables.md), [référentiels comptables](referentiels-comptables.md) et facturation électronique.

Le champ `Code dossier` reste modifiable après la création de l'entreprise. Sa modification nécessite le droit `Autoriser l'accès au paramétrage de la comptabilité`.

## Erreurs fréquentes

* **Message `Ficher pas au bon format` lors de l'import du fichier FEC à la création d'une entreprise dans INGENEO PRECOMPTA.** Le fichier FEC n'est pas au format attendu. Vérifiez que le fichier FEC est au format `.txt`. Les FEC provisoires sont acceptés. Vérifiez que les codes journaux sont présents dans le fichier. \[À VÉRIFIER : le message affiché commence-t-il bien par `Ficher` (sans « i »), ou par `Fichier` ?]
* **Écritures et documents non intégrés en comptabilité après la création d'une entreprise dans INGENEO PRECOMPTA.** Le champ `Code dossier` de l'entreprise diffère probablement du code dossier du logiciel comptable, ce qui bloque la synchronisation. Comparez les deux codes dossier. Corrigez le champ `Code dossier` dans les paramètres avancés de l'entreprise, rubrique comptabilité.
* **Modèle d'entreprise absent de la liste `Sélectionner un modèle` dans INGENEO PRECOMPTA.** Un modèle désactivé n'apparaît pas dans la liste. Un modèle doit aussi être créé par un administrateur avant la création de l'entreprise. Demandez à un administrateur de créer ou d'activer le modèle.

## Fiches liées

* [Détail des droits](../administration/detail-des-droits.md) : description du droit `Autoriser la création d'entreprise`
* [Modèles d'entreprises](../administration/modeles-dentreprises.md) : création et activation d'un modèle avant la création d'une entreprise
* [Paramétrages généraux](parametrages-generaux.md) : informations générales de l'entreprise après sa création
* [Référentiels comptables](referentiels-comptables.md) : référentiels créés par l'import du fichier FEC
* [Classeurs & éléments comptables](classeurs-comptables.md) : paramétrage des classeurs de l'entreprise

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-creer-une-entreprise
* type : procedure
* module : Entreprises
* version\_outil : toutes
* roles\_concernes : Collaborateur de site, Gestionnaire de site
* tags : création entreprise ; dossier ; code dossier ; FEC ; modèle d'entreprise
* formulations\_utilisateur : « ajouter un dossier » ; « créer un dossier » ; « créer un nouveau dossier » ; « ajouter une entreprise »
* sources : Refonte de la page GitBook /ingeneo-pre-compta/gestion-des-entreprises/creer-une-entreprise ; réponses de l'expert 2026-10-13 ; page GitBook /ingeneo-pre-compta/administration/detail-des-droits (droit lié au code dossier)
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-13
* statut : brouillon

</details>
