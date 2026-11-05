# Crédits-bails

{% hint style="info" %}
**Où le trouver :** Menu **Fiches › Crédits-bails**
{% endhint %}

{% hint style="success" %}
**En bref** — Cet écran gère les crédits-bails du dossier : la fiche décrit le contrat (bien, durée, loyers, assurance, option d'achat), et le logiciel calcule l'échéancier des loyers et les comptabilise.

* Pour créer un crédit-bail : bouton \[Ajouter un crédit-bail], renseignez la nature, les caractéristiques et les loyers, puis bouton \[Enregistrer].
* Pour comptabiliser les frais et les loyers d'une période : bouton \[Comptabilisation manuelle], puis bouton \[Valider].
* Pour lever l'option d'achat : bouton \[Transfert en immobilisation], puis enregistrez la fiche immobilisation préremplie.
{% endhint %}

Cette option permet de gérer tous les crédits-bails du dossier, ceux en cours comme ceux déjà transférés en immobilisations. Une fiche de crédit-bail décrit le contrat de location avec option d'achat tel que l'organisme vous l'a consenti : le bien financé, la durée, les loyers, l'assurance et le montant de l'option d'achat. À partir de ces informations, le logiciel calcule l'échéancier des loyers, sait comptabiliser les frais puis chaque échéance, et vous permet le jour venu de transférer le bien en immobilisation.

<figure><img src="../../.gitbook/assets/15-cm816.jpg" alt="Écran Crédits-bails"><figcaption><p>Écran « Crédits-bails » de la nouvelle interface</p></figcaption></figure>

Un sélecteur au-dessus de la grille permet de filtrer la liste selon le statut du crédit-bail.

## La liste des crédits-bails

**Statuts** : ce sélecteur, au-dessus de la grille, propose « Tous » (valeur par défaut), « Crédits-bails en cours » et « Crédits-bails transférés en immobilisations ».

La grille présente quatre colonnes : **Code** (colonne sur laquelle la liste est triée à l'ouverture, dans l'ordre croissant), **Libellé**, **Montant du bien HT** et **Date de début**. Toutes sont triables. Ne vous étonnez pas si l'en-tête de la troisième colonne s'affiche tronqué en « Montant du bien » : la largeur allouée ne suffit pas au libellé complet.

Vous pouvez cocher plusieurs lignes, y compris au-delà de la page affichée, puis employer le bouton **\[Supprimer]** de la barre basse pour supprimer la sélection en une fois.

## Bouton \[Ajouter un crédit-bail]

Il ouvre une fiche de crédit-bail vide. La fiche s'organise en rubriques, décrites ci-dessous dans l'ordre où elles s'affichent. Deux d'entre elles n'apparaissent que selon la nature du bien financé.

## Rubrique « Informations générales »

<figure><img src="../../.gitbook/assets/15-cm816-11-informations-generales.png" alt="Crédits-bails, Rubrique « Informations générales »"><figcaption><p>Rubrique « Informations générales »</p></figcaption></figure>

| Champ                                                                  | Ce qu'il faut savoir                                                                                                                                                                                                                                                                                                                                                                                      |
| ---------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>1. <strong>Code du crédit-bail</strong><br><em>Obligatoire</em></p> | 20 caractères au maximum. Il doit être unique ; si vous reprenez un code déjà employé, le logiciel refuse l'enregistrement en indiquant que le code est déjà utilisé et vous demande d'en choisir un autre. Seules les lettres, les chiffres, le tiret, le souligné et le point sont admis. **Le code n'est plus modifiable après le premier enregistrement** : en modification, il s'affiche verrouillé. |
| <p>2. <strong>Libellé</strong><br><em>Obligatoire</em></p>             | 50 caractères au maximum.                                                                                                                                                                                                                                                                                                                                                                                 |
| 3. **Nature**                                                          | Trois choix, « Autres » (valeur par défaut), « Immeuble » et « Véhicule ». Ce choix commande l'affichage des deux rubriques complémentaires décrites ci-dessous : c'est donc la première chose à renseigner. **La nature n'est plus modifiable après le premier enregistrement** ; les boutons s'affichent alors inactifs.                                                                                |
| 4. **Compte fournisseur**                                              | C'est le compte de l'organisme de crédit-bail. Vous pouvez saisir directement le numéro, ou taper quelques caractères pour laisser le logiciel vous proposer les comptes correspondants. La ligne comporte un bouton **\[+]** qui crée le compte s'il n'existe pas encore, et une loupe qui ouvre la recherche.                                                                                           |
| 5. **Code fournisseur**                                                | 20 caractères au maximum.                                                                                                                                                                                                                                                                                                                                                                                 |
| 6. **Nom fournisseur**                                                 | 40 caractères au maximum.                                                                                                                                                                                                                                                                                                                                                                                 |
| <p>7. <strong>Montant HT du bien</strong><br><em>Obligatoire</em></p>  | C'est la valeur du bien pris en crédit-bail.                                                                                                                                                                                                                                                                                                                                                              |
| 8. **Montant de TVA**                                                  | —                                                                                                                                                                                                                                                                                                                                                                                                         |
| 9. **Montant TTC du bien**                                             | Calculé automatiquement, non modifiable.                                                                                                                                                                                                                                                                                                                                                                  |
| 10. **Coût global HT**                                                 | Calculé automatiquement, non modifiable. Il correspond au total des loyers HT augmenté des frais HT.                                                                                                                                                                                                                                                                                                      |

## Rubrique « Informations complémentaires du véhicule »

Cette rubrique n'apparaît que si la nature retenue est « Véhicule ». Elle sert à renseigner ce que la taxe sur les véhicules de société exige de connaître ; la plupart des champs se lisent directement sur la carte grise, et leur infobulle vous indique dans quelle rubrique de celle-ci les trouver.

| Champ                                                             | Ce qu'il faut savoir                                                                                                                                                                                                                                                                     |
| ----------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p><strong>Immatriculation</strong><br><em>Obligatoire</em></p>   | 9 caractères au maximum — rubrique A de la carte grise. À la création, l'immatriculation doit être unique : le logiciel refuse un véhicule déjà connu du dossier.                                                                                                                        |
| **Modèle**                                                        | 40 caractères au maximum — rubriques D.1 et D.3 de la carte grise.                                                                                                                                                                                                                       |
| **Date de première immatriculation en France**                    | — rubrique B de la carte grise.                                                                                                                                                                                                                                                          |
| **Emission CO2**                                                  | En gramme par kilomètre — rubrique V.7 de la carte grise.                                                                                                                                                                                                                                |
| <p><strong>Type de véhicule</strong><br><em>Obligatoire</em></p>  | — rubrique J.1 de la carte grise. Quatre choix : « Véhicule de tourisme » (valeur par défaut), « Véhicule utilitaire », « Moto » et « Vélomoteur, scooter ».                                                                                                                             |
| <p><strong>Norme euro</strong><br><em>Obligatoire</em></p>        | — rubrique V.9 de la carte grise. Le sélecteur affiche « Sélectionnez » tant que vous n'avez pas choisi, et propose les normes de EURO 1 à EURO 6d-TEMP puis de EURO 0 à EURO VI.                                                                                                        |
| <p><strong>Puissance fiscale</strong><br><em>Obligatoire</em></p> | De 1 à 99 — rubrique P.6 de la carte grise.                                                                                                                                                                                                                                              |
| <p><strong>Motorisation</strong><br><em>Obligatoire</em></p>      | Quatre choix : « Thermique », « Hydrogène », « Hybride » et « Electrique ». **Aucune valeur n'est présélectionnée** : vous devez impérativement en choisir une, sans quoi l'enregistrement est refusé.                                                                                   |
| <p><strong>Type de carburant</strong><br><em>Obligatoire</em></p> | Il ne s'affiche, et ne devient obligatoire, que pour les motorisations « Thermique » et « Hybride ». Quatre choix, sans présélection : « Diesel », « Super sans plomb », « Superéthanol E85 » et « GPL ». Pour les motorisations « Electrique » et « Hydrogène », le champ n'existe pas. |
| **Motif d'exonération sur le CO2**                                | Saisie libre.                                                                                                                                                                                                                                                                            |
| **Motif d'exonération sur les polluants**                         | Saisie libre.                                                                                                                                                                                                                                                                            |

## Rubrique « Informations complémentaires de l'immeuble »

<figure><img src="../../.gitbook/assets/15-cm816-23-informations-complementaires-de-l-immeuble.png" alt="Crédits-bails, Rubrique « Informations complémentaires de l&#x27;immeuble »"><figcaption><p>Rubrique « Informations complémentaires de l'immeuble »</p></figcaption></figure>

Cette rubrique n'apparaît que si la nature retenue est « Immeuble ». Elle renseigne les informations que la liasse fiscale attend d'un immeuble.

| Champ                                                               | Ce qu'il faut savoir                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| ------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1. **Adresse**                                                      | Un seul libellé, mais trois lignes de saisie, de 38 caractères chacune.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| 2. **Commune**                                                      | Saisissez le début de son nom : la zone propose des communes sous la forme « code - nom (département) », par exemple « 109 - Nantes (44) » ; la loupe placée à droite de la zone ouvre un panneau « Sélection d'une commune », dont la liste (Code INSEE, Ville, Département) se filtre par nom ou par code INSEE. **Code postal :** et **Ville :** sont en lecture seule (« Déduit de la commune ») : ils se remplissent d'après la commune choisie ; quand la commune compte plusieurs codes postaux (Nantes, par exemple), le code postal devient une liste « Sélectionnez » où vous choisissez le vôtre. **Pays :** « FRANCE » est proposé à l'ouverture. |
| <p>3. <strong>Nombre de locaux</strong><br><em>Obligatoire</em></p> | De 1 à 999. La valeur 1 est proposée par défaut.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                              |
| 4. **Dispositif de déduction spécifique**                           | Le sélecteur propose « Aucun » par défaut, puis les dispositifs de déduction des revenus fonciers : « Besson ancien », les variantes « Scellier », les conventionnements ANAH — Borloo ancien, secteur intermédiaire, social ou très social, puis les conventionnements Cosse avec leur taux de déduction.                                                                                                                                                                                                                                                                                                                                                    |
| 5. **Dispositif de déduction au titre de l'amortissement**          | Le sélecteur propose « Aucun » par défaut, puis « Périssol », « Robien classique », « Robien classique en zone de revitalisation rurale », « Robien recentré », « Robien recentré en zone de revitalisation rurale », « Borloo neuf » et « Besson neuf ».                                                                                                                                                                                                                                                                                                                                                                                                     |
| 6. **Nature de l'immeuble**                                         | À la saisie mais nécessaire à l'enregistrement. Sept choix : « Immeuble urbain » (valeur par défaut), « Immeuble rural », « Immeuble de rapport », « Appartement », « Maison », « Parking » et « Autre qualification ».                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| 7. **Etat de l'immeuble**                                           | Deux choix, « Bâti » (valeur par défaut) et « Non bâti ».                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

## Rubrique « Caractéristiques du crédit-bail »

<figure><img src="../../.gitbook/assets/15-cm816-12-caracteristiques-du-credit-bail.png" alt="Crédits-bails, Rubrique « Caractéristiques du crédit-bail »"><figcaption><p>Rubrique « Caractéristiques du crédit-bail »</p></figcaption></figure>

C'est la rubrique qui commande le calcul de l'échéancier.

| Champ                                                                 | Ce qu'il faut savoir                                                                                                                                                                                |
| --------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>1. <strong>Date de début</strong><br><em>Obligatoire</em></p>      | Un pictogramme de calendrier vous permet de la choisir.                                                                                                                                             |
| 2. **Périodicité**                                                    | Vous avez le choix entre « Mensuelle » (valeur par défaut), « Trimestrielle » et « Annuelle ». La périodicité semestrielle, disponible sur les emprunts, n'est pas proposée pour les crédits-bails. |
| <p>3. <strong>Nombre d'échéances</strong><br><em>Obligatoire</em></p> | De 1 à 999. Renseignez-le tôt : plusieurs contrôles de la fiche en dépendent.                                                                                                                       |
| 4. **Date de dernière échéance**                                      | Non modifiable. Elle est calculée automatiquement à partir de la date de début, de la périodicité et du nombre d'échéances.                                                                         |
| 5. **Type d'échéances**                                               | Choisissez entre « A échoir » et « Echues » ; la valeur retenue par défaut est **« A échoir »**.                                                                                                    |

## Rubrique « Loyers »

<figure><img src="../../.gitbook/assets/15-cm816-13-loyers.png" alt="Crédits-bails, Rubrique « Loyers »"><figcaption><p>Rubrique « Loyers »</p></figcaption></figure>

| Champ                                                       | Ce qu'il faut savoir                                                                                                                                                                                                                          |
| ----------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>1. <strong>Loyer HT</strong><br><em>Obligatoire</em></p> | Entrez le montant de chaque échéance.                                                                                                                                                                                                         |
| 2. **TVA**                                                  | —                                                                                                                                                                                                                                             |
| 3. **Loyer TTC**                                            | Calculé automatiquement, non modifiable.                                                                                                                                                                                                      |
| 4. **Activer la déduction des loyers**                      | « Non » par défaut. Répondez « Oui » pour faire apparaître les deux champs suivants, qui concernent la part de loyer que la fiscalité n'autorise pas à déduire.                                                                               |
| **Plafond applicable**                                      | Il ne s'affiche que si vous avez répondu « Oui ». Son infobulle précise que la base d'amortissement fiscal est renseignée par rapport au plafond de déductibilité des amortissements des véhicules de tourisme selon le BOI-BIC-AMT-20-40-50. |
| **Part annuelle des loyers non déductible**                 | Il ne s'affiche que si vous avez répondu « Oui ».                                                                                                                                                                                             |

## Rubrique « Premier loyer »

<figure><img src="../../.gitbook/assets/15-cm816-14-premier-loyer.png" alt="Crédits-bails, Rubrique « Premier loyer »"><figcaption><p>Rubrique « Premier loyer »</p></figcaption></figure>

| Champ                                                            | Ce qu'il faut savoir                                                                                                                                                    |
| ---------------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1. **Le premier loyer est-il différent ?**                       | « Non » par défaut, et la rubrique ne contient alors que cette question. Répondez « Oui » si le contrat prévoit un premier loyer majoré, et trois champs apparaissent : |
| <p><strong>Premier loyer HT</strong><br><em>Obligatoire</em></p> | Dès que vous avez répondu « Oui ».                                                                                                                                      |
| **TVA**                                                          | —                                                                                                                                                                       |
| **Premier loyer TTC**                                            | Calculé automatiquement, non modifiable.                                                                                                                                |

## Rubrique « Coûts annexes »

<figure><img src="../../.gitbook/assets/15-cm816-15-couts-annexes.png" alt="Crédits-bails, Rubrique « Coûts annexes »"><figcaption><p>Rubrique « Coûts annexes »</p></figcaption></figure>

Aucun champ de cette rubrique n'est obligatoire.

| Champ                      | Ce qu'il faut savoir                                                                      |
| -------------------------- | ----------------------------------------------------------------------------------------- |
| 1. **Total des frais HT**  | Une infobulle rappelle qu'il s'agit des frais de dossier et de tous types d'autres frais. |
| 2. **TVA sur frais**       | —                                                                                         |
| 3. **Total des frais TTC** | Calculé automatiquement, non modifiable.                                                  |

## Rubrique « Assurance »

<figure><img src="../../.gitbook/assets/15-cm816-16-assurance.png" alt="Crédits-bails, Rubrique « Assurance »"><figcaption><p>Rubrique « Assurance »</p></figcaption></figure>

| Champ                                                                     | Ce qu'il faut savoir                                                                               |
| ------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------- |
| 1. **Type d'assurance**                                                   | Deux choix seulement, « Sans assurance » (valeur par défaut) et « Montant fixe par échéance ».     |
| <p><strong>Montant fixe par échéance</strong><br><em>Obligatoire</em></p> | Il ne s'affiche, et ne devient obligatoire, que si vous avez retenu « Montant fixe par échéance ». |
| **Montant total**                                                         | Non modifiable, calculé par le logiciel. Il ne s'affiche que dans le même cas.                     |

Si vous basculez sur « Montant fixe par échéance » sans avoir renseigné le nombre d'échéances, le logiciel ouvre une fenêtre d'erreur portant « Le nombre d'échéances doit être renseigné. » : sans ce nombre, il ne peut pas calculer le montant total de l'assurance.

## Rubrique « Montant de l'option d'achat »

<figure><img src="../../.gitbook/assets/15-cm816-17-montant-de-l-option-d-achat.png" alt="Crédits-bails, Rubrique « Montant de l&#x27;option d&#x27;achat »"><figcaption><p>Rubrique « Montant de l'option d'achat »</p></figcaption></figure>

C'est le montant de la levée d'option, celui que vous paierez pour devenir propriétaire du bien en fin de contrat. Aucun champ n'est obligatoire.

**Montant de l'option HT** : facultatif. **TVA :** facultatif. **Montant de l'option TTC :** calculé automatiquement, non modifiable.

## Rubrique « Subventions »

Cette rubrique n'apparaît que sur une fiche déjà enregistrée, et seulement si au moins une subvention a été rattachée à ce crédit-bail. Le rattachement ne se fait pas ici : il se fait depuis la fiche de la subvention, dont le régime d'étalement est alors « Liée à un crédit-bail ».

Le tableau présente quatre colonnes — **Code**, **Libellé**, **Date d'octroi** et **Montant affecté** — et le pictogramme « Œil » de chaque ligne vous permet de visualiser la fiche de la subvention.

Une conséquence à connaître : dès qu'une subvention est rattachée, le coût global HT du crédit-bail ne peut plus être inférieur au montant total des subventions affectées. Si vous diminuez les loyers ou les frais au point de passer sous ce total, le logiciel refuse l'enregistrement en vous rappelant le montant des subventions affectées.

## Rubrique « Commentaires »

<figure><img src="../../.gitbook/assets/15-cm816-20-commentaires.png" alt="Crédits-bails, Rubrique « Commentaires »"><figcaption><p>Rubrique « Commentaires »</p></figcaption></figure>

C'est une zone de saisie libre, facultative, de 1 024 caractères au maximum, modifiable à tout moment.

## Rubrique « Documents »

<figure><img src="../../.gitbook/assets/15-cm816-18-documents.png" alt="Crédits-bails, Rubrique « Documents »"><figcaption><p>Rubrique « Documents »</p></figcaption></figure>

Vous pouvez joindre des documents à la fiche du crédit-bail : le contrat, l'échéancier remis par l'organisme, la facture du bien. Le tableau présente quatre colonnes — **Description**, **Nom du fichier**, **Date** et **Créé par** — et affiche « Liste vide » tant qu'aucun document n'est rattaché.

Trois boutons vous sont proposés selon l'origine du document : bouton **\[Nouveau doc depuis mon poste]**, bouton **\[Nouveau doc depuis la GED]** et bouton **\[Nouveau doc depuis l'OCR]**.

