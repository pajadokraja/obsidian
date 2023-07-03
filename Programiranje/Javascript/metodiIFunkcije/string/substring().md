#javascript #method #string #substring 
## Opis
Vraca podstring izmedju start i end. Ukoliko je start > end, zameni im mesta

## Sintaksa:
string.substring(start, end), gde:
- start je prvi index
- end je opcioni drugi index. Ukoliko nije dat ide do kraja stringa.

## Nacin koriscenja:
```js
let str = "stringify";

str.substring(2, 6); // "ring"
str.substring(6, 2); // "ring"
```

Negativni brojevi se pretvore u 0. Prednost je sto start moze biti vece od end.

[[slice()]]
[[substr()]]