# Import

{% hint style="info" %}
**Où le trouver :** Menu **Traitements › Import**
{% endhint %}

{% hint style="success" %}
**En bref** — Cet écran importe des données provenant d'un autre outil (clients, fournisseurs, articles, factures clients…) à partir d'un fichier Excel que vous remplissez vous-même.

* Pour préparer l'import : bouton \[Télécharger la trame d'import], puis renseignez les onglets du fichier.
* Pour lancer l'import : bouton \[Importer], puis choisissez le fichier Excel renseigné.
{% endhint %}

Cette option vous permet d'importer dans le logiciel des données provenant d'un autre outil, à partir d'un fichier Excel que vous remplissez vous-même.

<figure><img src="../../.gitbook/assets/18-cm834.jpg" alt="Écran Import"><figcaption><p>Écran « Import » de la nouvelle interface</p></figcaption></figure>

Le logiciel vous indique la marche à suivre en quatre étapes :

* « Pour procéder à un import, téléchargez le fichier Excel contenant les trames d'import de chaque fichier ainsi que la notice explicative décrivant les caractéristiques de chaque champ. »
* « Remplissez ensuite les différents onglets avec les données à importer. »
* « Réalisez ensuite l'import. »
* « Le logiciel éditera un rapport d'import avec le nombre d'enregistrements importés pour chaque fichier. S'il a détecté des erreurs, il indiquera pour chacune d'entre-elles, l'onglet concerné, la ligne où se trouve l'erreur et sa nature. »

Un pictogramme d'information est placé en fin de première ligne. En le survolant, vous obtenez la liste des fichiers que vous pouvez importer depuis cette option.

## Les fichiers que vous pouvez importer

Le logiciel vous propose d'importer les fichiers suivants :

* Clients ;
* Adresses des clients ;
* Banques des clients ;
* Fournisseurs ;
* Adresses des fournisseurs ;
* Banques des fournisseurs ;
* Articles ;
* Articles - Prix de catalogues ;
* Articles - Comptes comptables ;
* Factures clients.

Cette liste est propre à la « Gestion commerciale ». Le même écran est employé par d'autres modules, où les fichiers proposés ne sont pas les mêmes : fiez-vous toujours à l'infobulle affichée dans le module où vous vous trouvez.

Le fichier Excel comporte un onglet par fichier, ainsi qu'un onglet « Notes » qui décrit les caractéristiques attendues de chaque champ. Le nombre d'onglets qu'il contient ne correspond pas nécessairement à la liste ci-dessus.

## Bouton \[Télécharger la trame d'import]

Commencez par là. Le logiciel vous remet le fichier Excel contenant les trames d'import et leur notice. Enregistrez-le sur votre poste, puis renseignez les onglets correspondant aux fichiers que vous voulez importer.

Ne modifiez ni les onglets ni les intitulés de colonnes de la trame : c'est sur eux que le logiciel s'appuie pour reconnaître vos données.

## Bouton \[Importer]

Il ouvre la fenêtre « Import Gestion commerciale », qui comporte un seul champ :

**Fichier** : champ obligatoire. Choisissez sur votre poste le fichier Excel que vous avez renseigné. Seul le format Excel est accepté.

Dans cette fenêtre, le bouton **\[Importer]** lance l'import et le bouton **\[Annuler]** la referme sans rien importer.

{% hint style="warning" %}
Attention : c'est une opération de grande portée. Le logiciel crée dans votre dossier l'ensemble des données contenues dans les onglets renseignés — y compris les **factures clients** — et il n'existe pas de bouton pour revenir en arrière. Vérifiez votre fichier avant de le déposer, et faites un premier essai sur un petit nombre de lignes.
{% endhint %}

À l'issue de l'import, le logiciel affiche la fenêtre « Rapport d'import Gestion commerciale ». Elle rappelle le nom du fichier traité, puis indique soit que l'import s'est correctement déroulé, soit qu'il a rencontré des erreurs. Son bouton **\[Fermer]** recharge l'écran, sur lequel le rapport détaillé vous attend.

Si le fichier que vous déposez est protégé par un mot de passe, le logiciel refuse l'import et affiche en rouge, dans la fenêtre, le message « Le fichier \<nom de votre fichier> est protégé par un mot de passe. ». Le message « Une erreur est survenue. » signale un incident d'ordre général : reprenez alors l'opération depuis l'écran.

## Droits d'accès

Les trois boutons de cet écran dépendent chacun d'un droit distinct : selon votre profil, vous pouvez par exemple pouvoir télécharger la trame sans pouvoir réaliser l'import. Si l'un d'eux ne vous apparaît pas, adressez-vous à l'administrateur de votre logiciel.
