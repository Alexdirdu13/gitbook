# Banque — présentation générale

{% hint style="info" %}
**Où le trouver :** Menu **Relevés bancaires**
{% endhint %}

{% hint style="success" %}
**En bref** — Cette page présente le module « Banque » : récupérer vos lignes de relevés pour les transformer en écritures comptables, et générer les fichiers .XML de virements et de prélèvements SEPA.

* Pour démarrer : choisissez vos fonctionnalités dans le panneau « Paramètres », rubrique « Banque », onglet « Configuration ».
* Pour ouvrir les écrans de paramétrage : utilisez la porte « Paramètres » en bas de la barre de gauche.
{% endhint %}

* il permet de récupérer vos écritures bancaires pour les transformer en écritures comptables et les intégrer à votre logiciel de comptabilité,
* il permet de générer des fichiers .XML à transférer à votre banque pour les virements et les prélèvements SEPA.

<figure><img src="../../.gitbook/assets/34-cm387.png" alt="Écran Relevés bancaires"><figcaption><p>Écran « Relevés bancaires » de la nouvelle interface</p></figcaption></figure>

Les lignes de relevés sont d'abord récupérées, soit par une connexion directe à votre banque, soit par l'import d'un fichier fourni par votre banque.

Une fois que les lignes de relevés ont été récupérées, il faut lancer un traitement qui analyse les lignes au regard de règles de traduction que vous devrez paramétrer. Ces règles permettent de déterminer le compte de contrepartie de chaque écriture de banque.

Pour les lignes pour lesquelles aucune règle de traduction n'a pu être identifiée, vous avez la possibilité d'activer la fonction d'annotations. Cette fonction permet de donner un accès au client du cabinet, qui peut indiquer soit directement une affectation, soit à quelle pièce commerciale correspond le règlement de la ligne de banque.

Pour démarrer avec le module « Banque » vous devez réaliser les étapes suivantes :

* choisir les fonctionnalités que vous voulez activer (panneau « Paramètres », rubrique « Banque », onglet « Configuration »),
* indiquer les comptes bancaires dont vous souhaitez récupérer les écritures (menu « Relevés bancaires », bouton « Autres actions » (trois points) du bas de l'écran, rubrique « Connexion banque »),
* compléter les informations des comptes bancaires pour générer les écritures comptables (panneau « Paramètres », « Données », catégorie « Dossier et comptabilité », « Banques »),
* créer des règles de traduction pour générer des écritures les plus précises possibles (panneau « Paramètres », « Données », catégorie « Intégrations et workflow », « Règles de traduction »),
* créer le fichier des affectations si vous avez activé l'option d'annotations manuelles (panneau « Paramètres », « Données », catégorie « Intégrations et workflow », « Affectations »).

Le module ne possède pas d'écran d'accueil : lorsque vous ouvrez le module « Banque », le logiciel affiche directement la liste des relevés bancaires.

Le menu du module comporte les options suivantes :

* « Relevés bancaires », « Remises de chèques », « Prévisualisations » et « Ecritures », qui ouvrent directement un écran,
* « Paiements », « Traitements », « Editions », « Archives » et « Evénements », qui donnent accès à plusieurs sous-options.

Selon l'écran affiché, certaines de ces entrées sont regroupées dans le menu à trois points « Plus d'entrées », à droite de la barre. Les écrans de paramétrage ne sont plus des entrées de ce menu : ils s'ouvrent dans le panneau « Paramètres », par la porte « Paramètres » en bas de la barre de gauche. L'écran « Annotations » n'est plus proposé dans le menu.

## Autres vues de l'écran

<figure><img src="../../.gitbook/assets/34-cm387-02-bouton-creer-une-regle.png" alt="Banque — présentation générale, Bouton [Créer une règle]"><figcaption><p>Bouton [Créer une règle]</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-03-bouton-filtres.png" alt="Banque — présentation générale, Bouton [Filtres]"><figcaption><p>Bouton [Filtres]</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-04-bouton-vue.png" alt="Banque — présentation générale, Bouton [Vue]"><figcaption><p>Bouton [Vue]</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-05-bouton-exporter.png" alt="Banque — présentation générale, Bouton [Exporter]"><figcaption><p>Bouton [Exporter]</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-06-g-le-tiroir-nouvelle-regle-de-traduction.jpg" alt="Banque — présentation générale, g) Le tiroir « Nouvelle règle de traduction »"><figcaption><p>g) Le tiroir « Nouvelle règle de traduction »</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-07-f-le-tiroir-ligne-de-releve-bancaire.jpg" alt="Banque — présentation générale, f) Le tiroir « Ligne de relevé bancaire »"><figcaption><p>f) Le tiroir « Ligne de relevé bancaire »</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-09-h-le-volet-lier-un-document.jpg" alt="Banque — présentation générale, h) Le volet « Lier un document »"><figcaption><p>h) Le volet « Lier un document »</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-10-d-les-commandes-de-chaque-ligne.png" alt="Banque — présentation générale, d) Les commandes de chaque ligne"><figcaption><p>d) Les commandes de chaque ligne</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-11-rubrique-informations-generales.png" alt="Banque — présentation générale, Rubrique « Informations générales »"><figcaption><p>Rubrique « Informations générales »</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-12-rubrique-choix-de-la-banque.png" alt="Banque — présentation générale, Rubrique « Choix de la banque »"><figcaption><p>Rubrique « Choix de la banque »</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-13-rubrique-analyse-de-la-ligne-de-releve.png" alt="Banque — présentation générale, Rubrique « Analyse de la ligne de relevé »"><figcaption><p>Rubrique « Analyse de la ligne de relevé »</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-14-rubrique-traduction.png" alt="Banque — présentation générale, Rubrique « Traduction »"><figcaption><p>Rubrique « Traduction »</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-15-bouton-enregistrer.png" alt="Banque — présentation générale, Bouton [Enregistrer]"><figcaption><p>Bouton [Enregistrer]</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-16-menu-autres-actions-rubrique-connexion-banque.png" alt="Banque — présentation générale, Menu « Autres actions », rubrique « Connexion banque »"><figcaption><p>Menu « Autres actions », rubrique « Connexion banque »</p></figcaption></figure>

<figure><img src="../../.gitbook/assets/34-cm387-17-menu-autres-actions-entree-rechercher-les-regles.png" alt="Banque — présentation générale, Menu « Autres actions », entrée « Rechercher les règles »"><figcaption><p>Menu « Autres actions », entrée « Rechercher les règles »</p></figcaption></figure>
