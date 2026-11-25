# Comment transférer une entreprise d'une autre PA vers la PA SEPTEO dans INGENEO PRECOMPTA ?

**Résumé :** Cette procédure permet de demander, dans INGENEO PRECOMPTA, le transfert des mailles d'adressage d'une entreprise de sa PA d'origine vers la PA SEPTEO, puis de suivre la demande.&#x20;

Elle se fait dans `Paramètres > Enrôlement PA` et nécessite un profil de site avec le droit `Autoriser l'accès au paramétrage de la facturation électronique.`.

## Objectif

Dans INGENEO PRECOMPTA, la Plateforme Agréée (PA) de l'annuaire peut refuser l'enrôlement d'une entreprise sur la PA SEPTEO. Ce refus se produit quand l'entreprise est déjà rattachée à une autre PA, appelée PA d'origine. L'onglet `Paramètres > Enrôlement PA > Enrôlements` affiche alors `Enrôlement refusé` avec le motif `Portabilité requise`.

La portabilité demande à la PA d'origine de transférer la réception des factures électroniques de l'entreprise vers la PA SEPTEO. Dans INGENEO PRECOMPTA, la demande de portabilité se fait entièrement dans l'application, sans ticket ni formulaire.

Dans INGENEO PRECOMPTA, la portabilité se fait en 4 temps, dans l'écran `Paramètres > Enrôlement PA`. Cet écran s'ouvre aussi par le lien `Mandat et enrôlement Plateforme Agréée (PA)` de l'en-tête.

| Temps                                    | Onglet de `Paramètres > Enrôlement PA` | Résultat                                              |
| ---------------------------------------- | -------------------------------------- | ----------------------------------------------------- |
| 1. Générer le mandat de portabilité      | `Informations et mandats`              | Un mandat PDF au statut `Brouillon`                   |
| 2. Faire signer le mandat de portabilité | `Informations et mandats`              | Un mandat au statut `Mandat signé`                    |
| 3. Lancer la demande de portabilité      | `Enrôlements`                          | Une demande au statut `Portabilité en attente`        |
| 4. Suivre la demande de portabilité      | `Portabilité`                          | Statut `Portabilité réussie` ou `Portabilité refusée` |

Dans INGENEO PRECOMPTA, générer le mandat de portabilité ne lance pas la demande de portabilité. La demande se lance séparément, depuis l'onglet `Enrôlements`.

Dans INGENEO PRECOMPTA, la colonne `Statut enrôlement` de l'onglet `Paramètres > Enrôlement PA > Enrôlements` affiche l'un de ces statuts : `Sans enrôlement`, `Enrôlement en cours`, `Enrôlement refusé`, `Enrôlement validé`, `Erreur lors de l'enrôlement`. Avec `Enrôlement refusé`, un motif s'affiche : `Portabilité requise`, `Indisponibilité annuaire` ou `Action nécessaire`.

## Prérequis

