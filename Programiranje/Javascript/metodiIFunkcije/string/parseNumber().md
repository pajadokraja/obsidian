Ne postoji konkretno ovaj [[method]], ali postoje:
```js
parseInt("123px"); // 123
parseFloat("60.9.11"); //60.9

// Citaju sa leva na desno i traze int/float dokle god mogu. Mogu se koristiti
// sa drugim argumentom, radix, koji odredjuje bazu:

parseInt("2n9c", 36); // 123456
```