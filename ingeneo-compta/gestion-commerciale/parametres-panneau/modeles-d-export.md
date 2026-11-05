# Modèles d'export

{% hint style="info" %}
**Où le trouver :** Panneau **Paramètres**
{% endhint %}

{% hint style="success" %}
**En bref** — Cet écran gère les modèles d'import et d'export, fournis par Ingeneo Compta ou créés par vous, qui décrivent la forme des fichiers produits, notamment pour l'export des écritures.

* Pour créer un modèle : bouton \[Créer un modèle], puis choisissez le type de fichier.
* Pour récupérer les modèles fournis par Ingeneo Compta manquants : bouton \[Charger les nouveaux modèles].
{% endhint %}

Cette option permet de gérer les modèles d'import et d'export fournis par Ingeneo Compta — dont les modèles d'export d'écritures —, et de créer vos propres modèles. Un modèle d'export décrit la forme du fichier à produire : la façon dont les champs y sont séparés, le format des dates et des nombres, et l'ordre ou la position de chaque champ dans la ligne.

<figure><img src="../../.gitbook/assets/18-modeles-d-export.jpg" alt="Écran Modèles d&#x27;export"><figcaption><p>Écran « Modèles d'export » de la nouvelle interface</p></figcaption></figure>

Certains modèles, compte tenu de leur complexité, ont fait l'objet d'un développement spécifique : ils ne sont ni modifiables ni duplicables. La liste vous le dit, colonne **Modifiable**.

Un modèle paramétré ici ne produit aucun fichier par lui-même : il est proposé au moment de l'export, dans le menu « Ecritures ». C'est donc l'écran où vous vous servirez de ce que vous paramétrez ici.

Cet écran se trouve dans le panneau « Paramètres » : rubrique « Modèles », puis l'onglet du haut « Imports et exports », entrée « Écritures ». Il est commun à plusieurs modules : il présente les modèles de tous les types de fichier du dossier (écritures, balances, comptes…), à l'import comme à l'export.

L'écran présente la liste des modèles du dossier (imports et exports, tous types de fichier confondus), une ligne par modèle, avec quatre colonnes : **Libellé**, **Fichier** — le type de fichier produit —, **Description** et **Modifiable**. La liste est triée par défaut sur le libellé, par ordre croissant.

Au-dessus de la liste, la barre « Rechercher un modèle… » filtre à la saisie, et le bouton \[Filtres] permet de composer des critères. Deux rangées de boutons, à côté de \[Filtres], restreignent la liste d'un clic : « Tous / Import / Export » pour le sens du modèle, et « Tous / Balance / Brouillard d'écritures / Comptes / Ecritures / Fichier des écritures comptables » pour le type de fichier. Les boutons \[Vue] et \[Exporter] complètent la barre d'outils.

Un clic sur une ligne la sélectionne ; aucune case à cocher n'est affichée. Au survol d'une ligne, le menu « Autres actions » (trois points) propose « Modifier », « Dupliquer » et « Supprimer ». Sur un modèle dont la colonne **Modifiable** indique **Non**, ce menu ne propose que « Supprimer » : ce modèle ne peut être ni ouvert ni dupliqué. C'est la lecture de cette colonne qui vous dit à l'avance ce que vous pourrez faire d'une ligne.

La duplication est le moyen de partir d'un modèle existant pour en obtenir un autre, que vous adaptez ensuite ; elle n'est donc pas disponible sur les modèles non modifiables.

bouton **\[Créer un modèle]**

Placé dans la barre du bas, à droite, il déploie vers le haut un menu de cinq types de fichier : « Balance », « Brouillard d'écritures », « Comptes », « Ecritures » et « Fichier des écritures comptables ». Choisissez dans ce menu le type de fichier du nouveau modèle.

bouton **\[Charger les nouveaux modèles]**

Placé à côté de \[Créer un modèle], il récupère dans votre dossier les modèles fournis par Ingeneo Compta qui n'y figurent pas encore. Utilisez-le si un modèle standard attendu n'apparaît pas dans la liste.

bouton **\[Exporter]**

