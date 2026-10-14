---
description: >-
  Cette procédure permet de rattacher à la PA SEPTEO une entreprise rattachée à
  une autre Plateforme Agréée (PA). Elle s'applique dans INGENEO ENTREPRISE,
  INGENEO PRECOMPTA et INGENEO COMPTA. Les délais
---

# Comment transférer une entreprise d'une autre PA vers la PA SEPTEO ?

## Objectif

Cette procédure s'applique quand une entreprise ne peut pas être activée sur la PA SEPTEO parce qu'elle est rattachée à une autre Plateforme Agréée (PA). SEPTEO demande alors la portabilité des mailles d'adressage de l'entreprise auprès de la PA d'origine. La procédure est identique dans INGENEO ENTREPRISE, INGENEO PRECOMPTA et INGENEO COMPTA.

## Prérequis

* L'entreprise est rattachée à une Plateforme Agréée (PA) autre que la PA SEPTEO.
* Le mandat PA SEPTEO est signé et déposé par l'entreprise ou par son mandataire dans le logiciel INGENEO.
* Dans les logiciels INGENEO, la création d'un mandat ou d'un enrôlement nécessite le rôle `Administrateur`.
* Si le mandat PA SEPTEO est déjà signé et déposé, aucune nouvelle signature n'est nécessaire pour la portabilité.
* Pour chaque entreprise, préparez les informations suivantes : raison sociale, SIREN, NIC, mailles d'adressage concernées par la portabilité, PA d'origine, date de prise d'effet, email de suivi de la demande (client ou cabinet), nom du partenaire PA SEPTEO (cabinet, entreprise ou partenaire), date de signature du mandat PA SEPTEO.

## Étapes

1. Ouvrez l'écran des mandats et enrôlements de votre logiciel INGENEO :
   * dans INGENEO PRECOMPTA : `Paramètres > Enrôlement PA > Informations et mandats` ;
   * dans INGENEO ENTREPRISE : `Facturation électronique` ;
   * dans INGENEO COMPTA : `Sociétés gérées > Administration`.
2. Vérifiez que le mandat PA SEPTEO de l'entreprise est signé et déposé.
3. Si le mandat PA SEPTEO n'est pas signé, signez-le puis déposez-le dans l'écran des mandats et enrôlements de votre logiciel INGENEO.
4. Transmettez à SEPTEO, par ticket ou par le formulaire https://forms.monday.com/forms/05f83050230c7fdf34dfde4fe33f716e?r=euc1, la liste des entreprises concernées. Pour chaque entreprise, indiquez : raison sociale, SIREN, NIC, mailles d'adressage concernées par la portabilité, PA d'origine, date de prise d'effet, email de suivi de la demande, nom du partenaire PA SEPTEO, date de signature du mandat PA SEPTEO.
5. Si la PA d'origine vous demande une confirmation complémentaire, confirmez-lui votre choix de rejoindre la PA SEPTEO.

La demande explicite par ticket, ou le formulaire rempli, vaut accord pour lancer la portabilité vers la PA SEPTEO. Après réception de cette demande, la portabilité se déroule ainsi :

* SEPTEO notifie la demande de portabilité à la PA d'origine dans un délai maximum de 2 jours ouvrés.
* La PA d'origine dispose ensuite de 5 jours ouvrés pour répondre à la demande.
* Si la PA d'origine accepte, elle envoie à la PA SEPTEO une clé de transfert de maille (token).
* Après réception du token, SEPTEO réalise la migration technique. Sa durée est variable.
* La demande est traitée par l'équipe Portabilité de l'équipe Produit (service R\&D) de SEPTEO. Le Support SEPTEO assure le suivi de la demande.

## Résultat attendu

