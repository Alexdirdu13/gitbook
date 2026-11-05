# Comptes

{% hint style="info" %}
**Où le trouver :** Panneau **Paramètres** › **Immobilisations** › **Comptes**
{% endhint %}

{% hint style="success" %}
**En bref** — Cet écran paramètre les racines et numéros de comptes nécessaires aux écritures du module : classement des immobilisations, amortissements, sorties, subventions, emprunts, crédits-bails et contrats de location.

* Pour partir du paramétrage prévu par le logiciel : bouton \[Charger les valeurs par défaut], contrôlez les numéros en gris et en italique, puis bouton \[Enregistrer].
* Renseigner les cinq racines obligatoires de la rubrique « Classement des immobilisations », plusieurs racines se séparant par un point-virgule (par exemple 21;24).
* Pour créer un compte manquant : bouton \[+] à droite de la zone, ou pictogramme « Loupe » pour le rechercher dans le plan comptable.
{% endhint %}

Cette option permet de paramétrer toutes les racines et tous les numéros de comptes nécessaires à la génération des écritures comptables issues du module. Vous arrivez directement sur le formulaire, organisé en huit rubriques ; il n'y a pas de liste.

<figure><img src="../../.gitbook/assets/15-cm219.jpg" alt="Écran Comptes"><figcaption><p>Écran « Comptes » de la nouvelle interface</p></figcaption></figure>

Les cinq racines de la première rubrique sont les seuls champs obligatoires de l'écran : ce sont elles qui permettent au logiciel de reconnaître la catégorie d'une immobilisation d'après son numéro de compte. Les cinquante-huit autres champs sont facultatifs, et un champ laissé vide signifie simplement que le logiciel ne proposera rien à sa place.

## Les trois formes de saisie de l'écran

Il n'y en a que trois, et les reconnaître vous fait lire l'écran d'un coup d'oeil.

Une **racine** se saisit dans une zone courte, seule sur sa ligne. Une racine n'est faite que de chiffres, et vous pouvez en indiquer plusieurs en les séparant par un point-virgule, par exemple 21;24. Un point-virgule ne peut être ni au début, ni à la fin, ni doublé. Une même racine ne peut pas être employée pour deux paramétrages différents.

Un **compte** se saisit dans une zone suivie de trois éléments : le bouton \[+] crée le compte dans le plan comptable, le pictogramme « Loupe » ouvre la recherche dans le plan comptable — accessible aussi par les touches Ctrl + Alt + L —, et la zone « Intitulé compte », qui n'est pas saisissable, affiche l'intitulé du compte dès qu'il est reconnu. Un compte que le logiciel ne trouve pas dans le plan comptable est refusé à l'enregistrement, et si une racine est paramétrée pour ce même usage, le numéro saisi doit commencer par cette racine.

Une **liste**, enfin, pour les deux journaux de l'écran, avec à sa droite le libellé du journal choisi.

Un numéro affiché en gris et en italique n'est pas une valeur enregistrée : c'est une valeur que le logiciel vous propose et qui n'existe pas dans votre plan comptable, comme l'explique le paragraphe k).

## Rubrique « Classement des immobilisations »

Elle s'ouvre sur la phrase « Indiquez les racines de compte de chaque catégorie d'immobilisations : », et c'est bien de cela qu'il s'agit : chaque catégorie du bilan reçoit sa ou ses racines, et le logiciel en déduit la catégorie de chacune de vos immobilisations.

**Immobilisations incorporelles** \*

**Immobilisations corporelles** \*

**Immobilisations financières** \*

**Immobilisations mises en concessions** \*

**Immobilisations en cours** \*

Ces cinq racines sont obligatoires.

## Rubrique « Racines et numéros de comptes par défaut »

Elle s'ouvre sur la phrase « Pour éviter les erreurs d'affectation de numéros de compte, vous pouvez indiquer les racines de comptes ou les comptes à utiliser dans les fiches immobilisations : » et se lit en trois temps, annoncés par trois sous-titres.

Sous **« Acquisitions »** :

| Champ                                      | Ce qu'il faut savoir                                                                                      |
| ------------------------------------------ | --------------------------------------------------------------------------------------------------------- |
| **Journal d'achat**                        | La liste propose les journaux de type Achat du dossier ; elle est vide si le dossier n'en comporte aucun. |
| **Compte de TVA pour les immobilisations** | Le compte de TVA déductible sur immobilisations.                                                          |

Sous **« Amortissement économique »** :

**Racine des comptes d'amortissement**

**Racine des comptes de dotation pour les immobilisations incorporelles**

**Compte de dotation par défaut pour les immobilisations incorporelles**

**Racine des comptes de dotation pour les immobilisations corporelles**

**Compte de dotation par défaut pour les immobilisations corporelles**

**Compte de quote-part personnelle**

Sous **« Amortissement fiscal »**, trois couples racine et compte :

**Racine des comptes d'amortissement dérogatoire**

**Compte d'amortissement dérogatoire par défaut**

