# Modèles d'import

{% hint style="info" %}
**Où le trouver :** Panneau **Paramètres**
{% endhint %}

{% hint style="success" %}
**En bref** — Un modèle d'import décrit la structure d'un fichier de plan comptable à importer, pour que tous les fichiers construits de la même manière s'importent sans nouveau paramétrage.

* Pour créer un modèle : bouton \[Nouveau], renseignez la rubrique « Informations générales » et le « Type de séparation », puis bouton \[Enregistrer].
* Pour situer chaque information dans le fichier : rubrique « Données du modèle », numéro de colonne ou position du premier caractère et taille du champ.
* Pour partir d'un modèle voisin : pictogramme de duplication de sa ligne.
{% endhint %}

Un modèle d'import décrit la structure d'un fichier à importer : il indique au logiciel où trouver chaque information dans le fichier, et sous quelle forme elle y figure. Une fois le modèle défini, tous les fichiers construits de la même manière peuvent être importés sans nouveau paramétrage.

<figure><img src="../../.gitbook/assets/33-modeles-d-import.png" alt="Écran Modèles d&#x27;import"><figcaption><p>Écran « Modèles d'import » de la nouvelle interface</p></figcaption></figure>

**Depuis le module OCR, seuls les plans comptables s'importent.** Les modèles définis ici ne concernent donc que ce type de fichier. L'import d'écritures et de balances relève du module de comptabilité.

Vous pouvez créer vos propres modèles.

## La liste des modèles

<figure><img src="../../.gitbook/assets/33-cm385-11-bouton-nouveau.png" alt="Modèles d&#x27;import, Bouton [Nouveau]"><figcaption><p>Bouton [Nouveau]</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/33-cm385-12-bouton-nouveau.png" alt="Modèles d&#x27;import, Bouton [Nouveau]"><figcaption><p>Bouton [Nouveau]</p></figcaption></figure>

La grille présente les modèles d'import du module, avec pour chacun son **Libellé**, le **Fichier** concerné et sa **Description**. Ce sont ses trois seules colonnes : la personnalisation de la grille n'en propose aucune autre.

L'en-tête de la liste vous propose les pictogrammes habituels de sélection, de personnalisation des colonnes, de filtre et d'impression. Le pictogramme de personnalisation ouvre la fenêtre « Personnalisation de colonnes », où vous rendez chaque colonne visible ou non, fixez sa largeur et modifiez son ordre, puis validez par le bouton **\[Appliquer]**, revenez aux valeurs d'origine par le bouton **\[Réinitialiser]** ou renoncez par le bouton **\[Annuler]**.

Les pictogrammes de chaque ligne permettent de modifier, de supprimer ou de **dupliquer** un modèle. La duplication évite de resaisir entièrement un paramétrage voisin d'un modèle existant.

En barre du bas de l'écran, le bouton **\[Nouveau]** crée un modèle, et le bouton **\[Supprimer]** supprime ceux que vous avez cochés.

## Rubrique « Informations générales »

<figure><img src="../../.gitbook/assets/33-cm385-21-informations-generales.png" alt="Modèles d&#x27;import, Rubrique « Informations générales »"><figcaption><p>Rubrique « Informations générales »</p></figcaption></figure>

Cette rubrique décrit la forme du fichier. Les champs suivis d'une astérisque sont obligatoires.

