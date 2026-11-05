# Présentation et prise en main

{% hint style="success" %}
**En bref** — Le module Gestion interne vous permet de piloter les missions du cabinet et d'organiser le travail de vos collaborateurs : missions, planning, suivi et génération des factures.

* Pour mettre en place le module : renseignez les données de base dans le panneau « Paramètres », dans l'ordre indiqué (postes, collaborateurs, groupes de travail, tâches, modèles de mission).
* Pour démarrer : créez vos missions dans le menu « Missions », option « Missions en cours », puis placez leurs tâches dans le menu « Planning ».
{% endhint %}

## Ouvrir le module

Le module s'ouvre par l'entrée « Gestion interne » de la barre latérale, à gauche de l'écran, dans le groupe « Gestion cabinet », que l'on déplie d'un clic car il est replié à la connexion. Le logiciel vous place alors sur le menu « Missions », option « Missions en cours ».

Le menu du module, en haut de l'écran, propose les options suivantes :

* « Missions » : « Missions en cours » et « Missions archivées »,
* « Planning »,
* « Traitements » : « Génération des factures » et « Réaffectation de tâches »,
* « Editions » : « Suivi des missions », « Suivi des tâches » et « Plan de charge »,
* « Signatures ».

Les données de base du module ne figurent pas dans ce menu : elles se trouvent dans le panneau « Paramètres », présenté à l'étape 1 ci-dessous.

La mise en place du module suit les étapes ci-dessous. Chaque option est décrite dans la page qui lui correspond.

## Le paramétrage des données de base

Les données de base se saisissent dans le panneau « Paramètres », que vous ouvrez par l'entrée « Paramètres » de la barre latérale (affichée en permanence sur le tableau de bord ; sur les autres écrans, elle est masquée et s'ouvre d'un clic sur le bord gauche de l'écran). Celles du module y sont réparties entre la rubrique « Données », groupe « Organisation et temps » (postes, annualisations, groupes de travail, familles de tâches, tâches, types d'absences) et groupe « Tiers et commercial » (collaborateurs, clients), et la rubrique « Modèles » (modèles de mission, de lettre de mission et de page). Elles s'appuient les unes sur les autres — une tâche se range dans une famille, un groupe de travail se compose de collaborateurs et de leurs postes, un modèle de mission reprend des tâches et des postes — : renseignez-les de préférence dans l'ordre ci-dessous.

* « Postes (GI) » : les rôles que vos collaborateurs peuvent tenir. Un poste peut être déclaré tête de groupe.
* « Collaborateurs » : vos collaborateurs sont les utilisateurs du logiciel. Ce fichier ne les crée pas — il ne porte pas de bouton **\[Nouveau]** — et leur identité ne s'y modifie pas. Vous y complétez ce que la gestion interne demande : les postes auxquels chacun a accès, ses valorisations (salaire brut annuel, coût horaire salarial, prix de vente horaire…), sa charge de travail et les délégataires autorisés à tenir son planning.
* « Annualisations » : si le temps de travail d'un collaborateur n'est pas le même toute l'année, vous en décrivez ici la répartition, puis vous l'affectez au collaborateur depuis la rubrique « Charge de travail » de sa fiche.
* « Groupes de travail (GI) » : les équipes auxquelles vous rattachez vos missions. Un groupe se compose de collaborateurs, chacun avec son poste, et il doit avoir une tête de groupe, et une seule.
* « Familles de tâches » : elles regroupent par thème les tâches effectuées par vos collaborateurs.
* « Tâches (GI) » : chaque tâche appartient à une famille et se déclare tâche cabinet ou tâche client. Vous y fixez sa durée par défaut, sa périodicité et, si elle est facturable, son mode de facturation : au forfait, par quantité ou au temps effectif.
* « Missions », dans le groupe « Divers » de la rubrique « Modèles » (l'écran s'intitule « Modèles de mission ») : un modèle décrit une mission type — les tâches qu'elle comprend, le poste qui doit tenir chacune d'elles, et les modes de facturation qu'elle autorise.
* « Lettres de mission » et « Pages de document », dans le groupe « Documents » de la rubrique « Modèles » : les modèles qui servent à produire vos lettres de mission, et les en-têtes, pages de garde et pieds de page sur lesquels elles s'appuient. Le modèle de lettre de mission n'étant pas obligatoire sur un modèle de mission, vous pouvez les paramétrer dans un second temps.
* « Types d'absences » : les motifs d'absence de vos collaborateurs. Ce fichier est commun au module des feuilles de temps.
* « Clients » : ce fichier est partagé avec les autres modules ; il est donc possible que vos clients y soient déjà enregistrés.

## La création des missions

Menu « Missions », option « Missions en cours ». Une mission décrit, pour un client, le travail convenu avec lui. Elle se bâtit à partir d'un modèle de mission : dans la liste des missions, ce modèle apparaît dans la colonne « Type de mission ». Vous la rattachez ensuite à un groupe de travail.

Une mission clôturée quitte cette liste pour l'option « Missions archivées ». Les lettres de mission que vous adressez en signature électronique se suivent dans le menu « Signatures ».

## L'établissement du planning

Menu « Planning ». Vous y placez dans l'agenda d'un collaborateur les tâches qui lui sont confiées. Pour utiliser le planning, vous devez être vous-même inscrit comme collaborateur. La fiche d'un collaborateur désigne jusqu'à trois délégataires, autorisés à accéder à son planning et à le modifier.

En cas d'absence d'un collaborateur, le menu « Traitements », option « Réaffectation de tâches », vous permet de confier un ensemble de ses tâches à un autre collaborateur.

## La mise à jour des feuilles de temps depuis le planning

Dans le planning, le bouton **\[Transfert en feuilles de temps]** reporte dans la feuille de temps les tâches planifiées que vous avez sélectionnées dans l'agenda.

Ce transfert compte aussi pour la facturation : pour une tâche facturée au temps effectif, seul le temps transféré en feuilles de temps est facturé.

## Le suivi des missions

Le menu « Editions » vous propose deux éditions, « Suivi des missions » et « Suivi des tâches », qui rendent compte de l'avancement de vos missions et de leurs tâches. Il propose aussi le « Plan de charge », qui n'est pas une édition : il affiche directement à l'écran le taux d'occupation de chaque collaborateur, jour par jour.

## La génération des factures

Menu « Traitements », option « Génération des factures ». Elle se fait à la demande : vous indiquez une période, le logiciel vous présente les échéances de vos missions qui y tombent, puis vous générez les factures de celles que vous retenez. Les factures sont créées dans le module de facturation.

Leur montant vient des informations de facturation portées par les missions et par les fiches des collaborateurs : pour une tâche facturée au temps effectif, le temps transféré en feuilles de temps est valorisé au prix de vente du collaborateur.
