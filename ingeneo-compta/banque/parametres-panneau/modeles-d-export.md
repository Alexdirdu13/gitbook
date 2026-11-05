# Modèles d'export

{% hint style="info" %}
**Où le trouver :** Panneau **Paramètres**
{% endhint %}

{% hint style="success" %}
**En bref** — Cet écran définit le format des fichiers servant à exporter vos écritures vers un autre logiciel de comptabilité ; il ne sert que si vous n'utilisez pas la comptabilité du logiciel.

* Pour créer un modèle : bouton \[Nouveau], renseignez les trois rubriques de la fiche, puis bouton \[Enregistrer].
* Pour récupérer les modèles livrés par l'éditeur : bouton \[Charger les nouveaux modèles].
{% endhint %}

Les modèles d'export ne vous sont utiles que si vous n'utilisez pas le module de comptabilité du logiciel. Ils permettent de définir le format des fichiers à générer pour exporter les écritures comptables depuis le menu « Ecritures » vers un autre logiciel.

<figure><img src="../../.gitbook/assets/34-modeles-d-export.png" alt="Écran Modèles d&#x27;export"><figcaption><p>Écran « Modèles d'export » de la nouvelle interface</p></figcaption></figure>

Des modèles standard sont livrés par l'éditeur. Certains d'entre eux, compte tenu de leur complexité, ont fait l'objet d'un développement spécifique : ils ne sont pas modifiables.

L'écran affiche la liste des modèles d'export du dossier, classée par ordre croissant de libellé. Quatre colonnes sont présentées : **Libellé**, **Fichier** qui restitue la nature des données exportées, **Description** et **Modifiable**. Chacune peut servir de critère de tri : cliquez sur son en-tête. La colonne **Modifiable** commande en outre les commandes proposées sur la ligne.

En haut de la colonne de gauche, vous disposez d'une case à cocher qui sélectionne toutes les lignes de la page affichée, d'une seconde case qui étend la sélection à toutes les pages, du pictogramme « Engrenage » qui ouvre la personnalisation des colonnes, du pictogramme « Entonnoir » qui ouvre la fenêtre « Filtres », et du pictogramme « Imprimante » qui lance l'impression de la liste.

Sur une ligne dont la colonne **Modifiable** indique « Oui », vous disposez d'une case à cocher « Sélectionner », du pictogramme « Crayon » qui ouvre la fiche du modèle, du pictogramme « Croix » qui le supprime et du pictogramme « Ajout » qui le duplique.

Sur une ligne dont la colonne **Modifiable** indique « Non » — un modèle livré par l'éditeur —, les pictogrammes « Crayon » et « Ajout » ne vous sont pas proposés : vous ne pouvez donc ni modifier ni dupliquer ce modèle, ni même consulter son paramétrage. La case à cocher et le pictogramme « Croix » restent, eux, affichés.

bouton **\[Nouveau]**

Ouvre la fiche de création d'un modèle d'export.

bouton **\[Charger les nouveaux modèles]**

Installe dans votre dossier les modèles livrés par l'éditeur qui ne s'y trouvent pas encore.

bouton **\[Exporter]**

Produit un fichier à partir des modèles que vous avez cochés dans la liste.

bouton **\[Supprimer]**

Supprime les modèles que vous avez cochés dans la liste.

La fiche d'un modèle, en création comme en modification, présente trois rubriques dans cet ordre : « Informations générales », « Gestion des comptes auxiliaires et collectifs » et « Données du modèle ». La fiche est longue : vous la parcourez avec la barre de défilement.

## Rubrique « Informations générales »

