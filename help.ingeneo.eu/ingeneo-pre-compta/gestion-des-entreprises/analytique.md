---
description: >-
  Paramétrer l'analytique dans INGENEO PRECOMPTA : axes et sections analytiques,
  activation dans les classeurs comptables et ventilation des lignes d'écriture
  dans Bannettes.
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

# Comment paramétrer et saisir l'analytique d'une entreprise dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de créer les axes et sections analytiques d'une entreprise, d'activer l'analytique dans ses classeurs comptables et de ventiler les lignes d'écriture dans INGENEO PRECOMPTA. Le paramétrage prend environ 6 minutes. Il nécessite les droits `Autoriser l'accès au paramétrage de la comptabilité` et `Gérer les référentiels associés (ajouter, modifier, supprimer)`.

## Objectif

Dans INGENEO PRECOMPTA, l'analytique permet de ventiler le montant d'une ligne d'écriture sur des axes et des sections analytiques. Elle sert à suivre des budgets, des projets ou des chantiers.

* Un axe analytique est un critère de répartition, par exemple « Chantier ».
* Une section analytique est une subdivision d'un axe. Chaque section a un `Niveau` de 1 à 10. Exemple : axe « Chantier », section de niveau 1 « Matière première », section de niveau 2 « Ciment ».

La procédure se fait en trois temps :

1. Créer les axes et les sections dans `Entreprises > Editer > Entreprise > Référentiels comptables > Analytiques`.
2. Activer l'élément `ANALYTIQUES` dans l'onglet `Eléments comptables` de chaque classeur comptable concerné.
3. Ventiler les lignes d'écriture dans le menu `Bannettes`, pendant la pré-saisie comptable.

Les intitulés des niveaux de section (`Section #1` à `Section #10`) se personnalisent dans `Comptabilité > Paramétrage avancé`, bloc `PARAMÉTRAGE DE L'ANALYTIQUE`. Ce réglage est décrit dans [Paramétrage avancé de la comptabilité](parametrage-comptabilite-avance.md).

## Prérequis

* Droits pour le paramétrage : dans INGENEO PRECOMPTA, la création des axes et des sections analytiques nécessite deux droits : `Autoriser l'accès au paramétrage de la comptabilité` et `Gérer les référentiels associés (ajouter, modifier, supprimer)`. Le détail des droits est dans [Détail des droits](../administration/detail-des-droits.md).
* Droit pour la saisie : dans INGENEO PRECOMPTA, la ventilation analytique dans le menu `Bannettes` nécessite seulement le droit `Enregistrer les documents`.
* Logiciel comptable : certains logiciels comptables ne reçoivent pas les lignes analytiques exportées par INGENEO PRECOMPTA, et d'autres les reçoivent sans les traiter. Il n'existe pas de liste des logiciels compatibles : vérifiez dans votre logiciel comptable qu'il gère l'analytique.
* Organisation analytique : préparez la liste des axes et des sections analytiques à créer, avec leur niveau.

## Étapes

### Ouvrir l'écran Analytiques d'une entreprise

1. Dans INGENEO PRECOMPTA, cliquez sur `Entreprises` dans le menu de gauche.
2. Sur l'écran `Entreprises`, sur la ligne de l'entreprise, cliquez sur `Editer`.
3. Dans l'onglet `Entreprise`, cliquez sur `Référentiels comptables`.
4. Cliquez sur `Analytiques`.

L'écran affiche deux onglets : `Axes analytiques` et `Sections analytiques`.

### Récupérer les axes et sections par synchronisation

Dans INGENEO PRECOMPTA, écran `Référentiels comptables > Analytiques` d'une entreprise, le bouton `Synchroniser` récupère les axes et les sections analytiques du logiciel comptable. La synchronisation fonctionne avec les logiciels comptables dont la technologie le permet, le plus souvent par API.

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Analytiques`.
2. Cliquez sur `Synchroniser`.

Si la synchronisation récupère des sections, INGENEO PRECOMPTA crée automatiquement un axe par défaut (code `D_AXE`, intitulé `Axe par défaut`). Sans synchronisation, créez au moins un axe à la main.

### Créer un axe analytique

Dans INGENEO PRECOMPTA, toute section analytique doit être rattachée à un axe analytique. Créez au moins un axe avant de créer des sections. Le `Code` et l'`Intitulé` de l'axe sont libres.

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Analytiques`.
2. Cliquez sur l'onglet `Axes analytiques`.
3. Cliquez sur `Ajouter`.
4. Dans le panneau `Axe analytique`, renseignez le champ `Code`.
5. Renseignez le champ `Intitulé`.
6. Cliquez sur `Enregistrer`.

### Créer une section analytique

