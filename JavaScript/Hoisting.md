Hoisting consiste a appeler une variable avant sa définition.

Cette variable se doit d'être défini par l'un des mots clés suivants :
- function (2)
- function* (2)
- async function (2)
- async function* (2)
- var (1)
- const (3)
- let (3)
- class (3)
- import (2, 4)

- Être capable d'utiliser une variable avant qu'elle soit déclarée sans déclencher une erreur de référence :
	´
	console.log(a); // undefined
	
	var a = "123";
	console.log(a) // 123
	´
- Être capable d'utiliser la valeur d'une variable avant sa définition :
	´
	console.log(someObject.someValue); // undefined
	
	var someObject = {
		someValue: "123"
	}
	console.log(someObject.someValue); // 123
	´
- The declaration of the variable causes behavior changes in its scope before the line in which it is declared.
- The side effects of a declaration are produced before evaluating the rest of the code that contains it.