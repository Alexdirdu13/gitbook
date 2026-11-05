# Modèles d'export

{% hint style="info" %}
**Où le trouver :** Panneau **Paramètres**
{% endhint %}

{% hint style="success" %}
**En bref** — Cet écran gère les modèles d'export de données fournis par Ingeneo Compta et vous permet de créer vos propres modèles, notamment pour exporter le brouillard d'écritures.

* Pour récupérer les modèles fournis par Ingeneo Compta : bouton \[Charger les nouveaux modèles].
* Pour créer un modèle : bouton \[Nouveau], renseignez les « Informations générales » puis la position de chaque champ dans « Données du modèle », et bouton \[Enregistrer].
* Pour supprimer des modèles : cochez-les dans la liste, puis bouton \[Supprimer].
{% endhint %}

Cette option permet de gérer les modèles d'export de données fournis par Ingeneo Compta mais aussi de créer vos propres modèles.

<figure><img src="../../.gitbook/assets/33-modeles-d-export.png" alt="Écran Modèles d&#x27;export"><figcaption><p>Écran « Modèles d'export » de la nouvelle interface</p></figcaption></figure>

L'écran affiche la liste des modèles existants sur quatre colonnes : **Libellé**, **Fichier** (la nature des données exportées), **Description** et **Modifiable**.

L'en-tête de la liste vous propose les pictogrammes habituels de sélection, de personnalisation des colonnes, de filtre et d'impression.

Chaque ligne porte trois pictogrammes : « Crayon » pour ouvrir le modèle, « Croix » pour le supprimer et « Feuille avec un plus » pour le dupliquer.

bouton **\[Nouveau]**

Ouvre le formulaire de création d'un modèle, décrit ci-dessous.

bouton **\[Charger les nouveaux modèles]**

Récupère les modèles fournis par Ingeneo Compta qui ne figurent pas encore dans votre liste.

bouton **\[Supprimer]**

Supprime les modèles que vous avez cochés dans la liste.

## Rubrique « Informations générales »

<figure><img src="../../.gitbook/assets/33-cm385-21-informations-generales.png" alt="Modèles d&#x27;export, Rubrique « Informations générales »"><figcaption><p>Rubrique « Informations générales »</p></figcaption></figure>

| Champ                                                              | Ce qu'il faut savoir                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| ------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 1. **Type de fichier**                                             | Il décrit la nature du fichier des éléments exportés et donc les champs que le fichier sera susceptible de contenir. Depuis le module OCR, une seule valeur vous est proposée : « Brouillard d'écritures ».                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| 2. **Libellé**                                                     | —                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| 3. **Description**                                                 | —                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| 4. **Type de séparation**                                          | <p>Les enregistrements des fichiers exportés peuvent être construits de deux manières en fonction de fichier à générer :<br>• soit avec des longueurs fixes : dans ce cas chaque champ occupe sur chaque ligne la même position (par exemple le champ « date » du caractère 1 à 10, le champ « n° de compte » du caractère 11 à 18, le champ « Libellé d'écriture » du caractère 19 à 53, etc. et ce, quelle que soit la taille effective du contenu (les caractères inutilisés étant occupés par des espaces) ;<br>• soit avec des longueurs variables (il n'y a plus d'espaces inutilisés) mais dans ce cas tous les champs doivent être séparés par un caractère facilement identifiable.</p> |
| 5. **Séparateur**                                                  | Le caractère séparateur est présent uniquement pour les fichiers avec un « Type de séparation » à « Séparateur de champs » et est obligatoire. Les caractères les plus courants sont dans le sélecteur mais vous avez la possibilité d'en indiquer un différent en cliquant sur le choix « Autre ».                                                                                                                                                                                                                                                                                                                                                                                              |
| 6. **Caractère d'encadrement**                                     | Le caractère d'encadrement est demandé uniquement pour les fichiers avec un « Type de séparation » à « Séparateur de champs » et est facultatif. Il permet, en plus du caractère séparateur, d'ajouter un caractère d'encadrement pour indiquer le début et la fin de chaque champ, comme des guillemets par exemple.                                                                                                                                                                                                                                                                                                                                                                            |
| **Format des dates (ex. jj/mm/aaaa)**                              | Choisissez dans le sélecteur le format de date à utiliser dans le fichier à exporter.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Séparateur des décimales**                                       | —                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Nombre de décimales**                                            | —                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Ignorer les données vides**                                      | Si l'interrupteur est activé, le logiciel n'écrit rien dans le fichier lorsque la donnée est absente.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Afficher un en-tête**                                            | Le fichier généré aura une ligne d'en-tête contenant, dans le même ordre, les libellés de tous les champs présents dans le fichier exporté.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| **Supprimer les caractères '0' terminaux des comptes auxiliaires** | Si l'interrupteur est activé, les zéros de fin des numéros de comptes auxiliaires ne sont pas exportés.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |

## Rubrique « Gestion des comptes auxiliaires et collectifs »

<figure><img src="../../.gitbook/assets/33-cm385-23-gestion-des-comptes-auxiliaires-et-collectifs.png" alt="Modèles d&#x27;export, Rubrique « Gestion des comptes auxiliaires et collectifs »"><figcaption><p>Rubrique « Gestion des comptes auxiliaires et collectifs »</p></figcaption></figure>

L'écran rappelle qu'Ingeneo Compta gère les comptes auxiliaires dans un fichier distinct des comptes généraux, puis vous pose la question **« Les écritures exportées sont-elles gérées de la même manière ? »**. Si ce n'est pas le cas pour le fichier exporté, les écritures concernant des tiers et contenant un compte collectif et un compte auxiliaire seront retraitées ; le compte auxiliaire sera placé à la place du compte collectif avant d'être exporté.

## Rubrique « Données du modèle »

<figure><img src="../../.gitbook/assets/33-cm385-24-donnees-du-modele.png" alt="Modèles d&#x27;export, Rubrique « Données du modèle »"><figcaption><p>Rubrique « Données du modèle »</p></figcaption></figure>

Il faut, pour finaliser le modèle, indiquer la position de chaque champ.

Si le type de séparation du fichier est à « Caractères fixes », pour chaque champ, vous devez indiquer la position de son premier caractère et sa longueur en nombre de caractères. La taille maximale gérée dans Ingeneo Compta est indiquée sur chaque ligne ; si vous indiquez une valeur supérieure, vous ne pourrez pas enregistrer le modèle.

Si le champ du fichier Ingeneo Compta est plus grand que la taille que vous indiquez, il sera tronqué à la taille indiquée.

Si le type de séparation du fichier est à « Séparateur de champs » : pour chaque champ vous devez indiquer son numéro d'ordre dans les lignes du fichier exporté.

Le dernier champ « Référence des pièces jointes » est particulier. En effet, si vous utilisez ce champ, vous pourrez exporter non seulement les écritures mais également les pièces jointes à toutes les écritures.

bouton **\[Enregistrer]**

Enregistre le modèle et vous ramène à la liste.

bouton **\[Retour]**

Revient à la liste sans enregistrer.

## Autres vues de l'écran

<figure><img src="../../.gitbook/assets/33-cm385-11-bouton-nouveau.png" alt="Modèles d&#x27;export, Bouton [Nouveau]"><figcaption><p>Bouton [Nouveau]</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/33-cm385-12-bouton-nouveau.png" alt="Modèles d&#x27;export, Bouton [Nouveau]"><figcaption><p>Bouton [Nouveau]</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/33-cm385-22-changement-des-numeros-de-compte.png" alt="Modèles d&#x27;export, Changement des numéros de compte"><figcaption><p>Changement des numéros de compte</p></figcaption></figure>
