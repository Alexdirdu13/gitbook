# Annotations

{% hint style="success" %}
**En bref** — Cet écran rapproche les lignes de relevés non reconnues des événements clients et fournisseurs, ou leur attribue une affectation ; il peut être ouvert aux clients du cabinet.

* Pour rapprocher : cochez une ligne de banque et l'événement correspondant, vérifiez les deux « Total de la sélection : », puis bouton \[Valider le rapprochement].
* Pour affecter une ligne : cliquez sur sa cellule « Affectation », choisissez l'affectation, puis bouton \[Enregistrer].
* Pour rapprocher d'une remise de chèques : cochez une seule ligne de banque, puis bouton \[Appeler une remise de chèques].
{% endhint %}

## La barre de filtres

Une seule ligne, au-dessus des deux listes, porte quatre zones. Les deux premières, à gauche, concernent la liste des lignes de banque ; les deux dernières, à droite, concernent la liste des événements.

| Champ                     | Ce qu'il faut savoir                                                                                                             |
| ------------------------- | -------------------------------------------------------------------------------------------------------------------------------- |
| **Total de la sélection** | (à gauche) le logiciel cumule ici le montant des lignes de banque que vous avez sélectionnées. Cette zone n'est pas saisissable. |
| **Banque**                | N'affiche que les lignes du compte bancaire choisi. Le choix « Toutes » est proposé par défaut.                                  |
| **Total de la sélection** | (à droite) le logiciel cumule ici le montant des événements que vous avez sélectionnés. Cette zone n'est pas saisissable.        |
| **Type d'événement**      | N'affiche que les événements de la nature choisie : « Tous », « Evénements clients » ou « Evénements fournisseurs ».             |

## La liste « Lignes de banque »

Elle contient les lignes de relevés bancaires auxquelles aucune règle de traduction n'a été associée. Elle comporte les colonnes suivantes, toutes triables en cliquant sur leur en-tête :

| Champ                | Ce qu'il faut savoir                                                                                                                                                                                                                                  |
| -------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Date**             | Date de l'opération.                                                                                                                                                                                                                                  |
| **Libellé**          | Libellé de l'opération tel que la banque l'a communiqué.                                                                                                                                                                                              |
| **Montant**          | Montant de l'opération. Le logiciel l'affiche en vert pour un crédit et en rouge pour un débit.                                                                                                                                                       |
| **Affectation**      | Affectation retenue pour la ligne.                                                                                                                                                                                                                    |
| **Evénements**       | Événements rapprochés de la ligne.                                                                                                                                                                                                                    |
| **Référence**        | <p>Référence de l'opération. Cette dernière colonne n'est visible qu'en faisant défiler la liste horizontalement.<br>La case à cocher de l'en-tête sélectionne toutes les lignes de la page affichée. Chaque ligne porte ensuite deux commandes :</p> |
| **Sélectionner**     | Coche la ligne en vue du rapprochement.                                                                                                                                                                                                               |
| **Eclater la ligne** | Permet de répartir une même ligne de banque sur plusieurs montants, lorsqu'elle correspond à plusieurs pièces.                                                                                                                                        |

Pour affecter une ligne de banque, cliquez sur sa cellule « Affectation » ou sur sa cellule « Référence » : le logiciel ouvre la fenêtre « Affectation de lignes de banque », décrite au paragraphe d). Une ligne déjà rapprochée d'un événement ne peut plus être affectée : le clic reste alors sans effet.

## La liste « Evénements »

Elle contient les événements clients et fournisseurs issus des modules de facturation, de gestion commerciale et de reconnaissance de documents, qui ont été validés dans ces modules. Elle comporte les colonnes suivantes, toutes triables :

| Champ              | Ce qu'il faut savoir                                                                                                                                          |
| ------------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Date**           | Date de la pièce.                                                                                                                                             |
| **Nature**         | Nature de la pièce, par exemple « Facture client », « Avoir client » ou « Facture fournisseur ».                                                              |
| **Raison sociale** | Tiers concerné par la pièce.                                                                                                                                  |
| **Libellé**        | Libellé de la pièce.                                                                                                                                          |
| **Montant**        | <p>Montant de la pièce.<br>La case à cocher de l'en-tête sélectionne tous les événements de la page affichée. Chaque ligne porte ensuite deux commandes :</p> |
| **Sélectionner**   | Coche l'événement en vue du rapprochement.                                                                                                                    |
| **Supprimer**      | Retire l'événement de la liste.                                                                                                                               |

