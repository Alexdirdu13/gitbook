# Comment paramétrer mon circuit de validation des factures fournisseurs ?

## Se rendre sur la vue des workflows

Pour paramétrer vos statuts, rendez-vous d'abord dans le menu déroulant "**Achats**", puis cliquez sur "**Étapes de validation**".

Vous aurez par défaut les trois étapes suivantes :

* Enregistrement
* En attente
* Validé

**Chemin : Créer un nouveau statut**

## Créer un nouveau statut

Pour créer un nouveau statut, il vous suffit de cliquer sur le bouton "**Ajouter**".

## Informations

Une fenêtre apparaîtra. Vous pourrez donner le nom que vous souhaitez au statut, choisir sa couleur et renseigner le reste des champs selon vos souhaits.

## Autorisations

Continuez de faire défiler la fenêtre pour arriver aux autorisations. Ici, vous aurez la possibilité de gérer l'accès aux statuts, les autorisations de validation et de modification des documents, ainsi que leur visibilité.

**À savoir :**

Vous avez aussi la possibilité d'ajouter des blocs de conditions en cliquant sur les cases portant le même nom.

## Exemple 1

Par exemple, si vous souhaitez restreindre la validation du document au profil Manager, vous pouvez renseigner les éléments suivants :

* Profil : cochez Admin et Manager **(NB : pensez à bien cocher le profil Admin à chaque fois que vous ajoutez une restriction ; en effet, ce profil ne doit pas avoir de restriction)**

Vous pouvez également appliquer cette restriction à des utilisateurs plutôt qu'à des profils.

## Exemple 2

Vous pouvez également ajouter des conditions si vous ne souhaitez pas que ces restrictions s'appliquent à l'ensemble de vos factures.

Par exemple, vous souhaitez restreindre au profil Manager la validation des factures supérieures à 500 €.

Vous pouvez cliquer sur "Ajouter un bloc de condition" et renseigner les champs suivants :

* Source : Montant HT
* Comparaison : Supérieur à
* Montant : 500
* Liste des utilisateurs : cocher Admin et Manager

## Prochaine étape

En continuant de faire défiler la fenêtre, vous pourrez choisir la prochaine étape du statut parmi celles déjà existantes.

**À savoir :**

Il vous est aussi possible de créer une condition en cliquant sur "**Ajouter un bloc de condition**".

Pour finaliser la création du nouveau statut, cliquez sur le bouton "**Valider**".

**Chemin : Modifier un statut**

## Modifier un statut

Pour modifier un statut, cliquez sur le pinceau pour accéder à l'éditeur.

**Chemin : Supprimer un statut**

## Supprimer un statut

Pour supprimer un statut, il vous suffit de cliquer sur la corbeille et de valider votre choix de supprimer cette étape.
