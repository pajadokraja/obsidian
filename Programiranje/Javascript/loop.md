#javascript #loops
```javascript
while(condition){
	// code
}

do{
	// code
}while(condition)

// razlika je u tome da li prvo proveravamo uslov pa radimo kod ili prvo radimo kod pa proverimo uslov

for(begin;condition;step){
	// code
	// begin je statement koji se obavi na pocetku loop-a (ako deklarisemo varijable ovde onda su vidljive samo unutar loop-a). Condition se proverava pre svake iteracije, ako je false loop prestaje. Step je statement koji se obavi na kraju svake iteracije. Svaki od ovih delova moze da se preskoci ukoliko nam iz nekog razloga nije potreban
}

```

## break
Mozemo da korsitimo break da izadjemo iz loop-a u bilo kom trenutku

## continue
Koristimo da preskocimo ostatak trenutne iteracije i predjemo na sledecu

break i continue ne mozemo da korsitimo u sintaksnim konstruktima koji nisu statement-i
Ako imamo loopove u loopovima, mozemo da odredimo na koji od njih se odnose break i continue tako sto loopovima dodelimo label (imeLabel: dopisemo pre pocetka loopa) i onda koristimo "break imeLabel"