# FCC Javascript Notes
This is a note for my javascript learning process at freeCodeCamp

### Comment your javascript Code
```js
// This is my first comment on free code camp.
/**
 * this is my second comment on free code camp
 */
```

### Declare Javascript Variable
```js
var myName;
```

### Storing Values with the Assignment Operator
```js
// Setup
var a;

// Only change code below this line
a = 7;
```

### Assigning the Value of One Variable to Another
```js
var a;
a = 7;
var b;
b = a;
```

### Initializing Variables with the Assignment Operator
```js
var a = 9;
```

### Declare String Variables
```js
var myFirstName = "Day";
var myLastName = "Cod";
```

### Understanding Uninitialized Variables
```js
var a = 5;
var b = 10;
var c = "I am a";

a = a + 1;
b = b + 5;
c = c + " String!";
```

### Understanding Case Sensitivity in Variables
```js
var studlyCapVar;
var properCamelCase;
var titleCaseOver;

studlyCapVar = 10;
properCamelCase = "A String";
titleCaseOver = 9000;
```

### Explore Differences Between the var and let Keywords
```js
let catName = "Oliver";
let catSound = "Meow!";
```

### Declare a Read-Only Variable with the const Keyword
```js
const FCC = "freeCodeCamp";
let fact = "is cool!";
fact = "is awesome!";
console.log(FCC, fact)
```

### Add Two Numbers with JavaScript
```js
const SUM = 10 + 10;
```

### Subtract One Number from Another with JavaScript
```js
const DIFFERENCE = 45 - 33;
```

### Multiply Two Numbers with JavaScript
```js
const PRODUCT = 8 * 10;
```


### Divide One Number by Another with JavaScript
```js
const QUOTIENT = 66 / 33;
```

### Increment a Number with JavaScript
```js
let myVar = 87;
myVar++

// equivalent to myVar = myVar + 1;
```

### Decrement a Number with JavaScript
```js
let myVar = 11;
myVar--;

// equivalent to myVar = myVar - 1;
```

### Create Decimal Numbers with JavaScript
```js
const MY_DECIMAL = parseFloat(5.7);

// if your input number is 5 it'll return 5.0;
```

### Multiply Two Decimals with JavaScript
```js
const PRODUCT = 2.0 * 2.5;

// return 5.0;
```

### Divide One Decimal by Another with JavaScript
```js
const QUOTIENT = 4.4 / 2.0;

// return 2.2;
```

### Finding a Remainder in JavaScript
```js
const REMAINDER = 8 % 3;

// return 2, because 8 / 3 = 2 remainder 2;
```

### Compound Assignment With Augmented Addition
```js
let a = 3;
let b = 17;
let c = 12;

a += 12;
b += 9;
c += 7;

// equivalent to a = a + 12;
```

### Compound Assignment With Augmented Subtraction
```js
let a = 11;
let b = 9;
let c = 3;

a -= 6;
b -= 15;
c -= 1;

// equivalent to a = a - 6;
```

### Compound Assignment With Augmented Multiplication
```js
let a = 5;
let b = 12;
let c = 4.6;

a *= 5;
b *= 3;
c *= 10;

// equivalent to a = a * 5;
```

### Compound Assignment With Augmented Division
```js
let a = 48;
let b = 100;
let c = 33;

a /= 12;
b /= 4;
c /= 11;

// equivalent to a = a / 12;

```