* **Droit :** dans INGENEO PRECOMPTA, l'utilisateur a un profil de site avec le droit `Autoriser l'accès au paramétrage de la facturation électronique.`.
* **Enrôlement :** dans `Paramètres > Enrôlement PA > Enrôlements`, l'enrôlement de l'entreprise est `Enrôlement refusé` avec le motif `Portabilité requise`.
* **Mandat initial :** l'entreprise a un mandat PA SEPTEO (mandat de facturation électronique), appelé mandat initial, avec un signataire cabinet renseigné. Le mandat de portabilité reprend les signataires du mandat initial.
* **SIREN :** le SIREN de l'entreprise est renseigné dans INGENEO PRECOMPTA.
* **Mandat de portabilité :** un mandat de portabilité est obligatoire pour toute demande de portabilité, même si le mandat PA SEPTEO est déjà signé. Il n'est pas demandé pour un enrôlement sans portabilité.

## Étapes

### Repérer l'entreprise à porter

1. Dans INGENEO PRECOMPTA, ouvrez `Paramètres > Enrôlement PA > Enrôlements`.
2. Recherchez l'entreprise.
3. Vérifiez que la ligne de l'entreprise affiche `Enrôlement refusé` avec le motif `Portabilité requise`.

Dans l'onglet `Enrôlements` d'INGENEO PRECOMPTA, la colonne `Actions` d'une entreprise en `Portabilité requise` affiche un bouton en forme de double flèche. Son infobulle indique `Initier une demande de portabilité`. Les autres actions de la ligne, comme `Voir`, restent disponibles.

| Situation de l'entreprise                                                                                        | État du bouton `Initier une demande de portabilité`                                  |
| ---------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------ |
| `Enrôlement refusé` avec `Portabilité requise`, aucune demande en cours                                          | Actif                                                                                |
| Demande `Portabilité en attente`, `Portabilité en cours`, `Inscription annuaire en cours` ou `Action nécessaire` | Grisé, avec l'infobulle `Une demande de portabilité existe déjà pour cet enrôlement` |
| Dernière demande `Portabilité réussie`                                                                           | Absent                                                                               |

### Générer le mandat de portabilité

Dans INGENEO PRECOMPTA, le mandat de portabilité est l'accord de l'entreprise et du cabinet pour changer de PA. C'est un document PDF intitulé « Accord formel de portabilité ».

1. Dans INGENEO PRECOMPTA, ouvrez `Paramètres > Enrôlement PA > Informations et mandats`.
2.  Sur la ligne de l'entreprise, cliquez sur l'action `Mandat de portabilité`.

    Cette action n'est proposée que pour une entreprise en `Portabilité requise`. Le panneau `Mandat de portabilité` s'ouvre.
3. Vérifiez les zones préremplies et non modifiables `Entreprise` (raison sociale, SIREN, adresse), `Nouvelle PA` (dénomination, SIREN et matricule de SEPTEO) et `PA d'origine` (dénomination, SIREN s'il est connu, matricule).
4. Dans `Date de prise d'effet`, vérifiez ou modifiez la date à partir de laquelle la PA SEPTEO reçoit les factures. La date proposée est J+1, le lendemain de la date du jour.
5. Dans `Mailles d'adressage concernées`, décochez les mailles d'adressage que vous ne voulez pas porter. Les mailles du rejet sont cochées par défaut. Gardez au moins une maille cochée.
6. Cliquez sur `Actualiser l'aperçu` pour afficher les informations reprises dans le mandat de portabilité.
7.  Cliquez sur `Générer le mandat`.

    Un message de confirmation s'affiche. Le bloc `Mandat en cours` apparaît en haut du panneau `Mandat de portabilité`, avec le statut `Brouillon`.

Dans le panneau `Mandat de portabilité` d'INGENEO PRECOMPTA, les types de mailles d'adressage possibles sont `SIREN`, `SIREN_SIRET` et `SIREN_SUFFIXE`.

Dans le panneau `Mandat de portabilité` d'INGENEO PRECOMPTA, une date antérieure à J+1 est refusée avec le message `La date de prise d'effet doit être au minimum égale à J+1.`. Si toutes les mailles sont décochées, `Actualiser l'aperçu` et `Générer le mandat` sont impossibles.

**Numéro de mandat :** dans INGENEO PRECOMPTA, le numéro du mandat de portabilité est créé automatiquement. Il suit le format `SIREN de l'entreprise_SIREN de SEPTEO_AAAAMMJJ_NN`. AAAAMMJJ est la date du jour ; NN numérote les mandats générés ce jour-là (01, 02…). Plusieurs mandats peuvent être générés le même jour : le panneau `Mandat de portabilité` affiche toujours le dernier. Notez ce numéro : le panneau `Demande de portabilité` le demande.

### Faire signer le mandat de portabilité

Dans INGENEO PRECOMPTA, le bloc `Mandat en cours` du panneau `Mandat de portabilité` affiche le numéro du mandat, la date de prise d'effet, la date d'envoi, la date de signature et un badge de statut. Les boutons proposés dépendent de ce statut.

| Statut du badge                                                  | Boutons disponibles                                                                                                                       |
| ---------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------- |
| `Brouillon` (mandat de portabilité généré)                       | `Consulter`, `Envoyer en signature`, `Signer par délégation` (si la fonction est activée sur votre environnement), `Déposer le PDF signé` |
| `A signer : client` ou `A signer : cabinet` (signature en cours) | `Consulter`, `Annuler la signature`                                                                                                       |
| `Mandat signé`                                                   | `Télécharger`                                                                                                                             |

