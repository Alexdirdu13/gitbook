# À quoi sert l'adressage dans le cadre de la facturation électronique ?

## L'utilité de l'adressage dans le cadre de la facturation électronique

L'adressage, dans le contexte de la facturation électronique (notamment la réforme française du e-invoicing entre entreprises), c'est le mécanisme qui permet de savoir **à qui envoyer une facture électronique et par quel canal**, de façon fiable et automatisée.

Concrètement, il répond à trois besoins :

**1. Identifier le bon destinataire**

Une facture doit arriver à l'entité juridique exacte qui doit la recevoir (et pas une entité proche, une filiale différente, etc.). L'adressage s'appuie sur des identifiants normalisés :

* SIREN
* SIREN + SIRET en France
* SIREN + SUFFIXE en France

**2. Trouver la "route" technique**

Chaque entreprise choisit sa propre plateforme pour émettre et recevoir ses factures (ce qu'on appelle une PA, Plateforme Agréée). L'émetteur ne sait pas forcément quelle plateforme utilise son client. Un **annuaire central** (tenu par l'administration fiscale, via le futur PPF, Portail Public de Facturation) répertorie qui utilise quelle plateforme en fonction de son adressage.

**À savoir :** en effet, une entreprise peut utiliser plusieurs PA. Pour l'adressage SIREN + SUFFIXE, par exemple 123456789\_FRAISGENERAUX, l'entreprise utilise la PA en réception 1 et, pour l'adressage 123456789\_ACHATSTRATEGIQUE, l'entreprise utilise la PA en réception 2.

L'adressage consiste à acheminer la facture vers la bonne adresse et à identifier au passage la plateforme qui recevra la facture.

Si votre fournisseur n'enregistre pas d'adressage par défaut, il risque d'envoyer la facture sur votre identifiant d'adressage SIREN et donc de l'envoyer au mauvais endroit.

**3. Acheminer la facture sans intervention humaine**

Une fois la bonne plateforme identifiée, l'adressage permet le routage automatique du document (souvent au format structuré comme Factur-X, UBL ou CII) de la plateforme de l'émetteur vers celle du destinataire, sans que l'un ou l'autre ait à ressaisir ou renvoyer manuellement l'information.

**Pourquoi c'est important**

Sans adressage fiable :

* des factures pourraient être perdues ou envoyées au mauvais interlocuteur ;
* l'automatisation complète du cycle de la facture (obligation centrale de la réforme) serait impossible ;
* l'administration fiscale perdrait la capacité de collecter les données de facturation (e-reporting) de façon cohérente.

L'adressage est donc un peu l'équivalent d'un "système postal" numérique et normalisé pour les factures, indispensable pour que la dématérialisation fonctionne.