## Rubrique « Paramètres comptables »

<figure><img src="../../.gitbook/assets/15-cm816-19-parametres-comptables.png" alt="Crédits-bails, Rubrique « Paramètres comptables »"><figcaption><p>Rubrique « Paramètres comptables »</p></figcaption></figure>

Cette rubrique réunit le journal et les comptes nécessaires à la comptabilisation des écritures du crédit-bail.

| Champ                                                                             | Ce qu'il faut savoir                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| --------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1. **Journal**                                                                    | <p>Le sélecteur propose les journaux du dossier ; il affiche « Sélectionnez » tant que vous n'avez pas choisi.<br><strong>Compte de charge des loyers * :obligatoire</strong> — c'est le seul compte de la rubrique à l'être.<br>Viennent ensuite quatre comptes facultatifs : <strong>Compte d'immobilisations</strong>, <strong>Compte d'assurance</strong>, <strong>Compte de frais de dossier</strong> et <strong>Compte de TVA</strong>.<br>Chaque ligne de compte comporte le numéro, l'intitulé du compte en regard — non modifiable, il se remplit dès que le numéro est reconnu — puis deux commandes : le bouton <strong>[+]</strong> qui crée le compte s'il n'existe pas encore, et une loupe qui ouvre la recherche dans le plan comptable. La loupe est également accessible au clavier par la combinaison Ctrl + Alt + L. Un numéro qui ne correspond à aucun compte existant est refusé à l'enregistrement.</p> |
| 2. **Souhaitez-vous déclencher la comptabilisation automatique des loyers ?**     | « Non » par défaut. Si vous répondez « Oui », le logiciel vérifie chaque nuit s'il a des écritures de loyers à comptabiliser pour ce crédit-bail, les génère et les enregistre en comptabilité sans autre intervention de votre part.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| <p><strong>Date de début de comptabilisation</strong><br><em>Obligatoire</em></p> | Elle ne s'affiche, et ne devient obligatoire, que si vous avez répondu « Oui » à la question précédente. Elle doit être comprise dans la période de saisie ou dans les dates de l'exercice. Attention à ce que dit son infobulle : la comptabilisation automatique porte sur les **loyers**, mais la comptabilisation des **frais** du crédit-bail reste à demander une fois, à l'aide du bouton \[Comptabilisation manuelle].                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  |

