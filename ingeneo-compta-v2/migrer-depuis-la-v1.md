# Migrer depuis la V1

Cette page s'adresse aux intégrateurs qui appellent déjà les webservices `MonCompteService.svc`. Elle donne les règles de passage vers `/api/v2`, puis l'équivalent de chaque domaine. Le détail de chaque opération est dans la référence.

Les charges utiles (corps des requêtes d'écriture) gardent la structure de la V1 : l'essentiel du travail de migration porte sur l'authentification, les adresses et la lecture des erreurs.

## Ce qui change

| V1                                                                                                   | V2                                                                                                            |
| ---------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| En-têtes `CODEABONNE`, `TICKET`, `CLE` (et `CODECLIENT`), avec une empreinte calculée à chaque appel | Un jeton `Authorization: Bearer …`, demandé une fois par heure sur `oauth/token`                              |
| `GET Societes/{codeClient}/DossiersAnnuels/{id}/…`                                                   | `GET societes/{codeClient}/dossiers-annuels/{id}/…` : minuscules et tirets                                    |
| Identifiant du dossier annuel obligatoire                                                            | `en-cours` accepté à la place de l'identifiant, pour viser le dossier annuel en cours                         |
| `200` avec `EstErreur` ou un rapport à inspecter                                                     | Le code HTTP porte le résultat : `200` fait, `422` tout rejeté, autres `4xx` refus expliqué en `problem+json` |
| Dates en texte, parfois doublées d'une date typée                                                    | Une seule date, en ISO 8601                                                                                   |
| Fichier en multipart ou en base64                                                                    | Corps brut, nom du fichier dans l'adresse                                                                     |
| Suffixes `/MAJ`, `/Creer`, `/Supprimer` dans l'adresse                                               | Verbes HTTP : `POST` crée, `PUT` remplace, `PATCH` modifie, `DELETE` supprime                                 |
| Liste rendue pour un élément unique                                                                  | L'objet lui-même, ou `404` s'il n'existe pas                                                                  |

## Équivalences par domaine

| Domaine V1                                                                          | Ressources V2                                                                                                 |
| ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------- |
| Sociétés, bases, modèles éditeur                                                    | `societes`, `societes/{codeClient}`, `societes/{codeClient}/base`, `societes-modeles-editeur`                 |
| Dossiers annuels : création, base, clôture, suppression                             | `societes/{codeClient}/dossiers-annuels`, `…/{id}`, `…/base`, `…/cloture`                                     |
| Utilisateurs et tags                                                                | `utilisateurs`, `utilisateurs/{code}`, `tags`, `utilisateurs/{code}/tags`                                     |
| Télédéclarations                                                                    | `teledeclarations`, `teledeclarations/edi`                                                                    |
| Comptabilité : comptes, tiers, journaux, TVA, axes, écritures, documents            | `…/dossiers-annuels/{id}/comptes`, `comptes-auxiliaires`, `journaux`, `tva`, `axes`, `ecritures`, `documents` |
| Éditions                                                                            | `…/dossiers-annuels/{id}/editions/…`                                                                          |
| Imports de fichiers (FEC, TRA, immobilisations, CFONB, écritures par modèle) et OCR | `imports/{type}/{nomFichier}`, `societes/{codeClient}/ocr/documents/{nomFichier}`                             |
| Paie : boîte aux lettres, Ximi, DSN                                                 | `paie/boite-aux-lettres/{nomFichier}`, `societes/{codeClient}/paie/…`                                         |
| Facturation : factures, avoirs, documents, clients                                  | `…/dossiers-annuels/{id}/factures`, `avoirs`, `clients`                                                       |
| Banque et relevés                                                                   | `…/banques`, `…/banques/lignes-archivees/cfonb`, `stb/regles-traduction`, `stb/affectations`                  |
| Immobilisations et emprunts                                                         | `…/dossiers-annuels/{id}/immobilisations…`, `…/emprunts…`                                                     |
| Vision Expert                                                                       | `societes/{codeClient}/vision/frise-sur-budget`, `vision/modeles/{modele}/frise-sur-budget`                   |
| Feuilles personnalisées                                                             | `…/dossiers-annuels/{id}/feuilles-personnalisees…`                                                            |
| Données externes                                                                    | `societes/{codeClient}/donnees-externes…`                                                                     |
| Plaquettes                                                                          | `…/dossiers-annuels/{id}/plaquettes…`                                                                         |
| Dossier permanent                                                                   | `societes/{codeClient}/dossier-permanent/…`                                                                   |

## Ce qui disparaît

* Les adresses de dossier annuel sans société (`DossiersAnnuels/…`) : en V2, un dossier annuel se lit toujours sous sa société.
* Les tags d'une actualité (`Actualites/{id}/Tags`) et le dépôt de documents bancaires en XML (`Banque/Documents`) n'ont pas d'équivalent en V2.

{% hint style="warning" %}
Si vous utilisez une opération V1 que vous ne retrouvez pas dans la référence, signalez-le au support avant la fin de la V1.
{% endhint %}
