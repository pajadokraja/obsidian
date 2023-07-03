#javascript #number #function 
## Opis
Vraca true ako je vrednost konacan broj, false ako nije broj ili je beskonacnost.

## Sintaksa:
isFinite(number), gde:
- number je broj koji testiramo

## Nacin koriscenja:
```js
isFinite(2); // True
isFinite(0); // True
isFinite(2/0); // False
isFinite("HAHA"); // False
```

Ukoliko argument nije [[number]], automatski vraca false.

[[isNaN()]]