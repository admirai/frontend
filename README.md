# About this repository
# Best practises
# Image Gallery
# Async API Data



#### The good ol' use strict thingie
Strictly use use strict! This is nothing more than just adding string put in your code that adds more magic to your script.


#### Use Single "var" Declaration per Scope
Since "var" accepts multiple declarations there is no reason to use more. All scope variables are moved to the top of the scope anyway (this is called hoisting). This may help reduce potential unexpected behavior in case duplicate names are introduced or some other logical mistakes are made.

#### Use Strict
Before ECMAScript 5 you were allowed to assign to variable that is not declared it would create it in a global scope:

(function(){
    name = 'John';
}());
With "use strict" you would just get an error:

(function(){
    'use strict';
    name = 'John';
}());
It helps you avoid introducing global variables inadvertently and spot errors early.

#### Declaraties bovenaan
Het is goed om alle declaraties bovenaan het script te zetten.
dit zorgt voor:
-schone code
-1 plek om te zoeken waar lokale variableen zich bevinden.
-zorgt voor minder kans op re-declarations, dus dat je ze opnieuw doet.
https://www.w3schools.com/js/js_best_practices.asp
