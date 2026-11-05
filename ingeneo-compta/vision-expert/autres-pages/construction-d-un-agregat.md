# Construction d'un agrégat

{% hint style="success" %}
**En bref** — Cette page explique comment écrire un agrégat de comptes : liste de comptes et racines, formule commençant par =, ou donnée externe.

* Pour additionner des comptes : séparez-les par un point-virgule, par exemple 500-505D;60C;700001.
* Pour écrire une formule : commencez par = et mettez chaque groupe entre crochets, par exemple =\[70701000]/\[#Nombre de véhicules#].
{% endhint %}

Dans plusieurs modules du logiciel vous êtes amené à indiquer des agrégats de comptes.

Ces agrégats peuvent se construire de deux manières : soit sous la forme d'une liste de comptes (ou racines de comptes), soit par l'utilisation de formules. Les indicateurs acceptent en outre un troisième mode d'écriture, décrit en fin de page.

## Fonctionnement par comptes et racines de comptes :

Il s'agit de saisir une suite de numéros de compte ou de fourchette de comptes dont les soldes seront additionnés.

Chaque compte ou fourchette de comptes doit être suivi d'un point-virgule pour le distinguer de la racine suivante ; écrivez les éléments à la suite, sans espace avant ni après le point-virgule.

Une fourchette s'écrit en séparant ses deux bornes par un tiret ; les deux bornes sont incluses.

Si vous souhaitez ne tenir compte que des débits ou des crédits, il suffit de faire suivre le numéro ou la racine par la lettre D ou C. Sans cette lettre, c'est le solde qui est retenu.

Pour ne retenir que certains comptes auxiliaires, indiquez-les entre parenthèses à la suite de la racine du compte général, une fourchette s'écrivant là aussi avec un tiret : 411(CLI1-CLI9) ne retient que les comptes auxiliaires de CLI1 à CLI9 du compte 411.

Pour limiter le calcul à certains journaux, indiquez leurs codes entre accolades devant la racine, séparés par une virgule : {VE,VT}706 ne retient les comptes 706 que dans les journaux VE et VT. Un code précédé d'un tiret est au contraire exclu : {-AN}706 retient les comptes 706 dans tous les journaux sauf AN. N'employez pas les deux formes dans la même liste de journaux : indiquez soit les journaux à retenir, soit ceux à écarter.

Les différents composants de la liste sont cumulés.

**Exemple 1** : 500-505D;60C;700001 = somme des débits des comptes commençant par 500, 501, 502, 503, 504 et 505 + somme des crédits des comptes commençant par 60 + solde des comptes commençant par 700001.

## Fonctionnement par formules :

Une formule commence par le caractère = (comme dans une formule Excel).

Chaque élément (ou groupe de sélection) composant la formule doit être mis entre crochet ; les éléments peuvent ensuite être assemblés par des opérateurs de calcul et des fonctions.

Entre les crochets, le fonctionnement est identique au fonctionnement par comptes et racines de comptes.

Les opérateurs utilisables sont : addition (+), soustraction (-), multiplication (\*) et division (/). Les parenthèses vous permettent d'ordonnancer les calculs.

**Exemple 2**

\=\[500-505D;60C;700001] est équivalent à l'exemple 1 ci-dessus.

{% hint style="warning" %}
Attention : chaque groupe de sélection de comptes (entre crochets) générera une requête vers la base de données à l'exécution ce qui, s'ils sont nombreux, peut diminuer les temps de réponse.
{% endhint %}

\=\[500-505D] + \[60C] + \[700001] aura le même résultat mais sera moins performant car trois requêtes seront exécutées au lieu d'une seule.

## Utilisation de données externes :

Si vous avez saisi des données externes depuis le module « Datas » ou le module « Supervision datas », vous pouvez les utiliser dans les formules des indicateurs pour, par exemple, générer un graphique sur l'évolution d'une donnée externe ou pour multiplier des valeurs issues de la comptabilité par une constante saisie dans les données externes.

Une donnée externe s'utilise de la manière suivante : \[#Libellé de la donnée#].

Le libellé de la donnée doit être celui que vous avez saisi dans le fichier des données externes, écrit en entier et avec ses espaces ; en revanche, les majuscules et les minuscules n'ont pas d'importance.

**Exemple 3**

\=\[70701000]/\[#Nombre de véhicules#] renverra le solde des comptes commençant par 70701000 divisé par la valeur de la donnée externe intitulée « Nombre de véhicules ».

Dans les indicateurs personnalisés, un troisième mode d'écriture est également accepté : si vous faites précéder votre saisie de deux signes égal, vous employez le langage de formules des états financiers (fonctions Solde, SoldeC, SoldeD, MvtC et MvtD).

Dans les indicateurs personnalisés et les alertes personnalisées, le logiciel ne contrôle pas la syntaxe de ce que vous saisissez : aucun message ne vous signale une liste de comptes ou une formule mal écrite. Après avoir enregistré, vérifiez donc le résultat obtenu.
