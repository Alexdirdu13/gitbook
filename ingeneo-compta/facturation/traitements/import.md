# Import

{% hint style="info" %}
**Où le trouver :** Menu **Traitements › Import**
{% endhint %}

{% hint style="success" %}
**En bref** — Cet écran reprend vos clients, articles et factures provenant d'un autre outil, à partir d'un classeur Excel fourni que vous remplissez.

* Pour préparer l'import : bouton \[Télécharger la trame d'import], puis remplissez le classeur.
* Pour importer : choisissez le classeur rempli, puis bouton \[Importer] et lisez le rapport d'import.
{% endhint %}

Cette option vous permet de reprendre dans le logiciel des données provenant d'un autre outil : vos clients, vos articles et vos factures. Comme les logiciels de facturation n'emploient pas tous les mêmes formats — contrairement à la comptabilité, où les écritures sont beaucoup plus normées —, le logiciel vous fournit une trame d'import sous la forme d'un classeur Excel que vous remplissez avec vos données.

<figure><img src="../../.gitbook/assets/25-cm832.jpg" alt="Écran Import"><figcaption><p>Écran « Import » de la nouvelle interface</p></figcaption></figure>

L'écran vous rappelle la marche à suivre en quatre temps : téléchargez le classeur contenant les trames d'import et la notice explicative, remplissez-le avec vos données, réalisez l'import, puis lisez le rapport. L'écran annonce que le logiciel éditera un rapport d'import indiquant le nombre d'enregistrements importés pour chaque fichier et, s'il détecte des erreurs, l'onglet concerné, la ligne où se trouve l'erreur et sa nature.

Le pictogramme d'information placé au bout de la première ligne porte une infobulle qui énumère les fichiers que cette option sait importer. Ils sont **sept** depuis la Facturation : les clients, les adresses des clients, les banques des clients, les articles, les prix de catalogues des articles, les comptes comptables des articles, et les factures clients. Aucun fichier de fournisseurs n'y figure : la même option, ouverte depuis la Gestion commerciale, en propose davantage.

bouton **\[Télécharger la trame d'import]**

Vous remet le classeur Excel à remplir. Outre les trames elles-mêmes, il contient une notice décrivant, fichier par fichier, les caractéristiques attendues de chaque champ : caractère obligatoire ou facultatif, longueur, valeurs admises. Reportez-vous y avant de saisir : c'est là que se trouvent les règles que le logiciel contrôlera à l'import.

Une précaution à prendre avec votre tableur, et elle est la cause d'imports rejetés sans raison apparente : certains champs qui ne contiennent que des chiffres — un numéro de compte, un code postal — peuvent être interprétés comme des nombres au moment où vous les recopiez dans la trame, et leurs « 0 » de tête disparaissent alors. Un code postal 06000 devient 6, un compte auxiliaire 0105000 devient 105. Assurez-vous que le logiciel avec lequel vous ouvrez la trame n'a pas modifié la nature de ces colonnes.