| Champ                                                              | Ce qu'il faut savoir                                                                                                                                                                                                                                                                               |
| ------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Type de fichier**                                                | Il décrit la nature des données exportées, et donc les champs que le fichier sera susceptible de contenir. Depuis le module Banque, une seule valeur vous est proposée : **Brouillard d'écritures**. C'est aussi celle que le logiciel positionne à la création d'un modèle.                       |
| **Libellé**                                                        | C'est sous ce libellé que le modèle est présenté dans la liste et proposé au moment de l'export.                                                                                                                                                                                                   |
| **Description**                                                    | Zone de texte libre, sur plusieurs lignes, où vous pouvez préciser l'usage du modèle.                                                                                                                                                                                                              |
| **Type de séparation**                                             | Les enregistrements du fichier exporté peuvent être construits de deux manières, selon ce qu'attend le logiciel destinataire.                                                                                                                                                                      |
| **Caractères fixes**                                               | Chaque champ occupe sur chaque ligne la même position, quelle que soit la taille effective de son contenu, les caractères inutilisés étant remplis par des espaces. Par exemple la date du caractère 1 à 10, le numéro de compte du caractère 11 à 18, le libellé d'écriture du caractère 19 à 53. |
| **Séparateur de champs**                                           | Les champs n'ont plus de longueur imposée, mais ils doivent tous être séparés par un caractère facilement identifiable. C'est la valeur proposée à la création d'un modèle.                                                                                                                        |
| **Séparateur**                                                     | Affiché uniquement si le type de séparation vaut **Séparateur de champs**. Choisissez dans la liste le caractère qui sépare les champs : **Point**, **Virgule**, **Point-virgule**, **Tabulation**, **Tiret**, **Sous-tiret**, ou **Autre** pour en indiquer un différent.                         |
| **Caractère d'encadrement**                                        | Affiché dans les mêmes conditions que le séparateur. Il permet, en plus du caractère séparateur, de marquer le début et la fin de chaque champ — des guillemets, par exemple.                                                                                                                      |
| **Format des dates (ex. jj/mm/aaaa)**                              | Choisissez dans la liste le format sous lequel les dates seront écrites dans le fichier. Vingt formats vous sont proposés, combinant l'ordre du jour, du mois et de l'année, l'année sur deux ou quatre chiffres, et le séparateur — barre oblique, point, tiret, ou aucun séparateur.             |
| **Séparateur des décimales**                                       | Choisissez **Virgule**, **Point**, ou **Rien** si le fichier ne comporte pas de séparateur décimal.                                                                                                                                                                                                |
| **Nombre de décimales**                                            | Indiquez le nombre de décimales des montants exportés.                                                                                                                                                                                                                                             |
| **Ignorer les données vides**                                      | Répondez « Oui » pour que le logiciel n'écrive rien dans le fichier lorsqu'une donnée est absente.                                                                                                                                                                                                 |
| **Afficher un en-tête**                                            | Répondez « Oui » pour que le fichier généré comporte une première ligne d'en-tête contenant, dans le même ordre, les libellés de tous les champs présents dans le fichier.                                                                                                                         |
| **Supprimer les caractères '0' terminaux des comptes auxiliaires** | Répondez « Oui » si le logiciel destinataire attend les comptes auxiliaires sans les zéros de fin.                                                                                                                                                                                                 |

Les trois derniers paramètres sont positionnés à « Non » à la création d'un modèle.

## Rubrique « Gestion des comptes auxiliaires et collectifs »

Le logiciel gère les comptes auxiliaires dans un fichier distinct des comptes généraux : dans une écriture concernant un tiers, il gère le numéro de compte général — le compte collectif — et le numéro de compte auxiliaire. La rubrique rappelle ce principe à l'écran, puis vous pose une seule question.

**Les écritures exportées sont-elles gérées de la même manière ?** : répondez « Oui » si le fichier attendu distingue lui aussi les deux comptes. Répondez « Non » dans le cas contraire. La réponse est positionnée à « Oui » à la création d'un modèle.

## Rubrique « Données du modèle »

C'est ici que vous finalisez le modèle, en indiquant la place de chaque donnée dans le fichier. Le tableau présente une ligne par champ exportable — vingt-six au total, du **Code journal** à la **Référence des pièces jointes** — et quatre colonnes de paramétrage.

| Champ                     | Ce qu'il faut savoir                                                                                                                                                                                                                                                                                 |
| ------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Champ Ingeneo Compta**  | Le nom de la donnée. Cette colonne ne se saisit pas.                                                                                                                                                                                                                                                 |
| **Numéro de colonne**     | L'ordre de la donnée dans la ligne du fichier. Cette colonne ne se saisit que si le type de séparation vaut **Séparateur de champs** ; elle est grisée dans l'autre mode.                                                                                                                            |
| **Pos. du 1er caractère** | **Taille du champ :** la position du premier caractère de la donnée et sa longueur, en nombre de caractères. Ces deux colonnes ne se saisissent que si le type de séparation vaut **Caractères fixes** ; elles sont grisées dans l'autre mode.                                                       |
| **Longueur maximale**     | La taille maximale gérée par le logiciel pour cette donnée. Cette colonne ne se saisit pas : elle vous sert de référence. Si vous indiquez une taille supérieure, vous ne pourrez pas enregistrer le modèle ; si la donnée est plus longue que la taille que vous avez indiquée, elle sera tronquée. |

La liste des vingt-six champs et leur ordre ne changent pas d'un mode de séparation à l'autre : seules les colonnes saisissables changent.

bouton **\[Enregistrer]**

Enregistre le modèle.

bouton **\[Retour]**

Quitte la fiche sans enregistrer et vous ramène à la liste.

Le pictogramme « Entonnoir » ouvre la fenêtre « Filtres », qui vous permet de restreindre la liste. Vous y retrouvez d'abord les quatre colonnes affichées — **Libellé**, **Fichier**, **Description**, **Modifiable** — puis deux colonnes masquées par défaut, que vous pouvez également utiliser comme critères : **Modèle éditeur** et **Dernière modification**, cette dernière étant un critère de date que vous choisissez au calendrier.

Chaque critère se compose d'un opérateur et d'une valeur, que vous pouvez combiner par « Et » ou « Ou » avec un second couple. La fenêtre offre cinq boutons : bouton **\[Filtrer]** applique les critères à la liste, bouton **\[Mémoriser les paramètres]** conserve la sélection de critères, bouton **\[Charger les paramètres]** la rappelle, bouton **\[Vider les filtres]** efface les critères saisis et bouton **\[Fermer]** referme la fenêtre.
