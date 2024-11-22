
On peut utiliser un ControllerAdvice pour gérer automatiquement les exceptions dans un HandlerGlobal.

Il suffit de définir derrière des méthodes annotées par @ExceptionHandler(MonException.class) pour que celles-ci soient automatiquement gérées lorsqu'elles remontent la pile.

Bien sur il faut retourner des response entity pour forcer a créer une enveloppe HTML contenant le message d'erreur a indiquer ainsi que le code erreur.

Il est possible d'annoter des exceptions customisées par @ResponseStatus pour préciser un statut par défaut.