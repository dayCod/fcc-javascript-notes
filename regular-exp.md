### Using the Test Method
```js
let myString = "Hello, World!";
let myRegex = /Hello/;
let result = myRegex.test(myString); // Change this line
```

### Match Literal Strings
```js
let waldoIsHiding = "Somewhere Waldo is hiding in this text.";
let waldoRegex = /Waldo/; // Change this line
let result = waldoRegex.test(waldoIsHiding);
```

### Match a Literal String with Different Possibilities
```js
let petString = "James has a pet cat.";
let petRegex = /has a pet dog|cat|bird|fish/; // Change this line
let result = petRegex.test(petString);
```

### Ignore Case While Matching
```js
let myString = "freeCodeCamp";
let fccRegex = /freecodecamp/i; // Change this line
let result = fccRegex.test(myString);
```