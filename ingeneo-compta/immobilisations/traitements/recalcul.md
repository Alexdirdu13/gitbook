# Recalcul

{% hint style="info" %}
**Où le trouver :** Menu **Traitements › Recalcul**
{% endhint %}

{% hint style="success" %}
**En bref** — Cet écran recalcule en une fois, à une même date, les valeurs calculées de toutes les fiches du dossier annuel : dotation de l'exercice, cumul des dotations et valeur nette comptable.

* Pour recalculer toutes les fiches : vérifiez la « Date de recalcul », puis bouton \[Valider] ; le traitement part sans demander de confirmation.
* Laisser la fenêtre de progression travailler jusqu'au bout : son bouton de fermeture ne devient actif qu'à la fin du traitement.
{% endhint %}

Chaque fiche immobilisation mémorise, dans sa rubrique « Valeurs calculées », une date de calcul et les valeurs arrêtées à cette date : la dotation de l'exercice, le cumul des dotations et la valeur nette comptable. Le recalcul met ces valeurs à jour.

<figure><img src="../../.gitbook/assets/15-cm903.jpg" alt="Écran Recalcul"><figcaption><p>Écran « Recalcul » de la nouvelle interface</p></figcaption></figure>

Vous n'avez pas à y penser au quotidien : le logiciel recalcule une fiche à chaque fois que vous l'enregistrez, et vous pouvez aussi la recalculer seule, à une date de votre choix, depuis la fiche elle-même. Cette option-ci fait la même chose **pour toutes les fiches du dossier annuel, à une seule et même date**.

## Rubrique « Recalcul »

L'écran ne comporte qu'un seul champ.

**Date de recalcul** : la date à laquelle vous voulez arrêter les valeurs. Son infobulle le rappelle : « Indiquez la date pour laquelle vous voulez lancer le recalcul de toutes les fiches immobilisations. »

Le logiciel propose par défaut la **date de fin de l'exercice** du dossier annuel sélectionné, qui est le cas le plus courant. Vous pouvez saisir n'importe quelle autre date : contrairement à l'option « Intégration des écritures », le calendrier n'est ici borné ni au début ni à la fin de l'exercice. Renseignez-la toujours : sans date, le recalcul ne peut pas se lancer.

## Bouton \[Valider]

Il n'apparaît que si votre profil vous autorise le recalcul.

**Il lance immédiatement le traitement sur toutes les fiches du dossier annuel, sans vous demander confirmation et sans avertissement préalable.** Il n'y a ni sélection de périmètre, ni aperçu : vérifiez donc votre date avant de cliquer.

Le logiciel ouvre alors une fenêtre de progression qui affiche le code et le libellé de la fiche en cours de traitement, l'avancement en pourcentage et en nombre de fiches traitées sur le total, une barre de progression et une estimation du temps restant. Cette fenêtre n'a pas de croix de fermeture, et son bouton de fermeture ne devient actif qu'une fois le traitement achevé. Laissez-la travailler.

À la fin, le logiciel vous annonce que le recalcul est terminé et vous indique le **nombre d'immobilisations recalculées**, ainsi que la durée de l'opération lorsqu'elle atteint cinquante secondes.

## Ce que le recalcul fait, et ce qu'il ne fait pas

Le recalcul ne touche qu'aux **valeurs calculées** de vos fiches : date de calcul, taux, dotation de l'exercice, cumul des dotations, cumul antérieur et valeur nette comptable — et, lorsque l'amortissement fiscal est activé sur la fiche, la dotation et le cumul fiscaux, l'amortissement dérogatoire et son cumul, ainsi que la réintégration ou la déduction et son cumul.

Il ne modifie aucune donnée que vous avez saisie, ne crée aucune écriture et ne supprime rien. Vous pouvez le relancer autant de fois que nécessaire : chaque exécution remplace simplement les valeurs mémorisées par celles de la nouvelle date.

Il inscrit en revanche, sur chaque fiche recalculée, la date du calcul et le **nom de l'utilisateur qui a lancé le traitement**. Comme ce traitement porte sur l'ensemble du dossier annuel, c'est donc votre nom qui figurera sur toutes les fiches recalculées, à la place de celui du collaborateur qui les avait calculées avant vous.

Le nombre annoncé en fin de traitement peut être **inférieur** au nombre de fiches de votre dossier : une fiche dont le paramétrage d'amortissement est incomplet — durée totale ou date de début d'amortissement manquante — est passée sans être recalculée. C'est le même critère qui écarte une fiche de la génération des écritures ; si l'écart vous surprend, c'est de ce côté qu'il faut chercher.
