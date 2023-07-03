#javascript 
Funkcije su kod koji mozemo da koristimo vise puta (umesto da kopi pejstujemo i menjamo svaki put).
```javascript
function name(parameter1, parameter2){
	// code
	return value; // optional return statement
}
```

name je ime funkcije
parametri su u zagradi - moze ih biti koliko hocemo
value je vrednost koju funkcija vraca. Ukoliko ne vraca vrednost, onda vraca [[undefined]]. Kada se stigne do return funkcija prekida sa izvodjenjem.

[[variable]] deklarisane u funkciji su dostupne samo u toj funkciji - lokalne su
funckije takodje mogu da pristupe globalnim varijablama i da ih menjaju
ukoliko postoje dve varijable sa istim imenom, funckija uzima lokalnu

## Function statement

funkcije su zapravo varijable koje predstavljaju akciju (mozemo ih kopirati u druge varijable isl)
mozemo stvoriti funkciju u okviru [[statement]]-a - ovo je function expression
```js
let message = function(name){
	alert(`Hello, ${name}`);
}; // obavezno ; na kraju
```
U nekim situacijama je ovako bolje raditi sa funkcijama - recimo ako zelimo samo da izvrsimo funkciju u jednom delu koda, bez da je imenujemo - anonimna funkcija
Ovakve funkcije dostupne su samo u okviru bloka koda u kome su stvorene

## Arrow function
```js
let func = (param1, param2) => expression;

// ovo iznad je kraca verzija:
let func = function(param1, param2){
	return expression;
};

```
arrow funkcije nemaju this. Ako se upotrebi this u njima, koristice ka "spolja"