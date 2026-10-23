---
description: >-
  Dans INGENEO PRECOMPTA, créer une entreprise en important le paramétrage d'un
  modèle d'entreprise, depuis l'étape Initialisation du panneau Créer une
  entreprise.
---

# Comment créer une entreprise depuis un modèle dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de créer une entreprise dans INGENEO PRECOMPTA en important le paramétrage d'un modèle d'entreprise. Elle prend environ 3 minutes et nécessite le droit `Autoriser la création d'entreprise`.

## Objectif

Dans INGENEO PRECOMPTA, un modèle d'entreprise permet de créer une entreprise avec un paramétrage déjà prêt. Le modèle se choisit à l'étape `Initialisation` du panneau `Créer une entreprise`. Les autres étapes sont celles de [Créer une entreprise](creer-une-entreprise.md).

Chaque interrupteur `Importer …` de l'étape `Initialisation` importe uniquement les éléments de l'onglet du modèle qui porte le même nom. Après la création, l'entreprise n'est plus liée au modèle : une modification ultérieure du modèle ne change pas l'entreprise.

## Prérequis

* Droit : l'utilisateur d'INGENEO PRECOMPTA doit avoir le droit [`Autoriser la création d'entreprise`](../administration/detail-des-droits.md). Aucun autre droit n'est nécessaire pour utiliser un modèle d'entreprise. Par défaut, les profils `Collaborateur de site` et `Gestionnaire de site` ont ce droit.
* Modèle d'entreprise : le modèle doit exister avant la création de l'entreprise. Un administrateur le crée dans `Entreprises > Actions > PARAMÉTRAGE GLOBAL > Modèles génériques`, rubrique `Modèles d'entreprise`. La procédure est décrite dans [Modèles d'entreprises](../administration/modeles-dentreprises.md).
* Activation : l'interrupteur `Activer le modèle` du modèle d'entreprise doit être activé.
* Sites : le modèle d'entreprise doit prévoir le site de la nouvelle entreprise, dans son champ `Sites` ou avec `Appliquer sur tous les sites`.
* Informations de l'entreprise : le SIREN, la raison sociale et le code dossier du logiciel comptable doivent être connus.
* FEC : si vous importez un fichier FEC, préparez un fichier FEC à jour au format `.txt`. Les FEC provisoires sont acceptés.

## Étapes

{% hint style="danger" %}
Dans INGENEO PRECOMPTA, le champ `Code dossier` d'une entreprise doit être identique au code dossier du logiciel comptable. Si les deux codes diffèrent, la synchronisation ne se fait pas. Les écritures et les documents ne sont alors pas intégrés en comptabilité.
{% endhint %}

### Renseigner l'étape Généralités

1. Dans INGENEO PRECOMPTA, dans le menu de gauche, cliquez sur `Entreprises`.
2. Cliquez sur `Ajouter`. Le panneau `Créer une entreprise` s'ouvre sur l'étape `Généralités`.
3. Renseignez le champ `SIREN`.
4. Renseignez le champ `Raison sociale`.
5. Si le logiciel comptable n'est pas interconnecté par API avec INGENEO PRECOMPTA, saisissez dans le champ `Code dossier` le code dossier du logiciel comptable.
6. Si le logiciel comptable est interconnecté par API avec INGENEO PRECOMPTA, sélectionnez le code dossier dans la liste déroulante du champ `Code dossier`.
7. Dans le champ `Sites`, sélectionnez le ou les sites de l'entreprise. Ce choix détermine les modèles proposés à l'étape `Initialisation`.
8. Si vous n'avez pas créé de site, sélectionnez `Site par défaut` dans le champ `Sites`.
9. Cliquez sur `Suivant`. L'étape `Initialisation` s'affiche.

### Choisir le modèle à l'étape Initialisation

Dans le panneau `Créer une entreprise` d'INGENEO PRECOMPTA, la liste `Sélectionner un modèle` ne propose que les modèles d'entreprise activés qui prévoient le site choisi à l'étape `Généralités`. Sans site choisi, elle affiche `Aucun modèle disponible`.

1. Dans le bloc `IMPORTER DEPUIS UN MODÈLE`, ouvrez la liste `Sélectionner un modèle`.
2. Sélectionnez le modèle d'entreprise. Les 7 interrupteurs d'import s'affichent, tous activés.
3. Si vous ne voulez pas importer les classeurs comptables du modèle, désactivez `Importer les classeurs comptables`.
4. Si vous ne voulez pas importer les référentiels comptables du modèle, désactivez `Importer les référentiels comptables`.
5. Si vous ne voulez pas importer les référentiels analytiques du modèle, désactivez `Importer les référentiels analytiques`.
6. Si vous ne voulez pas importer le plan de classement du modèle, désactivez `Importer le plan de classement`.
7. Si vous ne voulez pas importer les processus métier du modèle, désactivez `Importer les processus métier`.
8. Si vous ne voulez pas importer les profils d'entreprise du modèle, désactivez `Importer les profils d'entreprise`.
9. Si vous ne voulez pas importer la comptabilité du modèle, désactivez `Importer la comptabilité`.

### Importer un fichier FEC (facultatif)

1. Dans le bloc `INITIALISATION DES DONNÉES`, zone `Importer un fichier FEC`, cliquez sur `Parcourir...`.
2. Sélectionnez le fichier FEC au format `.txt`.

Dans INGENEO PRECOMPTA, le fichier FEC est traité après la création de l'entreprise. Il met à jour les référentiels comptables importés du modèle. Il ajoute aussi les comptes et les journaux absents du modèle.

### Paramétrer les classeurs comptables sans le modèle

Dans le panneau `Créer une entreprise` d'INGENEO PRECOMPTA, le bloc `CLASSEURS COMPTABLES` est masqué quand un modèle est sélectionné avec `Importer les classeurs comptables` activé. Il s'affiche si cet interrupteur est désactivé.

1. Si vous avez désactivé `Importer les classeurs comptables`, dans le bloc `CLASSEURS COMPTABLES`, activez l'interrupteur de la ligne `Achats`, de la ligne `Ventes`, ou des deux.
2. Vérifiez le `Libellé d'écriture` proposé par défaut : `[Intitule Tiers]` pour les achats et `[Numero Facture]` pour les ventes.
3. Vérifiez le `Code journal` proposé par défaut : `ACH` pour les achats et `VEN` pour les ventes.

### Enregistrer l'entreprise

1. En bas du panneau `Créer une entreprise`, cliquez sur `Enregistrer...`.
2. Sélectionnez l'action suivante parmi `... puis créer une nouvelle entreprise`, `... puis traiter les factures` ou `... puis accéder aux paramètres avancés`.

## Résultat attendu

Dans INGENEO PRECOMPTA, l'entreprise créée apparaît dans le menu `Entreprises`, associée au ou aux sites sélectionnés. L'action choisie après `Enregistrer...` s'ouvre.

L'entreprise contient les éléments des onglets du modèle d'entreprise dont l'interrupteur `Importer …` était activé. Si `Importer la comptabilité` était activé, le champ `Logiciel` de l'entreprise est celui du modèle, même si un autre logiciel avait été choisi à l'étape `Généralités`.

Si un fichier FEC a été importé, les référentiels comptables de l'entreprise sont mis à jour après la création, avec les comptes et les journaux du FEC.

L'entreprise n'est pas liée au modèle d'entreprise. Une modification ultérieure du modèle dans `Modèles génériques` ne change pas l'entreprise. Ses paramètres restent modifiables dans ses paramètres avancés.

## Erreurs fréquentes

* **Liste `Sélectionner un modèle` affichant `Aucun modèle disponible` dans INGENEO PRECOMPTA.** Aucun site n'a été choisi à l'étape `Généralités` du panneau `Créer une entreprise`. Cliquez sur `Précédent`, sélectionnez un site dans le champ `Sites`, puis cliquez sur `Suivant`.
* **Modèle d'entreprise absent de la liste `Sélectionner un modèle` dans INGENEO PRECOMPTA.** Le modèle ne prévoit pas le site choisi à l'étape `Généralités`, ou son interrupteur `Activer le modèle` est désactivé. Demandez à un administrateur d'ajouter le site au modèle (champ `Sites` ou `Appliquer sur tous les sites`) ou d'activer le modèle, dans `Entreprises > Actions > PARAMÉTRAGE GLOBAL > Modèles génériques`.
* **Logiciel de l'entreprise différent de celui choisi à l'étape `Généralités` dans INGENEO PRECOMPTA.** L'interrupteur `Importer la comptabilité` était activé : l'entreprise reçoit le `Logiciel` du modèle d'entreprise. Pour garder le logiciel choisi à l'étape `Généralités`, désactivez `Importer la comptabilité` avant d'enregistrer. Pour une entreprise déjà créée, modifiez le champ `Logiciel` dans ses paramètres avancés, rubrique comptabilité.

## Fiches liées

* [Créer une entreprise](creer-une-entreprise.md) : création d'une entreprise sans modèle
* [Modèles d'entreprises](../administration/modeles-dentreprises.md) : création, activation et sites d'un modèle d'entreprise
* [Référentiels comptables](referentiels-comptables.md) : référentiels importés du modèle ou mis à jour par le fichier FEC

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-creer-entreprise-depuis-modele-ingeneo-precompta
* titre\_menu : Créer une entreprise depuis un modèle
* type : procedure
* module : Gestion des entreprises
* version\_outil : 2.13.0 (version observée)
* roles\_concernes : utilisateur avec le droit `Autoriser la création d'entreprise` (par défaut : Collaborateur de site, Gestionnaire de site)
* tags : création entreprise ; modèle d'entreprise ; dossier ; import ; FEC ; classeurs comptables
* formulations\_utilisateur : « créer un dossier à partir d'un modèle » ; « utiliser un modèle d'entreprise » ; « appliquer un modèle à une nouvelle entreprise » ; « mon modèle n'apparaît pas dans la liste »
* sources : Page GitBook /ingeneo-pre-compta/gestion-des-entreprises/creer-une-entreprise ; observation de l'application INGENEO PRECOMPTA 2.13.0 (panneau `Créer une entreprise` et `Modèles génériques`, 2026-10-21) ; réponses de l'expert 2026-10-21
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-22
* statut : brouillon

</details>
