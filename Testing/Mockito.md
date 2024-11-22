C'est une librairie utilisée pour faire des mocks

Mock
--------------------------

Permet de copier la structure d'une classe ou d'une interface cependant aucune fonction n'est disponible par défaut. Il faut créer ce qu'on appelle des stub pour ces fonctions afin de leur donner une fausse implémentation que l'on contrôle.
Utile lorsque l'on ne souhaite pas appeler une API externe au sein de nos tests et ainsi ls garder isolés.

Spy
--------------------------
Mocking partiel, les vraies méthodes seront invoquées mais elles peuvent être tout de même stubbed et vérifiés.

On va surtout l'utiliser lorsque l'on veut valider que certaines fonctions ont bien été appelées tout en gardant l'implémentation natives pour ne pas avoir à définir plusieurs stubs