#javascript 
Objekti su [[dataType]] koji sadrze [[property]]s.
```js
let user = { // Object literal sintaksa
	name: "John",
	age: 30
};

// Drugi nacin da napravimo objekat: (object constructor sintaksa)
let user = Object();
```
Ako zelimo da pristupimo nekom propertiju:
```js
obj.property
obj["property"]
// Ako koristimo [], mozemo da koristimo varijablu da pristupimo propertiju,
// tako da je to mocnija opcija, ali u jednostavnim slucajevima koristimo .
```
Ako zelimo da radimo na propertiju:
```js
delete obj.prop // brise property iz objekta
"key" in obj // proverava da li postoji property sa kljucem key u objektu obj
for (let key in obj) // loopujemo nad objektom
```

Objekti su dodeljeni i kopirani preko reference. To znaci da se u [[variable]] kojoj je dodeljen objekat ne nalazi zapravo taj objekat vec referenca ka njemu.
Da bismo klonirali objekat moramo da koristimo metode za to [[object.assign()]] (shallow klon) odnosno [[structuredClone]] (deep/structured klon).
[[method]] je funckija u objektu

## [[constructor]]
Funckija koja pravi objekte.

## ?.

Mozemo koristiti ako nismo sigurni da li neki property objekta postoji i zelimo da vratimo undefined umesto da bude greska:
```js
let user = {}; // user has no address alert

user?.address?.street; // undefined (no error)
```

## Konverzija u primitivne tipove:
The object-to-primitive conversion is called automatically by many built-in functions and operators that expect a primitive as a value.

There are 3 types (hints) of it:

- `"string"` (for `alert` and other operations that need a string)
- `"number"` (for maths)
- `"default"` (few operators, usually objects implement it the same way as `"number"`)

The specification describes explicitly which operator uses which hint.

The conversion algorithm is:

1. Call `obj[Symbol.toPrimitive](hint)` if the method exists,
2. Otherwise if hint is `"string"`
    - try calling `obj.toString()` or `obj.valueOf()`, whatever exists.
3. Otherwise if hint is `"number"` or `"default"`
    - try calling `obj.valueOf()` or `obj.toString()`, whatever exists.

All these methods must return a primitive to work (if defined).

In practice, it’s often enough to implement only `obj.toString()` as a “catch-all” method for string conversions that should return a “human-readable” representation of an object, for logging or debugging purposes.