Situé dans la barre d'outils au-dessus de la liste, après \[Vue], il exporte le contenu de la liste des modèles affichée à l'écran. Il ne s'agit pas d'exporter des écritures : c'est la liste elle-même qui est reprise dans un fichier.

bouton **\[Supprimer]**

Il apparaît dans le bandeau de sélection, au bas de l'écran (« 1 modèle sélectionné », lien « Tout désélectionner »), qui remplace alors \[Créer un modèle] et \[Charger les nouveaux modèles]. Il supprime les modèles sélectionnés dans la liste.

## Rubrique « Informations générales »

<figure><img src="../../.gitbook/assets/18-cm385-11-informations-generales.png" alt="Modèles d&#x27;export, Rubrique « Informations générales »"><figcaption><p>Rubrique « Informations générales »</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/18-cm385-12-informations-generales.png" alt="Modèles d&#x27;export, Rubrique « Informations générales »"><figcaption><p>Rubrique « Informations générales »</p></figcaption></figure>

La rubrique regroupe d'abord le type de fichier, le libellé et la description, puis deux cartes : « Structure du fichier » (type de séparation, séparateur, caractère d'encadrement, format des dates, séparateur des décimales, nombre de décimales) et « Lignes et valeurs » (les trois interrupteurs).

| Champ                                                              | Ce qu'il faut savoir                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| ------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| **Type de fichier**                                                | Il décrit la nature des éléments exportés, et donc les champs que le fichier sera susceptible de contenir. Il se choisit à la création, par le menu de \[Créer un modèle] ; sur la fiche d'un modèle existant, il est grisé (par exemple « Brouillard d'écritures »).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                |
| **Libellé**                                                        | C'est sous ce nom que le modèle apparaîtra dans la liste, et au moment de choisir un modèle pour un export.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Description**                                                    | Zone de plusieurs lignes.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                            |
| **Type de séparation**                                             | <p>Deux boutons côte à côte, <strong>Caractères fixes</strong> et <strong>Séparateur de champs</strong>. Les enregistrements du fichier exporté peuvent en effet être construits de deux manières, selon le fichier à produire :<br>• soit avec des <strong>longueurs fixes</strong> : chaque champ occupe alors la même position sur chaque ligne — par exemple la date du caractère 1 au caractère 10, le numéro de compte du 11 au 18, le libellé d'écriture du 19 au 53 — et ce, quelle que soit la taille effective du contenu, les caractères inutilisés étant remplis par des espaces ;<br>• soit avec des <strong>longueurs variables</strong>, sans espaces inutilisés, mais dans ce cas tous les champs doivent être séparés par un caractère facilement identifiable.</p> |
| **Séparateur**                                                     | Lorsque le type de séparation est « Séparateur de champs ». Les caractères les plus courants vous sont proposés — **Point**, **Virgule**, **Point-virgule**, **Tabulation**, **Tiret**, **Sous-tiret** — et le choix **Autre** vous permet d'en indiquer un différent.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                               |
| **Caractère d'encadrement**                                        | Il permet, en plus du caractère séparateur, d'encadrer le début et la fin de chaque champ, par des guillemets par exemple.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                           |
| **Format des dates (ex. jj/mm/aaaa)**                              | Choisissez le format dans lequel les dates doivent figurer dans le fichier produit. Les formats proposés couvrent les trois ordres de jour, mois et année, l'année sur deux ou quatre chiffres, et quatre séparateurs — barre oblique, point, tiret, ou aucun : JJ/MM/AAAA, JJ.MM.AAAA, JJMMAAAA, JJ/MM/AA, JJ.MM.AA, JJMMAA, MM/JJ/AAAA, MM.JJ.AAAA, MMJJAAAA, AAAA/MM/JJ, AAAA.MM.JJ, AAAAMMJJ, AA/MM/JJ, AA.MM.JJ, AAMMJJ, JJ-MM-AA, JJ-MM-AAAA, MM-JJ-AAAA, AA-MM-JJ et AAAA-MM-JJ.                                                                                                                                                                                                                                                                                              |
| **Séparateur des décimales**                                       | Trois choix, **Virgule**, **Point** et **Rien**. Le choix « Rien » produit des montants sans séparateur décimal, les décimales étant collées à la partie entière.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Nombre de décimales**                                            | —                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |
| **Ignorer les données vides**                                      | Interrupteur sans texte (désactivé sur le modèle « Export des écritures »).                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                          |
| **Afficher un en-tête**                                            | Interrupteur sans texte. Activé, le fichier produit comporte une première ligne d'en-tête contenant, dans le même ordre, les libellés de tous les champs présents dans le fichier.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                   |
| **Supprimer les caractères '0' terminaux des comptes auxiliaires** | Interrupteur sans texte. Activé, les zéros de fin des numéros de comptes auxiliaires ne sont pas repris dans le fichier produit.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                     |

## Rubrique « Comptes auxiliaires et collectifs »

<figure><img src="../../.gitbook/assets/18-cm385-13-comptes-auxiliaires-et-collectifs.png" alt="Modèles d&#x27;export, Rubrique « Comptes auxiliaires et collectifs »"><figcaption><p>Rubrique « Comptes auxiliaires et collectifs »</p></figcaption></figure>

La rubrique rappelle d'abord comment le logiciel tient les comptes de tiers : Ingeneo Compta gère les comptes auxiliaires dans un fichier distinct des comptes généraux, et dans une écriture concernant un tiers il gère le numéro de compte général — le compte collectif — et le numéro de compte auxiliaire.

**Les écritures exportées sont-elles gérées de la même manière ?** : interrupteur sans texte, que l'écran affiche sous l'intitulé « ComptesAuxiliairesSepares » (la question ci-contre n'y apparaît pas). Activez-le si le logiciel destinataire du fichier distingue, comme Ingeneo Compta, le compte collectif et le compte auxiliaire.

## Rubrique « Données du modèle »

<figure><img src="../../.gitbook/assets/18-cm385-14-donnees-du-modele.png" alt="Modèles d&#x27;export, Rubrique « Données du modèle »"><figcaption><p>Rubrique « Données du modèle »</p></figcaption></figure>

Pour finaliser le modèle, il faut indiquer la place de chaque champ dans la ligne du fichier. La rubrique présente une ligne par champ exportable, avec cinq colonnes : **Champ Ingeneo Compta**, **Numéro de colonne**, **Pos. du 1er caractère**, **Taille du champ** et **Longueur maximale**.

Si le type de séparation est « Séparateur de champs », vous indiquez pour chaque champ son **numéro de colonne**, c'est-à-dire son numéro d'ordre dans les lignes du fichier exporté.

Si le type de séparation est « Caractères fixes », vous indiquez pour chaque champ la **position de son premier caractère** et sa **taille** en nombre de caractères. La **longueur maximale** gérée par le logiciel est rappelée sur chaque ligne.

Les colonnes qui ne servent pas au type de séparation retenu apparaissent grisées : c'est ce qui vous indique celles que vous avez à renseigner.

Vous n'êtes pas tenu de reprendre tous les champs : laissez sans position ceux dont le fichier destinataire n'a pas besoin.

Les champs proposés sont, dans l'ordre d'affichage : Code journal, Libellé journal, N° écriture, Date écriture, N° compte, Intitulé compte, N° de compte auxiliaire, Intitulé du compte auxiliaire, Référence, Date de la pièce, Libellé écriture, Débit, Crédit, Lettre, Date lettrage, Date validation, Montant devise, Devise, Quantité 1, Code quantité 1, Quantité 2, Code quantité 2, Date échéance, Taux de TVA, Date export et Référence des pièces jointes.

Le logiciel gère en outre des champs propres au format attendu par le logiciel de comptabilité Quadra, qui ne sont pas proposés sur ce modèle : ils n'apparaissent que sur les modèles destinés à ce format.

bouton **\[Enregistrer]**

Placé dans la barre du bas, à droite, il enregistre le modèle d'export.

**Chevron « Retour »**

Placé à gauche de la barre d'onglets du panneau, il revient à la liste sans enregistrer les modifications en cours (le bouton \[Retour] de la fiche est masqué).