1. Ouvrez `Entreprises > Editer > Entreprise > Référentiels comptables > Analytiques`.
2. Cliquez sur l'onglet `Sections analytiques`.
3. Cliquez sur `Ajouter`.
4. Dans le panneau `Section analytique`, sélectionnez l'axe dans le champ `Axe analytique`.
5. Renseignez le champ `Code`.
6. Renseignez le champ `Intitulé`.
7. Dans le champ `Niveau`, sélectionnez le niveau de la section, de `1` à `10`.
8. Cliquez sur `Enregistrer`.

Les niveaux sont indépendants : une section de niveau 2 ne dépend pas d'une section de niveau 1. Pour modifier une section existante, cliquez sur l'icône d'édition de sa ligne, dans la colonne `Actions` de l'onglet `Sections analytiques`.

### Importer ou supprimer des axes et sections en masse

Dans INGENEO PRECOMPTA, écran `Référentiels comptables > Analytiques`, le menu à 3 traits des onglets `Axes analytiques` et `Sections analytiques` propose deux actions :

* `Import / Exporter` : importe ou exporte la liste avec un fichier `.xlsx`. Téléchargez le modèle proposé et remplissez-le en respectant sa structure.
* `Tout supprimer` : supprime toute la liste de l'onglet. Les lignes analytiques déjà saisies sur les écritures ne sont pas supprimées.

### Activer l'analytique dans un classeur comptable

Dans INGENEO PRECOMPTA, aucune ventilation analytique n'est proposée dans le menu `Bannettes` tant que l'élément comptable `ANALYTIQUES` n'est pas actif dans le classeur comptable. Répétez cette étape pour chaque classeur concerné.

1. Ouvrez `Entreprises > Editer > Entreprise > Classeurs comptables`.
2. Sur la ligne du classeur, cliquez sur le bouton d'édition.
3. Dans le panneau `Classeur comptable`, cliquez sur l'onglet `Eléments comptables`.
4. Sur l'élément `ANALYTIQUES`, activez l'interrupteur `Actif`.
5. Dans `Autoriser la saisie sur les classes de compte :`, ajoutez les classes de compte qui acceptent l'analytique, par exemple `6`.
6. Si l'analytique doit être obligatoire, ajoutez les classes de compte concernées dans `Obliger la saisie sur les classes de compte :`.
7. Si besoin, sélectionnez un axe dans `Axe analytique par défaut :`.
8. Si besoin, sélectionnez une section dans chaque champ `Section analytique par défaut niveau N :`.
9. Cliquez sur `Enregistrer`.

Effet des champs de l'élément `ANALYTIQUES` :

| Champ                                             | Effet dans le menu `Bannettes`                                                                                                                         |
| ------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| `Autoriser la saisie sur les classes de compte :` | Une ligne analytique peut être ajoutée sous une ligne d'écriture dont le compte appartient à une de ces classes.                                       |
| `Obliger la saisie sur les classes de compte :`   | Une ligne analytique vide est ajoutée automatiquement sous la ligne d'écriture. Le bouton `Enregistrer` reste grisé tant qu'elle n'est pas renseignée. |
| `Axe analytique par défaut :`                     | Axe proposé sur chaque nouvelle ligne analytique. L'utilisateur peut le modifier.                                                                      |
| `Section analytique par défaut niveau N :`        | Section proposée pour le niveau N. Un champ s'affiche pour chaque niveau qui existe dans les sections analytiques. L'utilisateur peut la modifier.     |

{% hint style="warning" %}
Dans INGENEO PRECOMPTA, si l'élément `ANALYTIQUES` d'un classeur comptable est désactivé, les écritures déjà ventilées restent exportées vers le logiciel comptable, mais sans leurs lignes analytiques. Ne désactivez pas l'analytique en cours d'exercice sans l'accord de l'expert-comptable.
{% endhint %}

### Ventiler une ligne d'écriture dans Bannettes

Dans INGENEO PRECOMPTA, la ventilation analytique se fait pendant la pré-saisie comptable, dans le menu `Bannettes`. Elle n'est possible que si l'élément `ANALYTIQUES` est actif dans le classeur comptable.

1. Dans le menu de gauche, cliquez sur `Bannettes`.
2. Ouvrez le classeur comptable de l'entreprise.
3. Ouvrez le document à imputer.
4. Dans le tableau des lignes d'écriture, survolez avec la souris l'espace situé sous la ligne d'écriture à ventiler.
5. Cliquez sur `Insérer une ligne analytique`. Le raccourci `CTRL+A` ajoute aussi une ligne analytique sous la ligne d'écriture dont le compte appartient à une classe autorisée.
6. Dans la colonne `Compte` de la ligne analytique, sélectionnez l'axe analytique.
7. Dans la colonne `Libellé`, sélectionnez la section de chaque niveau utilisé, dans le champ intitulé `Section #1`, `Section #2` ou l'intitulé personnalisé.
8. Saisissez la part à ventiler : un pourcentage dans la colonne située juste avant le montant, ou un montant dans la colonne de droite.
9. Pour répartir la ligne d'écriture sur plusieurs sections, ajoutez une ligne analytique par section.
10. Cliquez sur `Enregistrer`.

