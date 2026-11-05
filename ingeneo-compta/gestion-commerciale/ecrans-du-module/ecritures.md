# Ecritures

{% hint style="info" %}
**Où le trouver :** Menu **Ecritures**
{% endhint %}

{% hint style="success" %}
**En bref** — Cet écran contient les écritures produites par la validation de vos pièces lorsqu'elles ne sont pas générées directement dans le module Comptabilité, et permet de les exporter vers un logiciel de comptabilité.

* Pour exporter les écritures : bouton \[Exporter], puis indiquez le modèle d'export.
{% endhint %}

## Si vous utilisez la comptabilité Ingeneo Compta

<figure><img src="../../.gitbook/assets/18-cm400.jpg" alt="Écran Ecritures"><figcaption><p>Écran « Ecritures » de la nouvelle interface</p></figcaption></figure>

L'écran n'affiche alors qu'un message, et rien d'autre : « Vous avez indiqué que vous utilisez le module comptabilité. Pour visualiser les écritures, veuillez vous rendre dans ce module. » Ni liste, ni filtre, ni bouton.

C'est le fonctionnement normal, et non une anomalie : vos écritures ont été enregistrées directement dans le module Comptabilité au moment de la validation des pièces, il n'y a donc rien à exporter ici. C'est dans le module de comptabilité que vous les retrouvez.

Ce que vous voyez sur cet écran dépend donc entièrement d'un seul paramètre du dossier annuel, celui du menu « Paramètres », option « Connexion comptabilité », qui indique si vous utilisez la comptabilité Ingeneo Compta. Si vous attendiez la liste des écritures et que vous obtenez ce message, c'est ce paramètre qu'il faut contrôler.

## Si vous n'utilisez pas la comptabilité Ingeneo Compta

L'écran présente la liste des écritures en attente d'export, précédée d'un tableau récapitulatif des totaux et d'une zone de filtres.

| Champ                              | Ce qu'il faut savoir                                                                                                                                                                                                                                                                                                        |
| ---------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Journal**                        | Il vous permet de restreindre la liste à un code journal. Le choix « Tous » regroupe toutes les écritures du container en attente d'export.                                                                                                                                                                                 |
| **Origine**                        | Il vous permet de restreindre la liste aux écritures générées par un des modules Ingeneo Compta. Seuls les modules ayant réellement produit des écritures vous sont proposés, et c'est le module dans lequel vous travaillez qui vous est proposé par défaut. Le choix « Tous » regroupe toutes les écritures du container. |
| **Date de début**                  | **Date de fin :** bornes de la période à afficher. Le logiciel vous propose par défaut les dates de début et de fin de saisie du dossier annuel.                                                                                                                                                                            |
| **Avec les lignes déjà exportées** | <p>Répondez Oui pour faire figurer dans la liste les écritures qui ont déjà fait l'objet d'un export. La proposition par défaut est Non : vous ne voyez donc que ce qui reste à exporter.<br>bouton <strong>[Afficher]</strong> : il applique les filtres et recharge la liste.</p>                                         |
| **Totaux**                         | Le tableau placé au-dessus de la liste porte le total des débits, le total des crédits et le solde. Ils sont là pour contrôle. Si d'aventure le solde n'était pas égal à zéro, contactez le service technique Ingeneo Compta.                                                                                               |

bouton **\[Exporter]** : il produit le fichier des écritures que vous pourrez ensuite importer dans votre logiciel de comptabilité. Indiquez le modèle d'export sur la base duquel vous souhaitez exporter, ainsi que l'origine des écritures à exporter : vous pouvez n'exporter que celles générées par le module en cours, ou toutes les écritures présentes. Si le modèle d'export dont vous avez besoin ne figure pas dans la liste, vous pouvez le créer dans le menu « Paramètres », option « Modèles d'export ». Lorsque le fichier est produit, enregistrez-le sur votre poste.

Ce bouton est soumis à un droit distinct de celui du menu : selon votre profil, il peut ne pas vous être proposé.
