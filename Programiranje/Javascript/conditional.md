#javascript 
If, else, else if rade normano:
```javascript
if (age > 18) {
	accessAllowed = true; 
}
else {
	accessAllowed = false; 
}
```
? se moze koristiti umesto if else, takodje se moze povezivati vise njih za redom
```javascript
let message = (age < 3) ? 'Hi, baby!' :
	(age < 18) ? 'Hello!' :
	(age < 100) ? 'Greetings!' :
	'What an unusual age!';
```
Takodje postoji i switch. Sintaksa:
```javascript
switch(x) {
	case 'value1': // if (x === 'value1')
	... [break]
	case 'value2': // if (x === 'value2')
	... [break]
	default: 
	... [break]
	}
	// Switch uvek koristi ===
```