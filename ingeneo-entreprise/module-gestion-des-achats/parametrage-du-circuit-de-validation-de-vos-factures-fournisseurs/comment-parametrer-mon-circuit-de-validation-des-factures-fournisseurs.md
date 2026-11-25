# Comment paramétrer mon circuit de validation des factures fournisseurs?

## Se rendre sur la vue des workflows

Pour paramétrer vos statuts, il vous faut dans un premier temps vous rendre dans le menu défilant "**Achats**" puis de cliquer sur "**Etapes de validation**".

Vous aurez par défaut les trois étapes suivantes :

* Enregistrement
* En attente
* Validé

**Chemin : Créer un nouveau statut**

## Créer un nouveau statut

Pour créer un nouveau statut, il vous suffit de cliquer sur le bouton "**Ajouter**".

## Informations

Une fenêtre apparaîtra. Vous pourrez créer le nom que vous souhaitez donner au statut, sa couleur ainsi que le reste des champs que vous voyez à remplir selon vos souhaits.

## Autorisations

Continuez de défiler la fenêtre pour arriver aux autorisations. Ici, vous aurez la possibilité de gérer l'accès aux statuts, aux autorisations de validation et de modification des documents ainsi que de leur visibilité.

**À savoir :**

Vous avez aussi la possibilité d'ajouter des blocs de conditions en cliquant sur les cases portant le même nom.

## Exemple 1

Par exemple, si vous souhaitez restreindre la validation du document au profil Manager, vous pouvez renseignez les éléments suivants :

* Profil : cochez Admin et Manager **(NB : pensez à bien cocher le profil Admin à chaque fois que vous ajoutez une restriction, en effet ce profil ne doit pas avoir de restriction)**

Vous pouvez également appliquer cette restriction sur des utilisateurs plutôt que des profils.

## Exemple 2

Vous pouvez également ajouter des conditions si vous ne souhaitez pas que ces restrictions s'applique à l'ensemble de vos factures.

Par exemple vous souhaitez restreindre la validation des factures supérieures à 500€ au profil manager.

Vous pouvez cliquer sur "ajouter un bloc de condition" et renseigner les champs suivants :

* Source : Montant HT
* Comparaison : Supérieur à
* Montant : 500
* Liste des utilisateurs : cocher Admin et Manager

## Prochaine étape

En continuant de défiler, vous pourrez choisir la prochaine étape du statut parmi ceux déjà existants.

**À savoir :**

Il vous est aussi possible de créer une condition en cliquant sur "**Ajouter un bloc de condition**".

Pour finaliser la création du nouveau statut, cliquez sur le bouton "**Valider**".

**Chemin : Modifier un statut**

## Modifier un statut

Pour modifier un statut, il vous faut cliquer sur le pinceau pour pouvoir accéder à l'éditeur.

**Chemin : Supprimer un statut**

## Supprimer un statut

Pour supprimer un statut, il vous suffit de cliquer sur la corbeille et de valider votre choix de supprimer cette étape.