Notez qu'il n'y a pas ici de choix entre écriture complète et écriture de répartition, contrairement à la fiche d'un emprunt.

## Bouton \[Enregistrer]

<figure><img src="../../.gitbook/assets/15-cm816-21-bouton-enregistrer-enregistrer.png" alt="Crédits-bails, Bouton [Enregistrer]"><figcaption><p>Bouton [Enregistrer]</p></figcaption></figure>

Il enregistre la fiche. Selon les droits qui vous sont accordés, il peut ne pas vous être proposé. Il n'est plus proposé une fois le crédit-bail transféré en immobilisation.

## Bouton \[Tableau des échéances]

<figure><img src="../../.gitbook/assets/15-cm816-21-bouton-enregistrer-tableau-des-echeances.png" alt="Crédits-bails, Bouton [Tableau des échéances]"><figcaption><p>Bouton [Tableau des échéances]</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/15-cm816-22-bouton-tableau-des-echeances.png" alt="Crédits-bails, Bouton [Tableau des échéances]"><figcaption><p>Bouton [Tableau des échéances]</p></figcaption></figure>

Il n'est proposé que sur une fiche déjà enregistrée, et selon les droits qui vous sont accordés. Il ouvre l'échéancier des loyers calculé à partir des caractéristiques de la fiche, sous la forme d'un tableau d'une ligne par échéance : **N° échéance**, **Date échéance**, **Loyer HT**, **Montant TVA**, **Assurance**, **Loyer TTC**, **Cumul échéances** et **Échéances restantes**. Une ligne de totaux ferme le tableau. Si aucune échéance ne peut être calculée, le tableau affiche « Aucune échéance à afficher. »

