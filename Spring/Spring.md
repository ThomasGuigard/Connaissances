
Qu'est ce qu'un bean
--------------------------

Un bean est une composant principale de Spring, généralement c'est un singleton. Celui-ci est géré par Spring.

Lors du démarrage d'une application Spring, un scan est effectué pour trouver tous les bean à instancier. Ceux-ci "meurent" en général lorsque l'application s'arrête.

Sinon son cycle de vie est le suivant :
- Instanciation
- Configuration
- Initialisation
- Utilisation
- Destruction

Design Patterns
--------------------------

Voici quelques designs patterns utilisés au sein de Spring
- Decorator : On le retrouve au travers des différentes annotations Spring tels que @Controller, @Service ou @Bean. Celui-ci permet d'ajouter un nouveau comportement a une classe sans en modifier son code (voir https://refactoring.guru/design-patterns/decorator)
- Singleton : Un classique, permet d'avoir une instance unique pour un objet. Attention cependant aux problèmes de synchronisation éventuels si celui est défini à la main (voir https://refactoring.guru/design-patterns/singleton)
- Factory : Permet de créer différents objets partageant la même interface au sein de la même superclass. Notamment utilisée sur la gestion des WebClientResponseException (voir https://refactoring.guru/design-patterns/factory-method)
- Chain of responsibility : Permet de faire passer une requête au travers d'un enchainement d'handlers qui appliqueront a chaque fois une validation avant de la transmettre (parfois aussi appelé middleware notamment avec Express.js) (voir https://refactoring.guru/design-patterns/chain-of-responsibility)