**Contrôler le PDF :** dans le bloc `Mandat en cours`, cliquez sur `Consulter`. Le PDF du mandat de portabilité contient 7 zones : l'entreprise, la nouvelle PA, la date d'effet, les mailles d'adressage, l'ancienne PA, le numéro du mandat et la zone de signature.

Choisissez l'un des 3 modes de signature du mandat de portabilité.

**Signature électronique par l'entreprise et le cabinet**

1.  Dans le bloc `Mandat en cours` du panneau `Mandat de portabilité`, cliquez sur `Envoyer en signature`.

    Le mandat de portabilité part en signature électronique (Yousign) à l'entreprise et au cabinet. Le message `Mandat de portabilité envoyé en signature.` s'affiche. Le badge indique qui doit encore signer : `A signer : client` ou `A signer : cabinet`. Il passe à `Mandat signé` quand toutes les signatures sont reçues.

**Signature par délégation**

Dans INGENEO PRECOMPTA, le bouton `Signer par délégation` n'existe que si la fonction est activée sur votre environnement.

1.  Dans le bloc `Mandat en cours` du panneau `Mandat de portabilité`, cliquez sur `Signer par délégation`.

    Le mandat de portabilité est envoyé au cabinet seul. Dans le PDF, seule la signature du représentant du cabinet est demandée. Le message `Mandat de portabilité envoyé en signature au cabinet.` s'affiche.

**Dépôt d'un PDF déjà signé**

Si le mandat de portabilité a été signé en dehors d'INGENEO PRECOMPTA, déposez le PDF signé. Le dépôt n'accepte que les fichiers `.pdf`, et seulement sur un mandat au statut `Brouillon`.

1. Dans le bloc `Mandat en cours` du panneau `Mandat de portabilité`, cliquez sur `Déposer le PDF signé`.
2.  Sélectionnez le fichier PDF signé.

    Le message `Mandat de portabilité signé déposé avec succès.` s'affiche. Le mandat de portabilité passe à `Mandat signé`.

**Annuler une signature en cours**

1.  Dans le bloc `Mandat en cours`, si le statut est `A signer : client` ou `A signer : cabinet`, cliquez sur `Annuler la signature`.

    Le message `La signature du mandat de portabilité a été annulée.` s'affiche. Vous pouvez alors générer un nouveau mandat de portabilité. Si l'annulation échoue, un message invite à réessayer.

**Télécharger le mandat signé**

1.  Dans le bloc `Mandat en cours`, si le statut est `Mandat signé`, cliquez sur `Télécharger`.

    Le fichier s'appelle `mandat-portabilite_<numéro du mandat>.pdf`. Si le téléchargement est impossible, réessayez plus tard ou contactez le support SEPTEO.

### Lancer la demande de portabilité

1. Dans INGENEO PRECOMPTA, ouvrez `Paramètres > Enrôlement PA > Enrôlements`.
2.  Sur la ligne de l'entreprise, cliquez sur le bouton en forme de double flèche `Initier une demande de portabilité`.

    Le panneau `Demande de portabilité` s'ouvre, avec le sous-titre `Demander le transfert des mailles sélectionnées vers la PA SEPTEO`.
3. Vérifiez les blocs `Entreprise`, `Ancienne PA (issue du rejet)` et `Nouvelle PA`. Ils sont préremplis et non modifiables.
4. Vérifiez la `Date de prise d'effet`. Elle est proposée à J+1 et ne peut pas être antérieure à J+1.
5. Dans `Mailles d'adressage concernées`, décochez les mailles d'adressage que vous ne voulez pas porter. Les mailles du rejet sont cochées par défaut. Gardez au moins une maille cochée.
6. Dans le bloc `Confirmation du mandat`, saisissez le `Numéro de mandat` du mandat de portabilité. Le numéro n'accepte que des lettres, des chiffres, des tirets et des tirets bas.
7. Cochez la case `Je confirme être en possession d'un mandat de portabilité valide pour l'entreprise et les mailles concernées par cette demande.`.
8.  Cliquez sur `Valider la demande`. Ce bouton reste inactif tant que la case de confirmation n'est pas cochée.

    Le panneau `Demande de portabilité` se ferme. Le message `La demande de portabilité a bien été créée. Vous pouvez suivre son avancement dans l'onglet « Portabilité ».` s'affiche.

