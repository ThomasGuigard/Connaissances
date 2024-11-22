Verbes HTTP
--------------------------

Il existe différents verbes HTTP que l'on peut utiliser lorsque l'on effectue une requête vers un serveur. Bien que l'on puisse utiliser n'importe quelle verbe pour n'importe quelle action ceux-ci sont régis par des conventions. Voici les différents verbes communément utilisés ainsi que leur but :
- GET : Pour récupérer une ressource
- POST : Pour créer une ressource
- PATCH : Pour mettre à jour une ressource
- PUT : Pour mettre à jour une ressource
- DELETE : Pour supprimer une ressource

Ceux-ci sont majoritairement utilisées au sein des API REST car ils permettent d'avoir des actions articulées autour de ressources.

Codes erreurs
--------------------------

- HTTP 200 : Concerne tout ce qui aux requêtes fructueuses. Quelques exemples :
	- 200 : OK
	- 201 : Created
- HTTP 3xx : Concerne tout ce qui touche aux redirections. Quelques exemples :
	- 301 : Moved Permanently
	- 302 : Found
	- 303 : See Other
- HTTP 4xx : Concerne toutes les erreurs utilisateurs, c'est à dire provenant de la personne qui effectue la requête. Quelques exemples :
	- 400 : Bad Request
	- 401 : Unauthorized
	- 403 : Forbidden
	- 404 : Not found
	- 405 : Method Not Allowed
- HTTP 5xx : Concerne toutes les erreurs côté serveur. Quelques exemples : 
	- 500 : Internal server error
	- 503 : Service unavailable