| Champ                                                                             | Ce qu'il faut savoir                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| --------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| <p>1. <strong>Type de fichier</strong><br><em>Obligatoire</em></p>                | Depuis l'OCR, la seule valeur proposée est **« Comptes »**.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                        |
| <p>2. <strong>Libellé</strong><br><em>Obligatoire</em></p>                        | Le nom sous lequel le modèle apparaîtra dans la liste.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                             |
| 3. **Description**                                                                | Facultative.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                       |
| 4. **Type de séparation**                                                         | <p>Deux boutons, selon la façon dont le fichier est construit :<br>• <strong>Caractères fixes</strong> : chaque information occupe toujours la même position sur la ligne — par exemple le numéro de compte du caractère 1 au caractère 12 — quelle que soit la longueur réelle de son contenu, les caractères inutilisés étant remplis d'espaces ;<br>• <strong>Séparateur de champs</strong> : les informations n'ont pas de longueur fixe, et sont séparées les unes des autres par un caractère identifiable.</p>                                                                                                                              |
| <p>5. <strong>Séparateur</strong><br><em>Obligatoire</em></p>                     | Demandé uniquement pour un fichier à séparateur de champs. Choisissez-le dans la liste : **Point**, **Virgule**, **Point-virgule**, **Tabulation**, **Tiret**, **Sous-tiret**. Le choix **Autre** permet d'indiquer un caractère qui ne figure pas dans la liste.                                                                                                                                                                                                                                                                                                                                                                                  |
| 6. **Caractère d'encadrement**                                                    | Lui aussi réservé aux fichiers à séparateur de champs. Certains fichiers encadrent chaque information par un caractère, des guillemets par exemple, pour en marquer le début et la fin.                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| 7. **Nombre de lignes en-tête à ignorer**                                         | Certains fichiers commencent par des lignes qui ne sont pas des données, les noms des colonnes par exemple. Indiquez ici combien de lignes le logiciel doit passer avant de commencer à lire.                                                                                                                                                                                                                                                                                                                                                                                                                                                      |
| 8. **Nombre de lignes de pied à ignorer**                                         | Sur le même principe pour la fin du fichier, qui peut porter des totaux.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| <p><strong>Format des dates (ex. jj/mm/aaaa)</strong><br><em>Obligatoire</em></p> | <p>Choisissez le format employé dans le fichier à importer. Une vingtaine de combinaisons sont proposées, du plus courant <strong>JJ/MM/AAAA</strong> aux formats sans séparateur comme <strong>AAAAMMJJ</strong>. Les dates lues sont automatiquement converties au format « JJ/MM/AAAA ».<br><strong>Séparateur des décimales * :Virgule</strong>, <strong>Point</strong> ou <strong>Rien</strong>. Le choix « Rien » signifie que les montants du fichier ne portent aucun séparateur : le logiciel considère alors que tous comportent le même nombre de décimales, celui que vous indiquez juste en dessous.<br>**Nombre de décimales ***</p> |

## Rubrique « Gestion des comptes auxiliaires et collectifs »

<figure><img src="../../.gitbook/assets/33-cm385-23-gestion-des-comptes-auxiliaires-et-collectifs.png" alt="Modèles d&#x27;import, Rubrique « Gestion des comptes auxiliaires et collectifs »"><figcaption><p>Rubrique « Gestion des comptes auxiliaires et collectifs »</p></figcaption></figure>

Cette rubrique rappelle une particularité d'Ingeneo Compta, puis pose une question.

L'écran rappelle : « Ingeneo Compta gère les comptes auxiliaires dans un fichier distinct des comptes généraux. Dans une écriture concernant un tiers, Teogest gère le numéro de compte général (compte collectif) et le numéro de compte auxiliaire. »

La question **« Les écritures exportées sont-elles gérées de la même manière ? »** vous demande si le fichier suit cette même organisation. Désactivez l'interrupteur si les comptes de tiers y figurent dans un seul et même champ.

## Rubrique « Données du modèle »

<figure><img src="../../.gitbook/assets/33-cm385-24-donnees-du-modele.png" alt="Modèles d&#x27;import, Rubrique « Données du modèle »"><figcaption><p>Rubrique « Données du modèle »</p></figcaption></figure>

C'est ici que le modèle prend forme : vous indiquez, pour chaque information attendue par Ingeneo Compta, où la trouver dans le fichier.

Le tableau présente une ligne par information, et cinq colonnes : **Champ Ingeneo Compta**, **Numéro de colonne**, **Pos. du 1er caractère**, **Taille du champ** et **Longueur maximale**.

Les informations attendues pour un plan comptable sont les suivantes ; seule la première est obligatoire :

* **N° de compte** \* — 12 caractères au maximum ;
* **N° de compte auxiliaire** — 12 caractères ;
* **Intitulé du compte** — 50 caractères ;
* **Intitulé 2 du compte** — 50 caractères ;
* **Intitulé du compte auxiliaire** — 50 caractères ;
* **Type de compte** — 9 caractères.

Les colonnes à renseigner dépendent du type de séparation choisi dans la première rubrique. Le logiciel **désactive celles qui sont sans objet** : vous ne pouvez pas vous tromper de colonne.

* pour un fichier à **caractères fixes**, renseignez la **position du premier caractère** et la **taille du champ** ;
* pour un fichier à **séparateur de champs**, renseignez le **numéro de colonne**, c'est-à-dire le rang de l'information sur la ligne. Le logiciel la retrouve à l'aide des séparateurs.

La colonne **Longueur maximale** rappelle la taille qu'Ingeneo Compta peut stocker pour chaque information. Si vous indiquez une taille supérieure, le modèle ne pourra pas être enregistré ; si l'information du fichier est plus longue que la taille indiquée, elle sera tronquée.

## Les actions

bouton **\[Enregistrer]**

Il enregistre le modèle et vous ramène à la liste.

bouton **\[Retour]**

Il revient à la liste sans enregistrer les modifications en cours.

## Autres vues de l'écran

<figure><img src="../../.gitbook/assets/33-cm385-22-changement-des-numeros-de-compte.png" alt="Modèles d&#x27;import, Changement des numéros de compte"><figcaption><p>Changement des numéros de compte</p></figcaption></figure>