Dans INGENEO PRECOMPTA, le `Numéro de mandat` du panneau `Demande de portabilité` est saisi à la main. Il n'est pas relié automatiquement au mandat de portabilité généré. INGENEO PRECOMPTA ne contrôle ni l'existence de ce mandat, ni sa signature.

Après `Valider la demande`, SEPTEO transmet la demande de portabilité à la PA d'origine. L'utilisateur d'INGENEO PRECOMPTA n'a plus d'action à faire, sauf si la PA d'origine demande une confirmation complémentaire. Dans ce cas, confirmez à la PA d'origine le choix de rejoindre la PA SEPTEO.

**Délais de la portabilité vers la PA SEPTEO :**

* SEPTEO notifie la demande de portabilité à la PA d'origine dans un délai maximum de 2 jours ouvrés.
* La PA d'origine dispose ensuite de 5 jours ouvrés pour répondre.
* Si la PA d'origine accepte, elle envoie à la PA SEPTEO une clé de transfert de maille (token).
* Après réception du token, SEPTEO réalise la migration technique. Sa durée est variable.

## Résultat attendu

### Liste des demandes de portabilité

Dans INGENEO PRECOMPTA, l'onglet `Paramètres > Enrôlement PA > Portabilité` affiche une ligne par demande de portabilité. Il s'ouvre directement, sans passer par l'onglet `Enrôlements`. Une entreprise en `Portabilité requise` sans demande lancée n'y apparaît pas.

| Colonne de l'onglet `Portabilité` | Contenu                                                                |
| --------------------------------- | ---------------------------------------------------------------------- |
| `Code`                            | Code dossier de l'entreprise                                           |
| `Entreprise`                      | Raison sociale et SIREN                                                |
| `Site`                            | Site de l'entreprise                                                   |
| `Statut portabilité`              | Statut global de la demande ; le survol du badge affiche sa définition |
| `Date d'envoi`                    | Date d'envoi de la demande à la PA d'origine                           |
| `Actions`                         | Icône en forme d'œil `Consulter la demande de portabilité`             |

Dans l'onglet `Portabilité` d'INGENEO PRECOMPTA, la recherche accepte un code dossier, une raison sociale ou un SIREN. Le bouton `Filtres` propose `Statut portabilité` (sélection multiple), `Site` (sélection multiple) et `Date d'envoi` (du / au). Le bouton de réinitialisation affiche de nouveau la liste complète. L'onglet `Enrôlements` propose aussi un filtre par statut de portabilité.

### Détail d'une demande de portabilité

Dans l'onglet `Paramètres > Enrôlement PA > Portabilité` d'INGENEO PRECOMPTA, l'icône en forme d'œil d'une ligne ouvre un panneau à droite, en lecture seule. La liste reste visible derrière. Le panneau affiche :

* `Informations de l'entreprise` : code, dénomination, SIREN, adresse, code postal, ville, région, site ;
* `Informations de la portabilité` : PA d'origine et son matricule, PA de destination, date de la demande, date de prise d'effet demandée, `Statut global de la portabilité` ;
* selon le cas, le motif du refus communiqué par la PA d'origine, ou le motif `Action nécessaire` ;
* `Suivi de la portabilité des mailles` : une ligne par maille d'adressage, avec son type, son identifiant, la date de demande, la date d'effet, son statut et sa dernière mise à jour.

Dans INGENEO PRECOMPTA, chaque maille d'adressage d'une demande de portabilité est suivie séparément. Une même demande peut contenir des mailles aux statuts différents. Dépliez une maille pour afficher sa chronologie.