Tous les événements importés correspondent à des pièces déjà validées dans d'autres modules ; ces pièces ont donc déjà généré des écritures comptables. C'est la raison pour laquelle vous pouvez les supprimer sans conséquence si vous estimez qu'elles n'ont plus de raison d'être rapprochées, par exemple lorsqu'elles sont antérieures à la mise en place des annotations.

## La fenêtre « Affectation de lignes de banque »

Cette fenêtre vous permet d'indiquer vous-même la contrepartie d'une ligne de relevé, lorsqu'aucune règle de traduction ne l'a reconnue. Elle est surtout destinée aux clients du cabinet, qui connaissent l'origine de l'opération.

| Champ           | Ce qu'il faut savoir                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                 |
| --------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Affectation** | <p>Saisissez le libellé de l'affectation, ou choisissez-la avec la loupe de recherche. Les affectations sont créées dans le menu « Fichiers », sous-option « Affectations ».<br>La loupe ouvre la fenêtre « Sélection d'une affectation » : une zone <strong>Affectation :</strong> et son bouton <strong>[Afficher]</strong> vous permettent de restreindre la liste « Libellé » qui figure au-dessous, et la mention « Cliquez pour sélectionner » vous rappelle qu'un clic sur une ligne de cette liste la retient.<br>Une fois l'affectation choisie, le logiciel affiche les zones <strong>N° de compte :</strong> et <strong>Intitulé :</strong> qu'elle porte. Les zones <strong>N° de compte auxiliaire :</strong> et son <strong>Intitulé :</strong> n'apparaissent que si l'affectation porte un compte auxiliaire. Ces zones ne sont pas modifiables : la ligne de contrepartie qui sera générée sera imputée au compte paramétré dans l'affectation.</p> |
| **Référence**   | Si vous ne trouvez aucune affectation qui convienne, saisissez ici un texte libre de trente caractères au plus. Le logiciel vous rappelle que « Le texte indiqué ici sera inséré dans le champ « Référence » de l'écriture qui sera générée dans le compte d'attente. ». Cette possibilité évite de conserver des lignes pour lesquelles vous n'avez pas d'information complémentaire à indiquer.                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                    |

Le bouton **\[Enregistrer]** enregistre l'affectation ; le bouton **\[Annuler]** ferme la fenêtre sans rien conserver.

## Ce que ces deux listes ne proposent pas

Contrairement aux autres listes du module, aucune des deux ne propose de personnalisation de colonnes, de fenêtre de filtres ni d'impression : les colonnes affichées sont celles décrites ci-dessus, et vous ne pouvez ni en ajouter, ni en régler la largeur.

## Les boutons de bas d'écran

bouton **\[Valider le rapprochement]**

Pour rapprocher des lignes de relevés et des événements, cochez les lignes à mettre en relation dans les deux listes, puis cliquez sur ce bouton.

Les deux zones **Total de la sélection :** vous permettent de vérifier, avant de valider, que le montant retenu à gauche correspond bien à celui retenu à droite.

La ligne de contrepartie qui sera générée sera imputée au compte de tiers de l'événement associé.

Ce bouton ne devient utilisable qu'à partir du moment où vous avez coché au moins une ligne de banque : tant que vous n'avez rien coché, un clic reste sans effet et le logiciel n'affiche aucun message.

Une ligne de banque qui porte déjà une affectation, ou qui est déjà rapprochée d'un événement, ne peut pas être sélectionnée pour un nouveau rapprochement.

bouton **\[Appeler une remise de chèques]**

Ce bouton ouvre la fenêtre « Appeler une remise de chèques », qui vous permet de rapprocher une ligne de banque d'une remise de chèques préparée dans l'option « Remises de chèques » du module.

Il ne devient utilisable que si vous avez coché **une seule** ligne de banque : une remise de chèques se rapproche d'une ligne à la fois.

Ce bouton n'est proposé qu'aux utilisateurs qui en ont le droit.

bouton **\[Annuler]**

Ce bouton abandonne la sélection en cours.
