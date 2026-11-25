# Comment indiquer un prélèvement en échec ?

## Contexte

Lorsque vous envoyez un fichier XML de prélèvement SEPA à votre banque, il est possible que certains paiements soient rejetés. Ces rejets peuvent être liés à des problèmes tels qu’un IBAN incorrect, un compte clôturé ou des fonds insuffisants.

La banque vous transmet alors une **liste de rejets**. Pour garder votre système à jour et refléter fidèlement la situation, il est nécessaire d’annuler manuellement les paiements concernés dans votre application Qotid.

## Se rendre dans l'onglet Paiement de la facture identifiée et annuler le prélèvement

À partir de la liste de rejets transmise par votre banque, identifiez la facture concernée dans votre application Qotid. Une fois sur la facture, accédez à l’onglet **Paiement**, puis cliquez sur la **croix** située à droite du paiement rejeté afin de l’annuler.

Suite à ce clic et une demande de confirmation, **le paiement passe au statut "Rejeté"**.

## La facture repassera automatiquement au statut "À payer"

Une fois le paiement annulé, la facture repasse automatiquement au statut **"À payer"**, ce qui vous permet de la régulariser ultérieurement.