| Étape de la chronologie d'une maille                           | Signification                                                                                                                                         |
| -------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Demande envoyée à la PA`                                      | La demande de portabilité est partie chez la PA d'origine.                                                                                            |
| `Acceptée par la PA d'origine` / `Refusée par la PA d'origine` | Réponse de la PA d'origine, avec le motif en cas de refus.                                                                                            |
| `Traitement en cours`                                          | La migration de la maille d'adressage est en cours.                                                                                                   |
| `Inscription annuaire en cours`                                | La migration est traitée ; l'activation de la maille dans l'annuaire est attendue.                                                                    |
| `Contrôle annuaire prévu (J+15)`                               | Étape à venir, affichée différemment des étapes faites. La date est indicative : aucun contrôle automatique de l'annuaire n'est réalisé à cette date. |
| `Portabilité réussie`                                          | La maille d'adressage est portée.                                                                                                                     |

Sous la chronologie d'une maille, le panneau de détail peut aussi afficher `Motif du refus`, `Action nécessaire` (avec la date de l'anomalie) et `Prochaine étape`.

### Statuts d'une demande de portabilité

| Statut                          | Définition affichée dans l'infobulle du badge                                                                 |
| ------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| `Portabilité en attente`        | En attente d'acceptation de la plateforme agréée actuelle                                                     |
| `Portabilité refusée`           | Refus motivé de la plateforme agréée actuelle                                                                 |
| `Portabilité en cours`          | Accord reçu et migration en cours                                                                             |
| `Inscription annuaire en cours` | Migration traitée, en attente d'activation des mailles dans l'annuaire                                        |
| `Portabilité réussie`           | Migration réalisée ; l'infobulle mentionne aussi la relance de l'enrôlement, qui n'est pas encore automatique |
| `Action nécessaire`             | Une anomalie empêche la poursuite automatique du traitement                                                   |

Dans INGENEO PRECOMPTA, le statut global d'une demande de portabilité se calcule à partir du statut de ses mailles d'adressage. Les règles s'appliquent dans cet ordre :

1. Si une maille est en `Action nécessaire`, ou si la PA d'origine a accepté certaines mailles et refusé d'autres, le statut global est `Action nécessaire`.
2. Si toutes les mailles sont refusées, le statut global est `Portabilité refusée`.
3. Si toutes les mailles sont réussies, le statut global est `Portabilité réussie`.
4. Sinon, le statut global est celui de la maille la moins avancée, dans cet ordre : `Portabilité en attente`, `Portabilité en cours`, `Inscription annuaire en cours`.

Exemple : une demande de 3 mailles, dont 1 réussie et 2 en `Inscription annuaire en cours`, reste en `Inscription annuaire en cours`. Une demande dont une maille est refusée et l'autre sans réponse reste en `Portabilité en attente`.

Dans INGENEO PRECOMPTA, le statut affiché dans l'onglet `Portabilité` est le dernier statut connu. Il se met à jour avec un décalage après le changement chez SEPTEO. Rechargez la page avant de conclure qu'un statut est bloqué.

## Erreurs fréquentes

**L'enrôlement sur la PA SEPTEO est refusé car la maille d'adressage est déjà assignée à une autre PA.** Dans INGENEO PRECOMPTA, la raison du rejet est du type `Raison du rejet de votre demande d'enrôlement : La maille d'adressage SIRENXXX chevauche une maille déjà existante assignée à la PA : XXX (Matricule : 00xx), qui a enregistré cette maille pour la période du 09/10/2026 au 31/12/9999.`. Le SIREN, le nom et le matricule de la PA d'origine et les dates varient selon l'entreprise. Solution : si l'enrôlement affiche le motif `Portabilité requise`, lancez une demande de portabilité depuis `Paramètres > Enrôlement PA > Enrôlements`.

**Le bouton `Initier une demande de portabilité` n'apparaît pas ou est grisé.** Dans l'onglet `Paramètres > Enrôlement PA > Enrôlements` d'INGENEO PRECOMPTA, le bouton en forme de double flèche n'apparaît que pour une entreprise en `Enrôlement refusé` avec le motif `Portabilité requise`. Il est grisé si une demande est déjà active, et masqué si la dernière demande a réussi.

**Le panneau `Mandat de portabilité` refuse de générer le mandat.** Dans INGENEO PRECOMPTA, un message orange explique la cause :

| Message                                                                                                     | Solution                                                                                                          |
| ----------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------- |
| `Le mandat de portabilité n'est disponible que pour un enrôlement refusé en « Portabilité requise ».`       | Vérifiez le statut de l'entreprise dans l'onglet `Enrôlements`.                                                   |
| `Aucun mandat initial n'est disponible pour reprendre les signataires.`                                     | Créez d'abord le mandat PA SEPTEO (mandat de facturation électronique) de l'entreprise.                           |
| `Le mandat initial n'a pas de signataire cabinet : complétez-le avant de générer le mandat de portabilité.` | Renseignez le signataire cabinet sur le mandat initial.                                                           |
| `Le SIREN de l'entreprise est obligatoire pour générer le mandat.`                                          | Renseignez le SIREN de l'entreprise.                                                                              |
| `La PA d'origine est inconnue : relancez l'enrôlement pour la récupérer.`                                   | Relancez l'enrôlement. Si le message revient, contactez le support SEPTEO.                                        |
| `Un mandat de portabilité est en cours de signature : annulez la signature avant d'en générer un nouveau.`  | Cliquez sur `Annuler la signature` dans le bloc `Mandat en cours`, puis générez un nouveau mandat de portabilité. |