Cet échéancier est en consultation seule : contrairement à celui d'un emprunt, il ne peut pas être personnalisé ligne à ligne. Deux boutons seulement y figurent, bouton **\[Imprimer l'échéancier]** et bouton **\[Retour]**.

## Bouton \[Comptabilisation manuelle]

<figure><img src="../../.gitbook/assets/15-cm816-21-bouton-enregistrer-comptabilisation-manuelle.png" alt="Crédits-bails, Bouton [Comptabilisation manuelle]"><figcaption><p>Bouton [Comptabilisation manuelle]</p></figcaption></figure>

Il n'est proposé que sur une fiche déjà enregistrée, et selon les droits qui vous sont accordés. Il ouvre une fenêtre qui vous rappelle d'abord ceci : la comptabilisation manuelle génère des écritures sur la base de ce qui figure dans la fiche, et si les écritures ont déjà été générées — manuellement ou automatiquement — de nouvelles écritures seront générées, à vous de faire les ajustements nécessaires en comptabilité. Autrement dit, le logiciel ne détecte pas les doublons à votre place.

**Comptabilisation des frais** : répondez « Oui » pour comptabiliser en même temps les frais de dossier du crédit-bail. C'est une opération à ne faire qu'une seule fois, à la mise en place du contrat.

**Date de début** et **Date de fin :** obligatoires. Elles délimitent la période dont vous souhaitez comptabiliser les loyers, et doivent toutes deux être comprises dans la période de saisie.

