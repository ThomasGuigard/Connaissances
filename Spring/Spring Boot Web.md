
Comment récupérer des informations dans une requête
--------------------------

- @PathVariable : Permet de récupérer un parametre dans le chemin de l'url. Attention dans le @GetMapping il faut préciser entre accolades le nom du paramètre.
- @RequestParam : Permet de récupérer les query params dans une requête.
- @RequestBody : Utilisé avec les méthodes PUT ou POST par exemple cette annotation permet de récupérer le body de la requête pour le mapper directement vers une DTO.