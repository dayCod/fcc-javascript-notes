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

### Escaping Literal Quotes in Strings
```js
const MY_STR = "I am a \"double quoted\" string inside \"double quotes\".";
```

### Quoting Strings with Single Quotes
```js
const MY_STR = '<a href="http://www.example.com" target="_blank">Link</a>';
```

### Escape Sequences in Strings
```js
const MY_STR = "FirstLine\n\t\\SecondLine\nThirdLine";

// return below format
/**
 * FirstLine
 *      \SecondLine
 * ThirdLine
*/
```

### Concatenating Strings with Plus Operator
```js
const MY_STR = "This is the start. " + "This is the end.";
```

### Concatenating Strings with the Plus Equals Operator
```js
let myStr = "This is the first sentence. ";
myStr += "This is the second sentence.";
```

### Constructing Strings with Variables
```js
const myName = "john william doe";
const myStr = "hi " + myName + " how are you ?";
```

### Appending Variables to Strings
```js
const someAdjective = "awesome cool and marvelous";
let myStr = "Learning to code is ";
myStr += someAdjective;
```

### Find the Length of a String
```js
let lastNameLength = 0;
const lastName = "Lovelace";
lastNameLength = lastName.length;
```

### Use Bracket Notation to Find the First Character in a String
```js
let firstLetterOfLastName = "";
const lastName = "Lovelace";

firstLetterOfLastName = lastName[0];
```

### Understand String Immutability
```js
let myStr = "Jello World";
myStr = "Hello World";
console.log(myStr);
```

### Use Bracket Notation to Find the Nth Character in a String
```js
const lastName = "Lovelace";
const thirdLetterOfLastName = lastName[2];
```

### Use Bracket Notation to Find the Last Character in a String
```js
const lastName = "Lovelace";
const lastLetterOfLastName = lastName[lastName.length - 1];
```

### Use Bracket Notation to Find the Nth-to-Last Character in a String
```js
const lastName = "Lovelace";
const secondToLastLetterOfLastName = lastName[lastName.length - 2];
```

### Word Blanks
```js
const myNoun = "dog";
const myAdjective = "big";
const myVerb = "ran";
const myAdverb = "quickly";

let wordBlanks = "my " + myNoun + " is " + myAdjective + " and " + myVerb + " " + myAdverb; 
console.log(wordBlanks)
```

### Store Multiple Values in one Variable using JavaScript Arrays
```js
const myArray = ["string", 1];
```

### Nest one Array within Another Array
```js
const myArray = [["bulls", 23]];
```