La ligne analytique insérée reprend d'abord le montant de la ligne d'écriture. Quand un pourcentage est saisi, INGENEO PRECOMPTA calcule le montant automatiquement. La somme des lignes analytiques doit être égale au montant de la ligne d'écriture.

## Résultat attendu

Dans INGENEO PRECOMPTA, à la fin du paramétrage :

* les onglets `Axes analytiques` et `Sections analytiques` de `Référentiels comptables > Analytiques` listent les axes et les sections de l'entreprise ;
* dans le menu `Bannettes`, les classeurs comptables où `ANALYTIQUES` est actif proposent `Insérer une ligne analytique` sous les lignes d'écriture des classes de compte autorisées ;
* après ventilation et clic sur `Enregistrer`, l'écriture est enregistrée avec ses lignes analytiques, puis exportée avec elles si le logiciel comptable gère l'analytique.

## Erreurs fréquentes

**Le bouton `Enregistrer` est grisé et une ligne analytique s'encadre en rouge au survol du bouton.** Dans INGENEO PRECOMPTA, menu `Bannettes`, deux causes sont possibles. Première cause : la ligne analytique ajoutée automatiquement sur une classe de compte obligatoire est vide ; renseignez son axe et sa section. Deuxième cause : la somme des lignes analytiques ne correspond pas au montant de la ligne d'écriture ; corrigez les pourcentages ou les montants.

**`Insérer une ligne analytique` n'apparaît pas dans `Bannettes`.** Dans INGENEO PRECOMPTA, l'élément `ANALYTIQUES` n'est pas actif dans le classeur comptable, ou la classe du compte de la ligne d'écriture ne figure pas dans `Autoriser la saisie sur les classes de compte :`. Vérifiez l'onglet `Eléments comptables` du classeur, dans `Entreprises > Editer > Entreprise > Classeurs comptables`.

**Aucun axe n'est proposé dans le classeur comptable ou sur la ligne analytique.** Dans INGENEO PRECOMPTA, l'entreprise n'a aucun axe analytique. Créez un axe dans `Référentiels comptables > Analytiques > Axes analytiques`, ou cliquez sur `Synchroniser` si le logiciel comptable le permet.

**Une section analytique ne peut pas être créée.** Dans INGENEO PRECOMPTA, une section analytique doit être rattachée à un axe. Créez d'abord un axe dans l'onglet `Axes analytiques`.

**Les lignes analytiques n'arrivent pas dans le logiciel comptable.** Dans INGENEO PRECOMPTA, deux causes sont possibles. Le logiciel comptable ne gère pas l'analytique : certains ne reçoivent pas les lignes analytiques, d'autres ne les traitent pas. Ou l'élément `ANALYTIQUES` du classeur comptable a été désactivé : les écritures sont alors exportées sans analytique.

## Fiches liées

* [Paramétrage avancé de la comptabilité](parametrage-comptabilite-avance.md) : personnalisation des intitulés `Section #1` à `Section #10` (bloc `PARAMÉTRAGE DE L'ANALYTIQUE`).
* [Créer et paramétrer un classeur comptable](classeurs-comptables.md) : onglet `Eléments comptables` du classeur.
* [Détail des droits](../administration/detail-des-droits.md) : droits `Autoriser l'accès au paramétrage de la comptabilité`, `Gérer les référentiels associés (ajouter, modifier, supprimer)` et `Enregistrer les documents`.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-parametrer-saisir-analytique-ingeneo-precompta
* titre : Comment paramétrer et saisir l'analytique d'une entreprise dans INGENEO PRECOMPTA ?
* titre\_menu : Paramétrer et saisir l'analytique
* type : procedure
* module : Gestion des entreprises
* version\_outil : 2.11.0 (version observée)
* roles\_concernes : utilisateur avec les droits `Autoriser l'accès au paramétrage de la comptabilité` et `Gérer les référentiels associés (ajouter, modifier, supprimer)` (paramétrage) ; utilisateur avec le droit `Enregistrer les documents` (saisie)
* tags : analytique, axe analytique, section analytique, classeur comptable, ventilation, Bannettes
* formulations\_utilisateur : « Comment créer un axe analytique ? » ; « L'analytique n'apparaît pas à la saisie » ; « Comment ventiler une facture sur plusieurs chantiers ? » ; « Le bouton Enregistrer est grisé avec une ligne en rouge » ; « Mon analytique ne remonte pas dans ma compta » ; « Comment ajouter une ligne analytique ? »
* sources : Refonte de la page GitBook ingeneo-pre-compta/gestion-des-entreprises/analytique ; démos Arcade « Création analytique » et « Saisie analytique » (captures) ; observation de l'application INGENEO PRECOMPTA 2.11.0 (2026-10-15) ; réponses de l'expert 2026-10-15
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-15
* statut : brouillon

</details>
