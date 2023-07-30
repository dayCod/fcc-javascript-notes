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

### Extract Matches
```js
let extractStr = "Extract the word 'coding' from this string.";
let codingRegex = /coding/i; // Change this line
let result = extractStr.match(codingRegex); // Change this line
```

### Find More Than the First Match
```js
let twinkleStar = "Twinkle, twinkle, little star";
let starRegex = /twinkle/gi; // Change this line
let result = twinkleStar.match(starRegex); // Change this line
```

### Match Anything with Wildcard Period
```js
let exampleStr = "Let's have fun with regular expressions!";
let unRegex = /.un/; // Change this line
let result = unRegex.test(exampleStr);
```