**Racine des comptes de reprise sur dérogatoire**

**Compte de reprise sur dérogatoire par défaut**

**Racine des comptes de provision dérogatoire**

**Compte de provision dérogatoire par défaut**

## Rubrique « Traitements sur immobilisations »

Elle réunit les comptes des trois traitements que vous pouvez conduire sur une immobilisation déjà enregistrée, chacun sous son sous-titre.

Sous **« Amortissement exceptionnel »** :

**Dotations exceptionnelles**

**Reprises de dotations exceptionnelles**

Sous **« Dépréciation »**, trois racines, sans compte par défaut :

**Racines des comptes de dotation aux dépréciations**

**Racines des comptes de dépréciations**

**Racines des comptes de reprise de dépréciations**

Sous **« Sortie d'immobilisation »**, la racine commune aux produits de cession, puis le compte de produit propre à chaque catégorie d'immobilisation, puis les trois comptes de la contrepartie :

**Racine de compte de produits de cessions**

**Compte de produit de cession d'immo incorporelles**

**Compte de produit de cession d'immo corporelles**

**Compte de produit de cession d'immo financières**

**Compte de TVA sur cession**

**Compte de valeur nette comptable (sortie)**

**Compte de TVA à reverser (sortie)**

## Rubrique « Subventions d'investissements »

Trois couples racine et compte par défaut.

**Racine des comptes de subventions d'investissements**

**Compte de subventions d'investissements par défaut**

**Racine des comptes de subventions d'investissements inscrites au compte de résultat**

**Compte de subventions d'investissements inscrites au compte de résultat par défaut**

**Racine des comptes de quotes-parts de subventions virées au compte de résultat**

**Compte de quotes-parts de subventions virées au compte de résultat par défaut**

## Rubrique « Autres paramètres »

| Champ                                   | Ce qu'il faut savoir                                                                                                                            |
| --------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------------------- |
| **Report à nouveau**                    | Le compte de report à nouveau.                                                                                                                  |
| **Journal d'intégration des écritures** | Le journal dans lequel le logiciel passe les écritures produites par le module. La liste propose les journaux d'opérations diverses du dossier. |

## Rubrique « Emprunts »

Les comptes des écritures d'emprunt.

**Racine des comptes d'emprunt**

**Racine des comptes banque**

**Compte banque par défaut**

**Racine des comptes de charge des intérêts**

**Compte de charge des intérêts**

**Racine des comptes d'assurance**

**Compte d'assurance**

**Racine des comptes de frais de dossier**

**Compte des frais de dossier**

**Compte de TVA**

## Rubrique « Crédits-bails »

Les comptes des écritures de crédit-bail : les loyers, selon que le bien est mobilier ou immobilier, puis les charges annexes.

**Racine des loyers mobiliers**

**Racine des loyers immobiliers**

**Racine des comptes d'assurance**

**Compte d'assurance**

**Racine des comptes de frais de dossier**

**Compte des frais de dossier**

**Compte de TVA**

## Rubrique « Contrats de location »

Elle demande exactement les mêmes sept informations que la rubrique « Crédits-bails », dans le même ordre — mais pour les contrats de location, dont les loyers ne se comptabilisent pas dans les mêmes comptes.

Prenez garde, en saisissant, à la rubrique dans laquelle vous vous trouvez : trois rubriques de cet écran demandent un « Compte d'assurance » et un « Compte de TVA », et rien ne les distingue que la rubrique qui les contient.

## Bouton \[Enregistrer]

Il enregistre l'ensemble du paramétrage et affiche « Les modifications ont bien été enregistrées. ».

Si une des cinq racines obligatoires est vide, si un numéro de compte n'existe pas dans le plan comptable, s'il ne correspond pas à la racine paramétrée, si une racine contient autre chose que des chiffres et des points-virgules, ou si la même racine est employée deux fois, l'enregistrement est refusé et le message s'affiche sous le champ concerné.

## Bouton \[Charger les valeurs par défaut]

Il remplit le formulaire avec le paramétrage prévu par le logiciel. Son pictogramme d'information le précise : « Ce bouton charge les valeurs prévues et vérifie que les comptes existent bien dans le plan comptable. Si ce n'est pas le cas, le numéro de compte sera affiché en gris et en italique. »

Le logiciel affiche alors le message « Les valeurs par défaut ont été chargées. Si des numéros de comptes n'ont pas été renseignés c'est qu'ils n'existent pas dans votre plan comptable. Cliquez sur le bouton \[Enregistrer] pour mémoriser votre nouveau paramétrage. »

Retenez-en deux choses. D'abord, ce bouton ne fait que remplir le formulaire : rien n'est enregistré tant que vous n'avez pas utilisé le bouton \[Enregistrer], et il écrase ce que vous aviez saisi. Ensuite, un numéro en gris et en italique n'est pas paramétré : créez le compte manquant dans votre plan comptable, ou saisissez à sa place le compte que vous employez.

Selon les droits qui vous sont accordés, l'enregistrement peut ne pas vous être autorisé.
