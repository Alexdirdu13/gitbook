# Événements fournisseurs

{% hint style="info" %}
**Où le trouver :** Menu **Evénements › Fournisseurs**
{% endhint %}

{% hint style="success" %}
**En bref** — Cet écran liste les événements fournisseurs (factures et avoirs validés dans d'autres modules), mis à disposition pour être rapprochés de vos lignes de relevés bancaires.

* Pour récupérer les nouveaux événements : bouton \[Importer].
* Pour écarter des pièces inutiles : sélectionnez-les, puis bouton \[Supprimer].
* Pour consulter la pièce d'origine : pictogramme « Télécharger » de la ligne.
{% endhint %}

Cet écran est commun aux options « Clients » et « Fournisseurs » du menu « Evénements ».

<figure><img src="../../.gitbook/assets/34-cm819 (1).jpg" alt="Écran Fournisseurs"><figcaption><p>Écran « Fournisseurs » de la nouvelle interface</p></figcaption></figure>

Cette option présente les **événements fournisseurs** du dossier : les pièces fournisseurs déjà validées dans les autres modules du logiciel, mises à disposition ici pour être rapprochées des lignes de vos relevés bancaires. Les pièces proviennent des modules « OCR », « Facturation » et « Gestion commerciale ».

Un événement ne se saisit pas : il arrive par import. L'écran ne propose donc ni bouton de création, ni fiche de consultation — il n'existe pas d'écran de détail d'un événement.

Cette option ne vous est proposée que si vous avez répondu « Oui » aux deux premières questions de la rubrique « Annotations manuelles » du panneau « Paramètres », rubrique « Banque », onglet « Configuration » : **Souhaitez-vous gérer les annotations manuelles ?** et **Souhaitez-vous importer les événements clients et fournisseurs pour faciliter le processus d'annotation ?**. C'est également là que vous choisissez, par le champ **Méthode d'import des événement fournisseurs**, si l'import est fait _Automatiquement_ par le logiciel ou _Manuellement_ par vos soins depuis le présent écran.

**a) La liste des événements**

L'écran se réduit à un seul tableau : il n'y a pas d'onglet, et seule la barre de la liste, décrite plus bas, se trouve au-dessus du tableau.

Les colonnes affichées sont les suivantes :

* **Date** : date de la pièce. C'est le tri initial de la liste, par ordre croissant.
* **Référence** : référence de la pièce d'origine (numéro de facture, par exemple).
* **SIREN** : numéro SIREN du fournisseur, lorsqu'il est connu. Il peut être vide.
* **Raison sociale** : nom du fournisseur.
* **Nature** : nature de la pièce à l'origine de l'événement : « Facture fournisseur » ou « Avoir fournisseur ».
* **Montant** : montant de la pièce.
* **Rapprochement** : cette colonne porte l'information de rapprochement de l'événement avec une ligne de relevé bancaire.

Toutes ces colonnes sont triables, et vous pouvez les réordonner ou en masquer par le bouton « Vue » (voir ci-dessous). Il n'existe pas de colonne supplémentaire à activer : la liste des colonnes disponibles est exactement celle qui s'affiche.

Le bas du tableau indique le nombre d'événements et vous permet de passer d'une page à l'autre.

**b) Les commandes de l'en-tête**

La barre placée au-dessus du tableau comporte :

* le champ « Rechercher un tiers… », qui restreint la liste aux événements correspondants ;
* le bouton **\[Filtres]**, qui ouvre le volet des critères de la liste ;
* le bouton **\[Vue]**, qui ouvre le menu de présentation de la liste (recherche d'une colonne, enregistrement de la vue actuelle, retour aux colonnes d'origine, bouton **\[Appliquer]**) ;
* le bouton **\[Exporter]**, dont le menu offre « Aperçu édition HTML », « Imprimer », « Exporter en Excel », « Exporter en PDF » et « Envoyer la liste par e-mail ».

Il n'y a plus de case à cocher : un clic sur une ligne la sélectionne, et les liens « Sélectionner la page » et « Tout sélectionner (N) », sous le tableau, sélectionnent les lignes de la page affichée ou de toute la liste.

**c) Les commandes de chaque ligne**

Chaque ligne porte deux commandes :

* le pictogramme « Télécharger » (une flèche vers le bas, visible au survol de la ligne) : il télécharge le document d'origine de l'événement ;
* le menu ⋮ « Autres actions », qui propose « Supprimer » pour supprimer l'événement.

Il n'y a pas de commande « Modifier » : un événement ne s'ouvre pas et ne se corrige pas depuis cet écran.

**d) Les boutons de bas d'écran**

bouton **\[Importer]**

Il enrichit la liste des nouveaux événements fournisseurs, sans passer par un écran intermédiaire : le traitement est lancé immédiatement, et le logiciel vous répond par un message indiquant le nombre d'événements importés, ou _« Aucun événement n'a été importé. »_ s'il n'a rien trouvé de nouveau.

C'est le bouton à utiliser si vous avez choisi l'import _Manuellement_ dans les paramètres (panneau « Paramètres », rubrique « Banque », onglet « Configuration »). Aucun événement n'est importé si le dossier annuel en cours est clôturé.

bouton **\[Supprimer]**

Il supprime les événements que vous avez sélectionnés. Il se trouve dans le bandeau de sélection, qui apparaît en bas de l'écran dès qu'une ligne est sélectionnée.

Les événements correspondent à des pièces déjà validées dans les autres modules du logiciel : elles ont donc déjà donné lieu à leurs propres écritures comptables. Supprimer un événement de cette liste ne remet pas la pièce en cause — cela retire seulement la possibilité de la rapprocher d'une ligne de relevé bancaire. C'est utile, par exemple, pour écarter les pièces antérieures à la mise en place du rapprochement.

Les commandes de cet écran dépendent de votre profil : selon les droits qui vous ont été accordés, certaines peuvent ne pas vous être proposées.