**Le bouton `Télécharger` est absent du bloc `Mandat en cours`.** Dans INGENEO PRECOMPTA, `Télécharger` n'existe que pour un mandat de portabilité au statut `Mandat signé`. Aux statuts `Brouillon`, `A signer : client` ou `A signer : cabinet`, utilisez `Consulter` pour ouvrir le PDF.

**L'action `Mandat de portabilité` reste proposée alors qu'une demande est en cours.** Dans l'onglet `Informations et mandats` d'INGENEO PRECOMPTA, l'action `Mandat de portabilité` reste proposée même quand une demande de portabilité est déjà en cours. C'est le comportement actuel.

**Le panneau `Demande de portabilité` refuse de créer la demande.** Dans INGENEO PRECOMPTA, un message indique la cause :

| Message                                                                                                                          | Signification et solution                                                                                                                                                                       |
| -------------------------------------------------------------------------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| `Aucune demande de portabilité ne peut être lancée pour cet enrôlement.`                                                         | L'enrôlement n'est plus en `Portabilité requise`.                                                                                                                                               |
| `Une demande de portabilité est déjà en cours pour cet enrôlement.`                                                              | Une demande active existe déjà. Suivez-la dans l'onglet `Portabilité`.                                                                                                                          |
| `La plateforme agréée actuelle n'a pas pu être identifiée depuis le motif de refus. Veuillez contacter le support.`              | La PA d'origine est introuvable dans le motif de refus. Contactez le support SEPTEO.                                                                                                            |
| `Les mailles d'adressage de l'enrôlement ne correspondent pas à celles connues de la plateforme. Veuillez contacter le support.` | Contactez le support SEPTEO.                                                                                                                                                                    |
| `Impossible de lancer la demande de portabilité, veuillez réessayer ultérieurement.`                                             | Message générique : problème temporaire ou donnée refusée par la plateforme, par exemple un matricule de PA inconnu. Réessayez plus tard ; si le message persiste, contactez le support SEPTEO. |

**La PA d'origine refuse la portabilité.** Dans INGENEO PRECOMPTA, la demande passe en `Portabilité refusée`. Le détail de la demande, dans l'onglet `Portabilité`, affiche le motif du refus communiqué par la PA d'origine. Chaque maille indique `Refusée par la PA d'origine`, avec la date et le motif. Si la PA d'origine conteste le choix de l'entreprise, confirmez-lui le choix de rejoindre la PA SEPTEO ; ce cas allonge le délai de la portabilité.

**La PA d'origine refuse sans donner de motif.** Dans INGENEO PRECOMPTA, la demande passe en `Action nécessaire` avec le motif `Motif de refus non renseigné par la PA d'origine.`. Contactez le support SEPTEO avec le code dossier de l'entreprise et le motif affiché.

**La PA d'origine accepte certaines mailles et en refuse d'autres.** Dans INGENEO PRECOMPTA, la demande passe en `Action nécessaire` avec le motif `Réponse PA partielle : mailles acceptées et refusées.`. Chaque maille garde son statut : les mailles acceptées avancent, la maille refusée reste en `Portabilité refusée`.

