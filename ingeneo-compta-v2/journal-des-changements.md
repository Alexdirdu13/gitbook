# Journal des changements

Le format suit [Keep a Changelog](https://keepachangelog.com/fr/1.1.0/). La version du contrat est celle du document OpenAPI (`info.version`).

## \[2.0.0] — en préparation (branche `API-V2`, novembre 2026)

Première version de l'API V2 (`/api/v2`), successeur de `MonCompteService.svc`.

### Ajouté

* OAuth2 _client credentials_ (`POST oauth/token`), jetons JWT de 60 minutes, portées `lecture` / `ecriture`, clients cabinet, société cliente, instance.
* Erreurs `application/problem+json` avec `code` stable et `requestId` ; plus de `200` sur un échec ; `422` avec le résultat ligne à ligne des traitements en lot.
* Rate limiting (jeton par adresse, requêtes par client), `429` + `Retry-After`.
* Document OpenAPI 3.0 servi par l'instance (`GET openapi.json`, sous drapeau) et versionné dans ce dossier.
* Sociétés et dossiers annuels (joker `en-cours`, `?inclure=dossiers-annuels`), utilisateurs, tags, télédéclarations, modèles éditeur.
* Comptabilité d'un dossier (comptes, tiers, journaux, TVA, axes, écritures, documents, import, purge), éditions.
* Imports de fichiers (FEC, TRA, immobilisations, CFONB, écritures par modèle), dépôt OCR ; paie (boîte aux lettres, Ximi, DSN).
* Facturation (factures, avoirs, PDF, clients), banques, CFONB archivé, STB ; immobilisations, emprunts, échéanciers, Vision ; feuilles personnalisées, données externes, plaquettes ; dossier permanent (identité, fiscal, juridique, documents).

### Modifié par rapport à la V1

* Dates en ISO 8601 (`2026-01-31`), énumérations en texte, champs nuls omis, camelCase.
* Les fichiers s'envoient en corps brut (`application/octet-stream`), le nom dans la route ; plus de multipart.
* Les routes « sans société » des dossiers annuels ne sont pas reprises : un dossier se lit toujours sous sa société.
* Les « MAJ » du dossier permanent deviennent des `PUT` ; les sept dépôts de documents V1 fusionnent en `POST …/documents/{typeDocument}/{nomFichier}`.

### Retiré

* Les en-têtes `CODEABONNE` / `TICKET` / `CLE` et l'empreinte MD5 : remplacés par le jeton.
* La documentation PDF : remplacée par ce dossier et le portail développeurs.
