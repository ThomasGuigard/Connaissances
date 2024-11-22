
Qu'est ce qu'un bean
--------------------------

Définition

Cycle de vie


Design Patterns
--------------------------

Voici quelques designs patterns utilisés au sein de Spring
- Decorator : On le retrouve au travers des différentes annotations Spring tels que @Controller, @Service ou @Bean. Celui-ci permet d'ajouter un nouveau comportement a une classe sans en modifier son code (voir https://refactoring.guru/design-patterns/decorator)
- Singleton : Un classique, permet d'avoir une instance unique pour un objet. Attention cependant aux problèmes de synchronisation éventuels si celui est défini à la main (voir https://refactoring.guru/design-patterns/singleton)
- Factory : Permet de créer différents objets partageant la même interface au sein de la même superclass. Notamment utilisée sur la gestion des WebClientResponseException (voir https://refactoring.guru/design-patterns/factory-method)
- Chain of responsibility : Permet de faire passer une requête au travers d'un enchainement d'handlers qui appliqueront a chaque fois une validation avant de la transmettre (parfois aussi appelé middleware notamment avec Express.js) (voir https://refactoring.guru/design-patterns/chain-of-responsibility)