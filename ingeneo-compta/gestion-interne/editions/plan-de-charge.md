# Plan de charge

{% hint style="info" %}
**Où le trouver :** Menu **Editions › Plan de charge**
{% endhint %}

{% hint style="success" %}
**En bref** — Le plan de charge affiche à l'écran, collaborateur par collaborateur et jour par jour, le taux d'occupation de votre équipe, pour repérer sous-charge et saturation.

* Pour consulter une période : choisissez le Mois et l'Année, éventuellement un groupe de travail, puis lisez la couleur de chaque case.
* Pour voir le taux chiffré : activez « % d'affectation ».
* Pour voir le détail d'une journée : cliquez sur une case portant une affectation, la fenêtre « Tâches collaborateur » s'ouvre.
{% endhint %}

Cette option vous montre, collaborateur par collaborateur et jour par jour, le taux d'occupation de votre équipe. Vous y voyez d'un coup d'œil qui est en sous-charge, qui est à saturation, et sur quelles périodes.

<figure><img src="../../.gitbook/assets/16-cm618.jpg" alt="Écran Plan de charge"><figcaption><p>Écran « Plan de charge » de la nouvelle interface</p></figcaption></figure>

Bien qu'elle figure dans le menu « Editions », cette option n'est pas une édition : elle n'ouvre pas de fenêtre de format et ne produit ni document ni fichier. Les critères sont en haut de l'écran, le plan de charge s'affiche directement en dessous.

## Les critères de l'affichage

Les critères tiennent sur une ligne, au-dessus du plan. Les cinq listes n'ont pas de libellé à l'écran : chacune porte un pictogramme, et son nom n'apparaît qu'en infobulle. Les deux interrupteurs qui les suivent portent un libellé court, leur nom complet n'apparaissant lui aussi qu'en infobulle.

**Mois** et **Année** : ils déterminent la période affichée. Les douze mois vous sont proposés, et les années de 2013 à 2027. À l'ouverture, le logiciel se place sur le mois et l'année en cours.

| Champ                  | Ce qu'il faut savoir                                                                                                                                                                                                             |
| ---------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **Groupes de travail** | Restreint le plan aux collaborateurs d'un groupe. Son nom est au pluriel, mais la liste ne retient qu'un seul groupe à la fois ; la valeur « Tous » ne restreint rien.                                                           |
| **Collaborateurs**     | Restreint le plan à un collaborateur. Là encore, la liste n'en retient qu'un seul ; la valeur « Collaborateur », affichée tant que personne n'est choisi, ne restreint rien.                                                     |
| **Mode d'affichage**   | Trois valeurs — **Jour**, **Semaine** ou **Mois**. C'est la maille sur laquelle la charge est présentée : en mode **Semaine** ou **Mois**, le taux affiché est la moyenne des taux journaliers de la période, et non leur cumul. |

**Week-end**, dont l'infobulle dit « Afficher les week-end » : ajoute ou retire les samedis et dimanches des colonnes de jours. Il est activé à l'ouverture, et ces deux colonnes se distinguent alors des autres par une teinte plus soutenue.

**% d'affectation**, dont l'infobulle dit « Afficher le pourcentage d'affectation » : fait apparaître le taux chiffré dans les cases, en plus de leur couleur. Il est désactivé à l'ouverture.

## Le plan de charge

Le plan se lit comme un tableau à double entrée.

* en ligne, un collaborateur, présenté par son **Nom** et son **Rôle** ;
* en colonne, un jour. Les colonnes sont regroupées par mois, dont le nom est rappelé en tête, et le jour de la semaine est indiqué au-dessus du quantième. Le mois que vous avez choisi occupe le centre du bandeau ; le mois précédent et le mois suivant l'encadrent, en grisé. Deux flèches, de part et d'autre de ce bandeau, vous déplacent vers la période précédente et vers la période suivante.

Chaque case porte une couleur qui traduit la charge du collaborateur ce jour-là. Si aucun collaborateur ne répond aux critères retenus, le logiciel affiche à la place « Aucun collaborateur à afficher ».

## Ce que mesure le taux d'affectation

Le taux rapporte le temps déjà occupé du collaborateur au temps de travail attendu de lui.

* le temps occupé est la durée cumulée de ce qui est positionné à son planning ce jour-là ; en mode **Jour**, les absences du collaborateur ce jour-là s'y ajoutent ;
* le temps attendu vient de son annualisation lorsqu'il en a une, et de ses plages horaires hebdomadaires sinon. C'est pourquoi le plan de charge dépend directement de ce qui est renseigné sur la fiche du collaborateur.

Un collaborateur dont le jour considéré ne porte ni plage horaire ni période d'annualisation n'a pas de temps attendu : aucun taux ne peut alors être calculé pour lui.

## La légende

Sous le plan, une légende donne le sens des couleurs. Elle comporte cinq états, présentés dans cet ordre :

* **< 50 %** : en vert, le collaborateur est occupé à moins de la moitié de son temps ;
* **< 100 %** : en jaune, il est occupé, sans être saturé ;
* **≥ 100 %** : en rouge, il est à saturation, ou au-delà ;
* **Aucune affectation** : en blanc, aucune tâche ne lui est affectée sur la période ;
* **Plages horaires non définies** : en gris, son temps de travail attendu n'est pas connu du logiciel.

Ne confondez pas les deux derniers états. « Aucune affectation » vous dit que le collaborateur est disponible ; « Plages horaires non définies » vous dit seulement que sa charge n'est pas mesurable, faute de temps attendu. Aucun taux n'est alors calculé, et la case reste sans pourcentage même si vous avez demandé l'affichage des pourcentages.

## Le détail d'une case

Une case portant une affectation est cliquable : le logiciel ouvre alors la fenêtre « Tâches collaborateur », qui présente les tâches de ce collaborateur sur la période de la case. Les cases sans affectation et celles dont le temps attendu n'est pas connu ne réagissent pas au clic.