Dans INGENEO PRECOMPTA, écran `Paramètres > Enrôlement PA > Enrôlements`, la colonne `Statut enrôlement` affiche l'état de l'enrôlement de l'entreprise. Les statuts possibles sont `Sans enrôlement`, `Enrôlement en cours`, `Enrôlement refusé`, `Enrôlement validé` et `Erreur lors de l'enrôlement`. Avec le statut `Enrôlement refusé`, un motif de refus s'affiche : `Portabilité requise`, `Indisponibilité annuaire` ou `Action nécessaire`.

Une fois la portabilité finalisée, l'entreprise est automatiquement rattachée à la PA SEPTEO. Dans INGENEO PRECOMPTA, la colonne `Statut enrôlement` affiche alors `Enrôlement validé`. Dans le menu `Facturation électronique`, la colonne `Enrôlement` de la maille d'adressage indique `PA Septeo`.

## Erreurs fréquentes

* **L'enrôlement sur la PA SEPTEO est refusé car la maille d'adressage est déjà assignée à une autre PA.** La raison du rejet est du type : `Raison du rejet de votre demande d'enrôlement : La maille d'adressage SIRENXXX chevauche une maille déjà existante assignée à la PA : XXX (Matricule : 00xx), qui a enregistré cette maille pour la période du 09/10/2026 au 31/12/9999.` Le SIREN, le nom et le matricule de la PA d'origine et les dates varient selon l'entreprise. Dans INGENEO PRECOMPTA, colonne `Statut enrôlement`, ce refus s'affiche `Enrôlement refusé` avec le motif `Portabilité requise` ou `Action nécessaire`. Cause : la maille d'adressage est déjà assignée à une autre Plateforme Agréée (PA). Solution : demandez à SEPTEO la portabilité vers la PA SEPTEO par ticket ou par formulaire.
* **La PA d'origine ne répond pas dans les 5 jours ouvrés.** Cause : la PA d'origine ne respecte pas le délai réglementaire de réponse. Sans clé de transfert de maille (token), SEPTEO ne peut pas réaliser le transfert vers la PA SEPTEO. SEPTEO attend le token et relance la PA d'origine, sans relance automatique. L'entreprise n'est pas notifiée de ce retard. Pour connaître l'avancement, contactez le Support SEPTEO.
* **La PA d'origine refuse ou conteste la portabilité vers la PA SEPTEO.** L'entreprise ou son mandataire en est informé. La PA d'origine peut contacter l'entreprise par l'email de suivi fourni dans la demande. Solution : confirmez à la PA d'origine le choix de rejoindre la PA SEPTEO. Ce cas allonge le délai de la portabilité.
* **La PA d'origine exige une validation explicite de l'entreprise.** Cette validation ajoute un délai à la portabilité vers la PA SEPTEO. Solution : répondez à la demande de confirmation de la PA d'origine.

## Fiches liées

* [Comment faire passer une entreprise de la PA SEPTEO à une autre Plateforme Agréée dans INGENEO ?](comment-transferer-une-entreprise-de-la-pa-septeo-a-une-autre-pa.md) : portabilité dans le sens inverse
* [Qu'est-ce que la suppression du rattachement à la PA SEPTEO en cas de cessation d'activité dans INGENEO ?](quimplique-la-cessation-dactivite-dune-entreprise.md) : fin du rattachement sans portabilité

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-portabilite-vers-pa-septeo
* type : procedure
* module : Facturation électronique
* version\_outil : toutes
* roles\_concernes : entreprise, mandataire
* tags : plateforme agréée, PA SEPTEO, portabilité, mailles d'adressage, mandat, portabilité requise
* formulations\_utilisateur : « un client est enrôlé sur une autre PA » ; « comment changer de PA pour la PA SEPTEO ? » ; « comment faire si un client a déjà souscrit à une PA ? » ; « que faire lorsqu'il y a un message Portabilité requise »
* sources : procédure écrite gestion des changements de PA, réponses expert 2026-10-13
* redacteur : SL
* relecteur :
* derniere\_verification : 2026-10-13
* statut : en\_relecture

</details>
