Cucumber est un outil orienté BDD.
Celui-ci permet de définir des scénarios en suivant la syntaxe Gherkin et de définir des scénario avec des steps Given, When, Then. Par la suite ces étapes sont implémentées avec le code correspondant.

Un des avantages de faire du Gherkin est qu'il permet aux personnes moins TI d'exprimer le besoin affaire autour du comportement attendu de l'application.

Un autre avantage est que la définition des scénarios en Gherkin permet de servir de documentation vivant grâce à sa syntaxe naturelle.

Il est généralement conseillé de mener des atelier d'example mapping pour définir les scénarios a implémenter.

Example de scénario : ´
	Scenario : Un utilisateur se connecte
		Given un utilisateur tente de se connecter
		When ses identifiants sont bon
		Then l'utilisateur est connecté
´