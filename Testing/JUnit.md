Comment tester les exceptions
--------------------------

assertThrows permet de valider qu'une exception est bien déclenchée au sein d'une méthode.
Il est possible de récupérer l'exception retournée afin d'effectuer d'autres traitements sur celle-ci.
Exemple : ´
	MyException someException = assertThrows(MyException.class, () -> aMethodThatShouldThrow());
´

assertDoesNotThrow permet de valider au contraire qu'une exception n'est pas déclenchée. 
Exemple : ´
	assertDoesNotThrow(() -> aMethodThatShouldNotThrow();
´




