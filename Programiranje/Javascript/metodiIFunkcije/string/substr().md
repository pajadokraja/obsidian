#javascript #method #string #substring 
## Opis
Vraca string duzine length pocevsi od start.

## Sintaksa:
string.substr(start, length), gde:
- start je index od koga pocinje
- length je duzina stringa koji vraca

## Nacin koriscenja:
```js
let str = "stringify";
alert( str.substr(2, 4) ); // 'ring', from the 2nd position get 4 characters
alert( str.substr(-4, 2) ); // 'gi', from the 4th position get 2 characters
```

Pocetak moze da bude negativan. U teoriji nije podrzan od nekih brauzera, ali u praksi jeste. Redje se koristi od drugih slicnih metoda.

[[slice()]]
[[substring()]]