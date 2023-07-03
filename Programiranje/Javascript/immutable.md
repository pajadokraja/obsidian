Ne moze se promeniti (ugl se odnosi na nizove, ako je niz immutable onda ne mozemo da ga promenimo "na mestu", vec moramo da ga prekopiramo u samog sebe praveci izmene)
```js
let rec = "HELLO";
rec[0] = 'h'; // Greska
rec = 'h' + rec.slice(1); // hELLO
```