bouton **\[Valider]** : il lance la comptabilisation. Le logiciel vous indique ensuite le nombre de lignes d'écriture générées, ou vous répond qu'aucune ligne n'a été générée. S'il ne peut pas comptabiliser, il vous en donne la liste des raisons — le plus souvent un compte ou une information manquante dans la rubrique « Paramètres comptables ».

bouton **\[Annuler]** : il ferme la fenêtre sans rien comptabiliser.

## Bouton \[Transfert en immobilisation]

<figure><img src="../../.gitbook/assets/15-cm816-21-bouton-enregistrer-transfert-en-immobilisation.png" alt="Crédits-bails, Bouton [Transfert en immobilisation]"><figcaption><p>Bouton [Transfert en immobilisation]</p></figcaption></figure>

Il n'est proposé que sur une fiche déjà enregistrée et non encore transférée, et selon les droits qui vous sont accordés. C'est l'opération de la levée d'option : le bien cesse d'être loué et entre à l'actif.

Une fenêtre de confirmation vous explique la manœuvre : si vous confirmez, vous êtes redirigé vers la fiche de saisie d'une immobilisation préremplie avec les informations du crédit-bail. Si vous enregistrez cette fiche, le crédit-bail sera clos ; si vous annulez la création de la fiche immobilisation en cours de saisie, la fiche du crédit-bail ne sera pas altérée. Vous validez par le bouton **\[Valider]** ou renoncez par le bouton **\[Annuler]**.

