#javascript 
Nizovi karaktera. U javscriptu, stringovi su [[immutable]].

Mozemo ih korstiti sa "", '' (ova dva su ista) ili \`\` (dodatna funkcionalnost)
```js
"String"

'String'

`Str
${1+2}
ing
`		// Str
		// 3
		// ing
```

## length
string.length je [[property]] (ne [[method]]) stringa, vrace njegovu duzinu:
```js
"bla\nbla\nbla".length // 11
```

## pristup karakterima
mozemo pristupiti karakterima koristeci \[\] ili pomocu [[at()]] metoda:
```js
"blablabla"[3] // b
"blablabla".at(-4) // a
```

mozemo i iterirati kroz karaktere koristeci sledeci [[loop]]:
```js
for (let char of "Hello"){
	console.log(char); // H e l l o
}

// ponasanje sa in umesto of:
for (let char of "Hello"){
	console.log(char); // 0 1 2 3 4
}
```

## [[method]]e vezane za stringove:

- ### promena velicine:
[[toUpper()]]
[[toLower()]]
- ### pretrazivanje za podstring:
[[indexOf()]]
[[lastIndexOf()]]
[[includes()]]
[[startsWith()]]
[[endsWith()]]
- ### dobijanje podstringa:
[[slice()]]
[[substring()]]
[[substr()]]