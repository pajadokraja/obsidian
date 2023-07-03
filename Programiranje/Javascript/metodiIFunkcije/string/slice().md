#javascript #method #string #substring
## Opis:
slice(start, end) vraca podstring izmedju start i end, ukljucuje start, ne ukljucuje end

## Sintaksa:
string.slice(start, end), gde:
- start je index pocetka podstringa
- end je opcioni argument, index kraja podstringa. Ukoliko nije dato, ide do kraja stringa.

## Nacin koriscenja:
```js
"Dobar dan".slice(0, 5); // Dobar
"Dobar dan".slice(6); // dan
"Dobar dan".slice(-6, -1); // ar da
```

Prednosti slice je sto radi sa negativnim brojevima.

[[substring()]]
[[substr()]]