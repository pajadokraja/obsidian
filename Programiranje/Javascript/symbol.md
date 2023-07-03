Simboli su posebni identifikatori, u sustini to su samo jako veliki brojevi. Sintaksa:
```js
Symbol("description"); // description ne utice na to koji broj je generisan

let id1 = Symbol("id");
let id2 = Symbol("id"); 

alert(id1 == id2); // false

// Ukoliko zelimo da za iste deskripcije dobijemo isti simbol (ovo
// se zove globalni simbol), koristimo:

let id1 = Symbol.for("id");
let id2 = Symbol.for("id");

alert(id1 === id2); // true

// Ukoliko zelimo da uradimo suprotno od ovoga - da dobijemo deskripciju za
// neku vrstu globalnog simbola - koristimo forKey:

let key = Symbol.forKey(id1); // vraca "id"

// Ukoliko zelimo da koristimo simbole za kljuc propertyja:
[id] : 123;

// Simboli su "nevidljivi" - for key in obj ih preskace, ali i dalje mozemo da
// im eksplicitno pristupimo. Prenose se kada ih kloniramo

```