Une fois le transfert effectué, le crédit-bail apparaît dans la liste sous le statut « Crédits-bails transférés en immobilisations », son libellé n'est plus modifiable, et les boutons \[Enregistrer] et \[Transfert en immobilisation] ne vous sont plus proposés.

## Bouton \[Imprimer l'échéancier]

<figure><img src="../../.gitbook/assets/15-cm816-21-bouton-enregistrer-imprimer-l-echeancier.png" alt="Crédits-bails, Bouton [Imprimer l&#x27;échéancier]"><figcaption><p>Bouton [Imprimer l'échéancier]</p></figcaption></figure>

Selon les droits qui vous sont accordés, il peut ne pas vous être proposé. Il ouvre une fenêtre d'édition où vous choisissez :

| Champ                           | Ce qu'il faut savoir                                |
| ------------------------------- | --------------------------------------------------- |
| **Avec des sous-totaux par an** | Répondez « Oui » pour obtenir un sous-total annuel. |
| **Format**                      | HTML, PDF ou Excel.                                 |

**Orientation** et **Largeur :** ces deux choix n'apparaissent que pour le format PDF. L'infobulle de la largeur précise qu'elle ajuste la taille si la largeur des colonnes dépasse la largeur de la page.

bouton **\[Edition]** génère le document ; bouton **\[Annuler]** ferme la fenêtre.

## Bouton \[Retour]

Il revient à la liste des crédits-bails sans rien enregistrer.
