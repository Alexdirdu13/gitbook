# Présentation

L'API V2 donne accès aux données comptables d'un cabinet et de ses sociétés : sociétés et dossiers annuels, écritures, imports, facturation, immobilisations, banque, dossier permanent. Cette page explique comment faire un premier appel ; la référence détaille ensuite chaque opération, domaine par domaine.

## Démarrage rapide

{% stepper %}
{% step %}
## Récupérer vos identifiants

Les identifiants sont un code et une clé API, à demander au cabinet qui vous mandate. Le cabinet les trouve dans Ingeneo Compta, à l'écran de gestion de la clé API.

| Vous êtes…                     | `client_id`             | `client_secret`          | Droits                                        |
| ------------------------------ | ----------------------- | ------------------------ | --------------------------------------------- |
| Le cabinet, ou son intégrateur | `CODEABONNE`            | Clé API complète         | Lecture et écriture                           |
| Le cabinet, en consultation    | `CODEABONNE`            | Clé API en lecture seule | Lecture                                       |
| Une société cliente du cabinet | `CODEABONNE.CODECLIENT` | Clé API de la société    | Lecture et écriture, sur sa société seulement |
{% endstep %}

{% step %}
## Demander un jeton

```bash
curl -X POST https://<instance>/api/v2/oauth/token \
  -d grant_type=client_credentials -d client_id=<CODEABONNE> -d client_secret=<clé API>
```

```json
{ "access_token": "eyJ…", "token_type": "Bearer", "expires_in": 3600, "scope": "lecture ecriture" }
```
{% endstep %}

{% step %}
## Appeler une ressource

```bash
curl "https://<instance>/api/v2/societes?taille=20" -H "Authorization: Bearer <jeton>"
```
{% endstep %}
{% endstepper %}

### À savoir sur le jeton

* Il vaut **60 minutes**. Il n'y a pas de jeton de rafraîchissement : redemandez-en un avec les mêmes identifiants.
* Il ne vaut que pour le serveur qui l'a émis. Si l'abonné est hébergé sur un autre serveur, la demande de jeton répond par une redirection `307` : suivez-la une fois et gardez cette adresse pour la suite.
* Si le cabinet régénère sa clé API, les jetons en cours sont refusés (`401 jeton_revoque`) : demandez la nouvelle clé.
* L'en-tête `Authorization: Basic base64(client_id:client_secret)` est accepté à la place du corps de formulaire.

## Conventions

* **Adresse de base** : `https://<instance>/api/v2`.
* **Format** : JSON en camelCase, dates ISO 8601, énumérations en texte, champs nuls omis.
* **Pagination** : `?page=1&taille=50` rend `{ elements, page, taille, total }`.
* **Débit** : 10 demandes de jeton par minute et par adresse, 120 requêtes par minute et par client. Au-delà, `429` avec l'en-tête `Retry-After`.
* **Identifiant de requête** : chaque réponse porte l'en-tête `X-Request-Id`. Citez-le au support.

## Erreurs

Le code HTTP dit toujours le résultat : il n'y a jamais de `200` sur un échec. Une erreur est un corps `application/problem+json` (RFC 9457) avec un `code` stable, un `detail` lisible et un `requestId`.

| Statut | Exemples de `code`                                                       | Sens                                                                                 |
| ------ | ------------------------------------------------------------------------ | ------------------------------------------------------------------------------------ |
| 400    | `requete_invalide`, `pagination_invalide`, `date_invalide`               | Paramètre ou corps illisible                                                         |
| 401    | `jeton_absent`, `jeton_invalide`, `jeton_revoque`                        | Jeton manquant, expiré, ou clé régénérée                                             |
| 403    | `portee_insuffisante`, `societe_interdite`, `reserve_au_cabinet`         | Clé en lecture seule sur une écriture, société hors de votre périmètre               |
| 404    | `societe_introuvable`, `dossier_annuel_introuvable`, `route_introuvable` | Ressource inconnue                                                                   |
| 409    | `base_inexistante`, `dossier_annuel_cloture`                             | L'état de la ressource interdit l'opération                                          |
| 422    | `traitement_rejete`, `import_avec_anomalies`                             | Reçu mais refusé par les règles métier ; le détail ligne à ligne est dans `resultat` |
| 429    | `debit_depasse`                                                          | Quota par minute atteint                                                             |
| 503    | `api_desactivee`                                                         | L'API n'est pas ouverte sur ce serveur                                               |

La demande de jeton fait exception : ses erreurs suivent le format OAuth2, `{ "error": "invalid_client", "error_description": "…" }`.

## Vous utilisez déjà la V1

Les webservices `MonCompteService.svc` restent servis au moins un an après la mise en ligne de la V2. Ils annonceront leur fin par les en-têtes `Deprecation`, `Sunset` et `Link rel="successor-version"`. La page « Migrer depuis la V1 » donne les règles de passage.
