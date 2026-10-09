# Diagnostic

Une section par test en échec : renseignez ses quatre champs.

## testAddingALineToAnUnknownOrderIsNotFound

**Symptôme** :

**Cause** :

**Règle du module en jeu** :

**Correctif** :

## testAddingALineToAPaidOrderIsAConflict

**Symptôme** :

**Cause** :

**Règle du module en jeu** :

**Correctif** :

## testAddingALineToMyOrder

**Symptôme** :

**Cause** :

**Règle du module en jeu** :

**Correctif** :

## testAddingALineWithAZeroQuantityIsUnprocessable

**Symptôme** :

**Cause** :

**Règle du module en jeu** :

**Correctif** :

## testListingKitchenTicketsReturnsMine

**Symptôme** :

**Cause** :

**Règle du module en jeu** :

**Correctif** :

## testListingKitchenTicketsWithoutTokenIsUnauthorized

**Symptôme** :

**Cause** :

**Règle du module en jeu** :

**Correctif** :

## testOpeningAnOrderIgnoresAnAbandonedOne

**Symptôme** : les lignes de la commande ouverte par Bob : JSON reçu différent de l'attendu

**Cause** : la ligne 23 dans le fichier SoftDeleteFilter.php:23 return sprintf('%s.deleted_by_id IS NULL', $targetTableAlias);

**Règle du module en jeu** : 

**Correctif** : Il faut modifier deleted_by_id IS NULL en deleted_at IS NULL

## testPayingMyOrderMarksItPaid

**Symptôme** :

**Cause** :

**Règle du module en jeu** :

**Correctif** :

## testRefreshingTwiceWithTheSameTokenIsUnauthorized

**Symptôme** : Statut 401 attendu, 2OO reçu

**Cause** : ça échouait parce que le jeton de renouvellement n'était pas à usage unique

**Règle du module en jeu** : La sécurité de l'auth

**Correctif** : aller dans gesdinet_jwt_refresh_token.yaml et passer single_use: false en true

## testRemovingALineFromSomeoneElsesOrderIsForbidden

**Symptôme** :

**Cause** :

**Règle du module en jeu** :

**Correctif** :