**Une demande de portabilité est en `Action nécessaire`.** Dans INGENEO PRECOMPTA, une anomalie bloque le traitement automatique. Le motif s'affiche dans le détail de la demande, dans l'onglet `Portabilité`. Exemples : `Adresse email de portabilité non renseignée.`, `PA d'origine inactive dans le référentiel.`, `Traitement de la migration en anomalie.`. Une maille acceptée par la PA d'origine sans identifiant de migration passe aussi en `Action nécessaire`. Ces anomalies ne se corrigent pas dans INGENEO PRECOMPTA : contactez le support SEPTEO avec le code dossier de l'entreprise et le motif affiché. Pendant ce temps, le bouton `Initier une demande de portabilité` reste grisé.

**La demande reste en `Portabilité en attente` plusieurs jours.** Dans INGENEO PRECOMPTA, la PA d'origine n'a pas encore répondu, ou sa réponse n'a pas encore été enregistrée. La PA d'origine dispose de 5 jours ouvrés pour répondre. Sans clé de transfert de maille (token), SEPTEO ne peut pas réaliser le transfert ; SEPTEO attend le token et relance la PA d'origine, sans relance automatique. L'entreprise n'est pas notifiée de ce retard. Rechargez la page, puis contactez le support SEPTEO avec le code dossier de l'entreprise.

**La PA d'origine exige une validation explicite de l'entreprise.** Cette validation ajoute un délai à la portabilité vers la PA SEPTEO. Solution : répondez à la demande de confirmation de la PA d'origine.

**Le statut de la demande ne change pas.** Dans l'onglet `Portabilité` d'INGENEO PRECOMPTA, les statuts se mettent à jour avec un décalage. Rechargez la page, puis rouvrez le détail de la demande.

**L'entreprise est en `Portabilité réussie` mais reste `Enrôlement refusé`.** Dans INGENEO PRECOMPTA, c'est le comportement actuel : la relance de l'enrôlement après portabilité n'est pas encore livrée.

**Une demande de portabilité a été lancée par erreur.** INGENEO PRECOMPTA ne propose aucune action de suppression ni d'annulation d'une demande transmise. La demande reste dans l'historique de l'onglet `Portabilité`. Contactez le support SEPTEO.

## Fiches liées

* [Comment faire passer une entreprise de la PA SEPTEO à une autre Plateforme Agréée dans INGENEO ?](comment-transferer-une-entreprise-de-la-pa-septeo-a-une-autre-pa.md) : portabilité dans le sens inverse
* [Qu'est-ce que la suppression du rattachement à la PA SEPTEO en cas de cessation d'activité dans INGENEO ?](quimplique-la-cessation-dactivite-dune-entreprise.md) : fin du rattachement sans portabilité

<details>

<summary>Métadonnées de la fiche</summary>

* id : proc-portabilite-vers-pa-septeo-ingeneo-precompta
* titre : Comment transférer une entreprise d'une autre PA vers la PA SEPTEO dans INGENEO PRECOMPTA ?
* titre\_menu : Transférer une entreprise vers la PA SEPTEO
* type : procedure
* module : Facturation électronique
* version\_outil : toutes
* roles\_concernes : utilisateur avec un profil de site portant le droit `Autoriser l'accès au paramétrage de la facturation électronique.`
* tags : plateforme agréée, PA SEPTEO, portabilité, mandat de portabilité, mailles d'adressage, portabilité requise
* formulations\_utilisateur : « un client est enrôlé sur une autre PA » ; « comment changer de PA pour la PA SEPTEO ? » ; « comment faire si un client a déjà souscrit à une PA ? » ; « que faire lorsqu'il y a un message Portabilité requise »
* sources : Refonte de la page GitBook enrolement-and-mandats/cote-cabinet/procedure-de-portabilite-cabinet-dexpertise-comptable/comment-transferer-une-entreprise-dune-autre-pa-vers-la-pa-septeo ; guide utilisateur « Portabilité entrante » (documentation technique) ; réponses de l'expert 2026-11-13
* redacteur : CH
* relecteur :
* derniere\_verification : 2026-11-13
* statut : brouillon

</details>
