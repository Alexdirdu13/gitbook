---
description: >-
  Dans INGENEO PRECOMPTA, le menu Informations générales d'une entreprise
  regroupe ses informations légales (base SIRENE), son logo, ses établissements
  et son mot de passe d'accès.
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

# Comment modifier les informations générales d'une entreprise

**Résumé :** Cette procédure permet de consulter et de mettre à jour les informations générales d'une entreprise dans INGENEO PRECOMPTA : informations légales, logo, établissements et mot de passe d'accès. Elle prend environ 5 minutes. Elle nécessite le droit `Autoriser l'accès au paramétrage des informations générales`.

## Objectif

Dans INGENEO PRECOMPTA, le menu `Informations générales` d'une entreprise centralise ses données légales et administratives. Il se trouve dans `Entreprises > Editer > Entreprise > Informations générales` et contient trois sous-onglets :

* `Siège` : logo, mode de facturation, sites, SIREN, TVA intracommunautaire, raison sociale et autres informations légales de l'unité légale.
* `Etablissements` : le siège et les établissements fermés de l'entreprise, avec leur SIRET, leur adresse et leur code EPCI.
* `Sécurité` : le `Mot de passe d'accès à l'entreprise`, qui verrouille l'entreprise.

Les informations légales sont récupérées par une interconnexion avec la base SIRENE (https://annuaire-entreprises.data.gouv.fr).

Utilisez cette procédure dans les cas suivants :

* compléter le paramétrage après la [création d'une entreprise](creer-une-entreprise.md) ;
* mettre à jour l'entreprise après un changement légal, par exemple une nouvelle adresse ou une nouvelle forme juridique ;
* protéger l'accès à une entreprise par un mot de passe.

## Prérequis

* Droit : l'utilisateur doit avoir le droit `Autoriser l'accès au paramétrage des informations générales`. Sans ce droit, il ne voit pas le menu `Informations générales` ni ses sous-onglets `Siège`, `Etablissements` et `Sécurité`. Le détail des droits est dans [Détail des droits](../administration/detail-des-droits.md).
* SIREN : le numéro SIREN de l'entreprise doit être valide pour que INGENEO PRECOMPTA récupère ses informations dans la base SIRENE.
* Informations légales : avant une modification importante, vérifiez les informations de l'entreprise dans les registres officiels.
* Logo : préparez un fichier image au format JPG ou PNG, de 25 Mo maximum.

{% hint style="warning" %}
Dans INGENEO PRECOMPTA, ne modifiez pas les informations générales d'une entreprise pendant ses périodes de déclarations fiscales, ni sans avoir vérifié les informations légales officielles. Sinon, des informations erronées risquent de se retrouver dans la pré-saisie, puis dans la production comptable.
{% endhint %}

## Étapes

### Ouvrir les informations générales de l'entreprise

1. Dans INGENEO PRECOMPTA, cliquez sur `Entreprises` dans le menu de gauche.
2. Sur l'écran `Entreprises`, sur la ligne de l'entreprise, cliquez sur `Editer`.
3. Dans l'onglet `Entreprise`, cliquez sur `Informations générales`.

Le sous-onglet `Siège` s'affiche.

### Mettre à jour les informations légales depuis la base SIRENE

1. Dans INGENEO PRECOMPTA, ouvrez `Entreprises > Editer > Entreprise > Informations générales`.
2. Dans le sous-onglet `Siège`, vérifiez le numéro du champ `SIREN`.
3. À droite du champ `SIREN`, cliquez sur le bouton d'information `Récupérer les informations de l'entreprise.`
4. Vérifiez les valeurs récupérées.
5. Cliquez sur `Enregistrer`.

Le lien `cliquer ici` du sous-onglet `Etablissements` lance la même récupération que le bouton du champ `SIREN`. Dans les deux cas, cliquez ensuite sur `Enregistrer`.

La récupération met à jour toutes les informations de l'entreprise, sauf `Mode de facturation`, `Logo de l'entreprise` et `Sites`. Elle ne fonctionne que si le SIREN figure dans l'annuaire des entreprises et que l'entreprise n'a pas masqué ses informations. Sinon, les champs vides restent vides et les valeurs déjà saisies sont conservées.

Mettez à jour ces informations à intervalles réguliers pour rester conforme aux registres officiels.

### Modifier les autres champs du sous-onglet Siège

Dans INGENEO PRECOMPTA, sous-onglet `Informations générales > Siège`, tous les champs sont modifiables à la main :

| Champ                             | Contenu                                                                                                                                                                                                                                                                |
| --------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Mode de facturation`             | Liste : `Partage documentaire`, `SCI/LMNP/BNC`, `BNC`, `BIC 50 factures/an`, `BIC 150 factures/an`, `BIC 1000 factures/an`, `BIC 5000 factures/an`. Non mis à jour par la base SIRENE. Un changement de valeur modifie la facturation de l'entreprise.                 |
| `Sites`                           | Un ou plusieurs sites de rattachement de l'entreprise. Un site est un groupement d'entreprises auquel des utilisateurs sont rattachés. Un changement de site modifie donc la visibilité de l'entreprise pour certains utilisateurs. Non mis à jour par la base SIRENE. |
| `SIREN`                           | Numéro SIREN de l'entreprise.                                                                                                                                                                                                                                          |
| `TVA Intracom`                    | Numéro de TVA intracommunautaire.                                                                                                                                                                                                                                      |
| `Raison sociale`                  | Raison sociale de l'entreprise.                                                                                                                                                                                                                                        |
| `Date de création (unité légale)` | Date de création de l'unité légale.                                                                                                                                                                                                                                    |
| `Forme juridique`                 | Forme juridique de l'entreprise.                                                                                                                                                                                                                                       |
| `Code APE`                        | Code APE de l'entreprise.                                                                                                                                                                                                                                              |
| `Classe unité légale`             | Classe de l'unité légale.                                                                                                                                                                                                                                              |
| `Section`                         | Section d'activité.                                                                                                                                                                                                                                                    |
| `Sous-section`                    | Sous-section d'activité.                                                                                                                                                                                                                                               |

1. Dans INGENEO PRECOMPTA, ouvrez `Entreprises > Editer > Entreprise > Informations générales`.
2. Dans le sous-onglet `Siège`, modifiez le champ voulu.
3. Cliquez sur `Enregistrer`.

### Ajouter le logo de l'entreprise

1. Dans INGENEO PRECOMPTA, ouvrez `Entreprises > Editer > Entreprise > Informations générales`.
2. Dans le sous-onglet `Siège`, champ `Logo de l'entreprise`, cliquez sur le bouton d'envoi.
3. Dans la fenêtre de votre ordinateur, sélectionnez un fichier JPG ou PNG de 25 Mo maximum.
4. Cliquez sur `Enregistrer`.

Le logo s'affiche à gauche de la ligne de l'entreprise, sur l'écran `Entreprises` et dans le menu `Bannettes`.

### Consulter les établissements de l'entreprise

1. Dans INGENEO PRECOMPTA, ouvrez `Entreprises > Editer > Entreprise > Informations générales`.
2. Cliquez sur le sous-onglet `Etablissements`.

Le sous-onglet `Etablissements` affiche deux blocs, `SIÈGE` et `ÉTABLISSEMENTS FERMÉS`. Chaque établissement indique son `SIRET`, son `Adresse`, son `Code EPCI` et son `Libellé EPCI`. Ces informations proviennent de la base SIRENE. Pour les mettre à jour, cliquez sur le lien `cliquer ici` du bandeau, puis sur `Enregistrer`.

### Définir le mot de passe d'accès à l'entreprise

Dans INGENEO PRECOMPTA, le `Mot de passe d'accès à l'entreprise` verrouille l'entreprise. Les utilisateurs l'appellent aussi « code PIN ». Une fois le mot de passe défini, tous les utilisateurs doivent le saisir pour accéder aux paramètres, aux informations, aux documents, à la recherche et aux écritures de l'entreprise.

1. Dans INGENEO PRECOMPTA, ouvrez `Entreprises > Editer > Entreprise > Informations générales`.
2. Cliquez sur le sous-onglet `Sécurité`.
3. Dans le champ `Mot de passe d'accès à l'entreprise`, saisissez le mot de passe.
4. Cliquez sur `Enregistrer`.

Le mot de passe n'a aucune restriction de format. Utilisez un mot de passe distinct pour chaque entreprise à protéger.

### Modifier ou supprimer le mot de passe d'accès à l'entreprise

Dans INGENEO PRECOMPTA, une fois le `Mot de passe d'accès à l'entreprise` défini, le sous-onglet `Sécurité` propose les boutons `Modifier` et `Supprimer`. Toute modification ou suppression du mot de passe demande les identifiants de connexion de l'utilisateur. Si la double authentification est activée, elle est aussi demandée.

Pour changer le mot de passe :

1. Dans INGENEO PRECOMPTA, ouvrez `Entreprises > Editer > Entreprise > Informations générales`.
2. Cliquez sur le sous-onglet `Sécurité`.
3. Cliquez sur `Modifier`.
4. Saisissez vos identifiants de connexion.
5. Si la double authentification est activée, saisissez le code demandé.
6. Dans le champ `Mot de passe d'accès à l'entreprise`, saisissez le nouveau mot de passe.
7. Cliquez sur `Enregistrer`.

Pour retirer le verrouillage de l'entreprise :

1. Dans INGENEO PRECOMPTA, ouvrez `Entreprises > Editer > Entreprise > Informations générales`.
2. Cliquez sur le sous-onglet `Sécurité`.
3. Cliquez sur `Supprimer`.
4. Saisissez vos identifiants de connexion.
5. Si la double authentification est activée, saisissez le code demandé.
6. Cliquez sur `Enregistrer`.

## Résultat attendu

Dans INGENEO PRECOMPTA, après un clic sur `Enregistrer` dans `Entreprises > Editer > Entreprise > Informations générales`, les modifications sont conservées pour l'entreprise.

* Après l'ajout d'un logo, le logo s'affiche à gauche de la ligne de l'entreprise, sur l'écran `Entreprises` et dans le menu `Bannettes`.
* Après la définition d'un `Mot de passe d'accès à l'entreprise`, l'entreprise affiche le badge `Sécurisé` dans la liste de l'écran `Entreprises`. Tous les utilisateurs doivent saisir ce mot de passe pour accéder à l'entreprise.
* Après la suppression du mot de passe, l'entreprise n'est plus verrouillée et le badge `Sécurisé` disparaît de la liste de l'écran `Entreprises`.

## Erreurs fréquentes

**Le menu `Informations générales` n'apparaît pas.** Dans INGENEO PRECOMPTA, le menu `Informations générales` d'une entreprise n'est visible qu'avec le droit `Autoriser l'accès au paramétrage des informations générales`. Demandez à un administrateur d'ajouter ce droit à votre profil. Le détail des droits est dans [Détail des droits](../administration/detail-des-droits.md).

**Les informations récupérées depuis la base SIRENE ont disparu.** Dans INGENEO PRECOMPTA, le bouton `Récupérer les informations de l'entreprise.` du champ `SIREN` et le lien `cliquer ici` du sous-onglet `Etablissements` n'enregistrent pas les valeurs récupérées. Après la récupération, cliquez sur `Enregistrer`.

**Aucune information n'est récupérée depuis la base SIRENE.** Dans INGENEO PRECOMPTA, la récupération ne fonctionne que si le SIREN figure dans l'annuaire des entreprises et que l'entreprise n'a pas masqué ses informations. Sinon, les champs vides restent vides et les valeurs déjà saisies sont conservées. Vérifiez le numéro du champ `SIREN`, ou saisissez les informations à la main.

**Le `Mode de facturation`, le logo ou les `Sites` ne changent pas après la récupération SIRENE.** Dans INGENEO PRECOMPTA, la récupération depuis la base SIRENE ne met pas à jour les champs `Mode de facturation`, `Logo de l'entreprise` et `Sites`. Modifiez-les à la main dans le sous-onglet `Siège`, puis cliquez sur `Enregistrer`.

**Le logo est refusé.** Dans INGENEO PRECOMPTA, le champ `Logo de l'entreprise` accepte les fichiers JPG ou PNG de 25 Mo maximum. Pour un autre format, le message `Le fichier n'est pas au bon format` s'affiche. Convertissez le logo en JPG ou en PNG, puis envoyez-le de nouveau.

## Fiches liées

* [Créer une entreprise](creer-une-entreprise.md) : création d'une entreprise, avant le paramétrage de ses informations générales.
* [Créer plusieurs entreprises en une fois par import](creer-une-entreprise-1.md) : création en masse, avant la vérification des informations de chaque entreprise.
* [Détail des droits](../administration/detail-des-droits.md) : droit `Autoriser l'accès au paramétrage des informations générales`.

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-modifier-informations-generales-entreprise-ingeneo-precompta
* titre : Comment modifier les informations générales et le mot de passe d'une entreprise dans INGENEO PRECOMPTA ?
* type : procedure
* module : Gestion des entreprises
* version\_outil : 2.10.4 (version observée)
* roles\_concernes : utilisateur avec le droit `Autoriser l'accès au paramétrage des informations générales`
* tags : informations générales, SIRENE, logo, sites, mot de passe, sécurité
* formulations\_utilisateur : « Comment mettre à jour le SIREN ou l'adresse d'une entreprise ? » ; « Comment ajouter le logo d'un dossier ? » ; « Comment mettre un code PIN sur une entreprise ? » ; « Pourquoi une entreprise est marquée Sécurisé ? » ; « Comment enlever le code PIN d'un dossier ? » ; « Synchroniser les infos avec l'INSEE »
* sources : Refonte de la page GitBook ingeneo-pre-compta/gestion-des-entreprises/parametrages-generaux ; observation de l'application INGENEO PRECOMPTA 2.10.4 (2026-10-14) ; réponses de l'expert 2026-10-14
* redacteur : AS
* relecteur :
* derniere\_verification : 2026-10-14
* statut : brouillon

</details>
