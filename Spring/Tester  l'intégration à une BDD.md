Il y a deux possibilités :
- H2 Database (https://www.h2database.com/html/main.html)
- Testcontainers (https://java.testcontainers.org/)

H2
--------------------------
Il est possible d'activer une base données H2 lors des tests d'intégration afin de valider les mappings JPA ainsi que les requêtes. Puisque celle-ci peut être démarré en mode in-memory elle sera automatiquement effacée par la suite. 

Par contre cela ne reflète pas forcément le SGBD utilisé en produtction

Testcontainers
--------------------------
Testcontainers permet de configurer des images docker qui sont automatiquement récupérées lors des tests d'intégration afin de ne avoir besoin d'une instance du container en route sur sa machine lors de ceux-ci.

On peut donc utiliser ceux-ci pour effectuer des tests en liens avec un SGBD en particulier et valider nos requêtes ainsi que nos configurations de BDD

Cependant, cela peut nécessiter un peu de configuration en amont pour créer toutes les tables dans la base mais cela est acceptable vu que ce sont des tests d'intégrations et qu'ils sont sensés être plus lents que les tests unitaires.

