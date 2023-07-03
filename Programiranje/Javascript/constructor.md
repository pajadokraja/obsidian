[[function]] koja pravi [[object]].
```js
function User(name) {
	this.name = name;
	this.sayHi = function() {
		alert( "My name is: " + this.name ); 
	};
} 
_let john = new User("John");
john.sayHi(); // My name is: John
```
Konveckija je da je prvo slovo imena konstruktora veliko i da se samo pozivaju sa new.