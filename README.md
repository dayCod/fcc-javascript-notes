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

### Access Array Data with Indexes
```js
const myArray = [50, 60, 70];

const myData = myArray[0];
```

### Modify Array Data With Indexes
```js
const myArray = [18, 64, 99];
myArray[0] = 45;

console.log(myArray)
```

### Access Multi-Dimensional Arrays With Indexes
```js
const myArray = [
  [1, 2, 3],
  [4, 5, 6],
  [7, 8, 9],
  [[10, 11, 12], 13, 14],
];

const myData = myArray[2][1];
```

### Manipulate Arrays With push Method
```js
const myArray = [["John", 23], ["cat", 2]];
myArray.push(['dog', 3]);
console.log(myArray)
```

### Manipulate Arrays With pop Method
```js
const myArray = [["John", 23], ["cat", 2]];
let removedFromMyArray = myArray.pop();
console.log(removedFromMyArray)
```

### Manipulate Arrays With shift Method
```js
const myArray = [["John", 23], ["dog", 3]];
let removedFromMyArray = myArray.shift()
console.log(removedFromMyArray)
```

### Manipulate Arrays With unshift Method
```js
const myArray = [["John", 23], ["dog", 3]];
myArray.shift();

myArray.unshift(["Paul", 35])
console.log(myArray)
```

### Shopping List
```js
const myList = [
  ["Shampoo", 15],
  ["Kitkat", 15],
  ["Bodywash", 15],
  ["Corn", 15],
  ["Cheese", 15],
];
```

### Write Reusable JavaScript with Functions
```js
function reusableFunction() {
  console.log("Hi World");
}

reusableFunction()
```

### Passing Values to Functions with Arguments
```js
function functionWithArgs(num1, num2) {
  console.log(num1 + num2);
}

functionWithArgs(1, 2)
functionWithArgs(7, 9)
```

### Return a Value from a Function with Return
```js
function timesFive(number){
  return number * 5;
}

timesFive(5);
timesFive(2);
timesFive(0);
```

### Global Scope and Functions
```js
// Declare the myGlobal variable below this line
const myGlobal = 10;
const oopsGlobal = 5;

function fun1() {
  // Assign 5 to oopsGlobal here
  return oopsGlobal;
}

// Only change code above this line

function fun2() {
  let output = "";
  if (typeof myGlobal != "undefined") {
    output += "myGlobal: " + myGlobal;
  }
  if (typeof oopsGlobal != "undefined") {
    output += " oopsGlobal: " + oopsGlobal;
  }
  console.log(output);
}

```

### Local Scope and Functions
```js
function myLocalScope() {
  // Only change code below this line
  const myVar = "foo";
  console.log('inside myLocalScope', myVar);
}
myLocalScope();

console.log('outside myLocalScope', myLocalScope());
```

### Global vs. Local Scope in Functions
```js
// Setup
const outerWear = "T-Shirt";

function myOutfit() {
  // Only change code below this line
  const outerWear = "sweater";
  // Only change code above this line
  return outerWear;
}

myOutfit();
```

### Understanding Undefined Value returned from a Function
```js
// Setup
let sum = 0;

function addThree() {
  sum = sum + 3;
}

// Only change code below this line
function addFive() {
  sum = sum + 5;
}

// Only change code above this line

addThree();
addFive();
```

### Assignment with a Returned Value
```js
// Setup
let processed = 0;

function processArg(num) {
  return (num + 3) / 5;
}

// Only change code below this line
processed = processArg(7)
```

### Stand in Line
```js
function nextInLine(arr, item) {
  // Only change code below this line
  arr.push(item);
  const removed = arr.shift();
  return removed;
  // Only change code above this line
}

// Setup
let testArr = [1, 2, 3, 4, 5];

// Display code
console.log("Before: " + JSON.stringify(testArr));
console.log(nextInLine(testArr, 6));
console.log("After: " + JSON.stringify(testArr));
```

### Understanding Boolean Values
```js
function welcomeToBooleans() {
  // Only change code below this line

  return true; // Change this line

  // Only change code above this line
}
```

### Use Conditional Logic with If Statements
```js
function trueOrFalse(wasThatTrue) {
  // Only change code below this line

  if (wasThatTrue) {
    return "Yes, that was true";
  }

  return "No, that was false";


  // Only change code above this line

}
```

### Comparison with the Equality Operator
```js
// Setup
function testEqual(val) {
  if (val == 12) { // Change this line
    return "Equal";
  }
  return "Not Equal";
}

testEqual(10);
```

### Comparison with the Strict Equality Operator
```js
// Setup
function testStrict(val) {
  if (val === 7) { // Change this line
    return "Equal";
  }
  return "Not Equal";
}

testStrict(10);
```

### Practice comparing different values
```js
// Setup
function compareEquality(a, b) {
  if (a === b) { // Change this line
    return "Equal";
  }
  return "Not Equal";
}

compareEquality(10, "10");
```

### Comparison with the Inequality Operator
```js
// Setup
function testNotEqual(val) {
  if (val != "99") { // Change this line
    return "Not Equal";
  }
  return "Equal";
}

testNotEqual(10);
```

### Comparison with the Strict Inequality Operator
```js
// Setup
function testStrictNotEqual(val) {
  if (val !== 17) { // Change this line
    return "Not Equal";
  }
  return "Equal";
}

testStrictNotEqual(10);
```

### Comparison with the Greater Than Operator
```js
function testGreaterThan(val) {
  if (val > 100) {  // Change this line
    return "Over 100";
  }

  if (val > 10) {  // Change this line
    return "Over 10";
  }

  return "10 or Under";
}

testGreaterThan(10);
```

### Comparison with the Greater Than Or Equal To Operator
```js
function testGreaterOrEqual(val) {
  if (val >= 20) {  // Change this line
    return "20 or Over";
  }

  if (val >= 10) {  // Change this line
    return "10 or Over";
  }

  return "Less than 10";
}

testGreaterOrEqual(10);
```

### Comparison with the Less Than Operator
```js
function testLessThan(val) {
  if (val < 25>) {  // Change this line
    return "Under 25";
  }

  if (val < 55>) {  // Change this line
    return "Under 55";
  }

  return "55 or Over";
}

testLessThan(10);
```

### Comparison with the Less Than Or Equal To Operator
```js
function testLessOrEqual(val) {
  if (val <= 12) {  // Change this line
    return "Smaller Than or Equal to 12";
  }

  if (val <= 24) {  // Change this line
    return "Smaller Than or Equal to 24";
  }

  return "More Than 24";
}

testLessOrEqual(10);
```

### Comparisons with the Logical And Operator
```js
function testLogicalAnd(val) {
  // Only change code below this line

  if (val >= 25 && val <= 50) {
      return "Yes";
  }

  // Only change code above this line
  return "No";
}

testLogicalAnd(10);
```

### Comparisons with the Logical Or Operator
```js
function testLogicalOr(val) {
  // Only change code below this line

  if (val < 10 || val > 20) {
    return "Outside";
  }

  // Only change code above this line
  return "Inside";
}

testLogicalOr(15);
```

### Introducing Else Statements
```js
function testElse(val) {
  let result = "";
  // Only change code below this line

  if (val > 5) {
    result = "Bigger than 5";
  } else {
    result = "5 or Smaller";
  }

  // Only change code above this line
  return result;
}

testElse(4);
```

### Introducing Else If Statements
```js
function testElseIf(val) {
  if (val > 10) {
    return "Greater than 10";
  }else if (val < 5) {
    return "Smaller than 5";
  }else {
    return "Between 5 and 10";
  }
}

testElseIf(7);
```

### Logical Order in If Else Statements
```js
function orderMyLogic(val) {
  if (val < 10 && val > 5) {
    return "Less than 10";
  } else if (val < 5) {
    return "Less than 5";
  } else {
    return "Greater than or equal to 10";
  }
}

console.log(orderMyLogic(4))
orderMyLogic(6);
orderMyLogic(11);
```

### Chaining If Else Statements
```js
function testSize(num) {
  // Only change code below this line
  let result = "";
  if (num < 5) {
    result += "Tiny";
  } else if (num < 10) {
    result += "Small";
  } else if (num < 15) {
    result += "Medium";
  } else if (num < 20) {
    result += "Large";
  } else if (num >= 20) {
    result += "Huge";
  } else {
    result += "Change Me";
  }

  return result;

  // Only change code above this line
}

testSize(7);
```

### Golf Code
```js
const names = ["Hole-in-one!", "Eagle", "Birdie", "Par", "Bogey", "Double Bogey", "Go Home!"];

function golfScore(par, strokes) {
  // Only change code below this line
  let result = "";

  if (strokes == 1) {
    result += names[0];
  } else if (strokes <= (par - 2)) {
    result += names[1];
  } else if (strokes == (par-1)) {
    result += names[2];
  } else if (strokes == par) {
    result += names[3];
  } else if (strokes == (par + 1)) {
    result += names[4];
  } else if (strokes == (par + 2)) {
    result += names[5];
  } else if (strokes >= (par + 3)) {
    result += names[names.length - 1];
  } 

  return result;
  // Only change code above this line
}

golfScore(5, 4);
```

### Selecting from Many Options with Switch Statements
```js
function caseInSwitch(val) {
  let answer = "";
  // Only change code below this line
  switch(val) {
    case 1:
      answer += "alpha";
      break;
    case 2:
      answer += "beta";
      break;
    case 3:
      answer += "gamma";
      break;
    case 4:
      answer += "delta";
      break;
  }

  // Only change code above this line
  return answer;
}

caseInSwitch(1);
```

### Adding a Default Option in Switch Statements
```js
function switchOfStuff(val) {
  let answer = "";
  // Only change code below this line
  switch (val) {
    case "a":
      answer += "apple";
      break;
    case "b":
      answer += "bird";
      break;
    case "c":
      answer += "cat";
      break;
    default:
      answer += "stuff";
      break
  }


  // Only change code above this line
  return answer;
}

switchOfStuff(1);
```

### Multiple Identical Options in Switch Statements
```js
function sequentialSizes(val) {
  let answer = "";
  // Only change code below this line
  
  switch (val) {
    case 1:
    case 2:
    case 3:
      answer += "Low";
      break;
    case 4:
    case 5:
    case 6:
      answer += "Mid";
      break;
    case 7:
    case 8:
    case 9:
      answer += "High";
      break;
  }


  // Only change code above this line
  return answer;
}

sequentialSizes(1);
```

### Replacing If Else Chains with Switch
```js
function chainToSwitch(val) {
  let answer = "";
  // Only change code below this line

  switch (val) {
    case "bob":
      answer = "Marley";
      break;
    case 1:
      answer = "There is no #1";
      break;
    case 7:
      answer = "Ate Nine";
      break;
    case 42:
      answer = "The Answer";
      break;
    case 99:
      answer = "Missed me by this much!";
      break;
  }

  // Only change code above this line
  return answer;
}

chainToSwitch(7);
```

### Returning Boolean Values from Functions
```js
function isLess(a, b) {
  // Only change code below this line
  return (a < b) ? true : false;
  // Only change code above this line
}

isLess(10, 15);
```

### Return Early Pattern for Functions
```js
// Setup
function abTest(a, b) {
  // Only change code below this line

  if (a < 0 || b < 0) return undefined

  // Only change code above this line

  return Math.round(Math.pow(Math.sqrt(a) + Math.sqrt(b), 2));
}

console.log(abTest(2,-2))
```

### Counting Cards
```js
let count = 0;

function cc(card) {
  // Only change code below this line
  var regex = /[JQKA]/;
  if (card > 1 && card < 7) {
    count++;
  } else if (card === 10 || regex.test(card)) {
    count--;
  }

  if (count > 0) return count + " Bet";
  return count + " Hold";

  // Only change code above this line
}
console.log(cc('2'))
cc(2); cc(3); cc(7); cc('K'); cc('A');
```

### Build JavaScript Objects
```js
const myDog = {
  // Only change code below this line
  "name": "AxeWall",
  "legs": 4,
  "tails": 1,
  "friends": ["Paw", "Undefined"]

  // Only change code above this line
};
```

### Accessing Object Properties with Dot Notation
```js
// Setup
const testObj = {
  "hat": "ballcap",
  "shirt": "jersey",
  "shoes": "cleats"
};

// Only change code below this line
const hatValue = testObj.hat;      // Change this line
const shirtValue = testObj.shirt;    // Change this line
```

### Accessing Object Properties with Bracket Notation
```js
// Setup
const testObj = {
  "an entree": "hamburger",
  "my side": "veggies",
  "the drink": "water"
};

// Only change code below this line
const entreeValue = testObj["an entree"];   // Change this line
const drinkValue = testObj["the drink"];    // Change this line
```

### Accessing Object Properties with Variables
```js
// Setup
const testObj = {
  12: "Namath",
  16: "Montana",
  19: "Unitas"
};

// Only change code below this line
const playerNumber = 16;  // Change this line
const player = testObj[playerNumber];   // Change this line
```

### Updating Object Properties
```js
// Setup
const myDog = {
  "name": "Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

// Only change code below this line
myDog['name'] = "Happy Coder";
```

### Add New Properties to a JavaScript Object
```js
const myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"]
};

myDog.bark = "bow-wow";
```

### Delete Properties from a JavaScript Object
```js
// Setup
const myDog = {
  "name": "Happy Coder",
  "legs": 4,
  "tails": 1,
  "friends": ["freeCodeCamp Campers"],
  "bark": "woof"
};

// Only change code below this line
delete myDog.tails;
```

### Using Objects for Lookups
```js
// Setup
function phoneticLookup(val) {
  let result = "";

  // Only change code below this line
  const lookup = {
    "alpha": "Adams",
    "bravo": "Boston",
    "charlie": "Chicago",
    "delta": "Denver",
    "echo": "Easy",
    "foxtrot": "Frank",
    "": undefined,
  }
  result = lookup[val];
  // Only change code above this line
  return result;
}

phoneticLookup("charlie");
```

### Testing Objects for Properties
```js
function checkObj(obj, checkProp) {
  // Only change code below this line
  return (obj.hasOwnProperty(checkProp)) ? obj[checkProp] : 'Not Found';
  // Only change code above this line
}

console.log(checkObj({gift: "pony", pet: "kitten", bed: "sleigh"}, "gift"))
```

### Manipulating Complex Objects
```js
const myMusic = [
  {
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [
      "CD",
      "8T",
      "LP"
    ],
    "gold": true
  }
];

myMusic.push({
    "artist": "Billy Joel",
    "title": "Piano Man",
    "release_year": 1973,
    "formats": [
      "CD",
      "8T",
      "LP"
    ],
    "gold": true
  });

console.log(myMusic);
```

### Accessing Nested Objects
```js
const myStorage = {
  "car": {
    "inside": {
      "glove box": "maps",
      "passenger seat": "crumbs"
     },
    "outside": {
      "trunk": "jack"
    }
  }
};

const gloveBoxContents = myStorage.car.inside["glove box"];
```

### Accessing Nested Arrays
```js
const myPlants = [
  {
    type: "flowers",
    list: [
      "rose",
      "tulip",
      "dandelion"
    ]
  },
  {
    type: "trees",
    list: [
      "fir",
      "pine",
      "birch"
    ]
  }
];

const secondTree = myPlants[1].list[1];

console.log(secondTree);
```

### Record Collection
```js

// Setup
const recordCollection = {
  2548: {
    albumTitle: 'Slippery When Wet',
    artist: 'Bon Jovi',
    tracks: ['Let It Rock', 'You Give Love a Bad Name']
  },
  2468: {
    albumTitle: '1999',
    artist: 'Prince',
    tracks: ['1999', 'Little Red Corvette']
  },
  1245: {
    artist: 'Robert Palmer',
    tracks: []
  },
  5439: {
    albumTitle: 'ABBA Gold'
  }
};

// Only change code below this line
function updateRecords(records, id, prop, value) {
  // Access target album in record collection
  const album = records[id];
  // Update the album
  if (value === "") {
    delete album[prop];
  } else if (prop !== "tracks") {
    album[prop] = value;
  } else {
    album["tracks"] = album["tracks"] || [];
    album["tracks"].push(value);
  }
  // Return the full collection
  return records;
}

updateRecords(recordCollection, 5439, 'artist', 'ABBA');

console.log(updateRecords(recordCollection, 5439, 'artist', 'ABBA'));

```

### Iterate with JavaScript While Loops
```js
// Setup
const myArray = [];

// Only change code below this line
let num = 0;

while (num < 6) {
  myArray.push(num);
  num++;
}

console.log(myArray.sort().reverse())
```

### Iterate with JavaScript For Loops
```js
// Setup
const myArray = [];

// Only change code below this line

for (let num = 1; num <= 5; num++) {
  myArray.push(num);
}

console.log(myArray);
```

### Iterate Odd Numbers With a For Loop
```js
// Setup
const myArray = [];

// Only change code below this line
for (let i = 1; i < 10; i += 2) {
  myArray.push(i);
}

console.log(myArray)
```

### Count Backwards With a For Loop
```js
// Setup
const myArray = [];

// Only change code below this line

for (let i = 9; i > 0; i -= 2) {
  myArray.push(i);
}

console.log(myArray);
```

### Iterate Through an Array with a For Loop
```js
// Setup
const myArr = [2, 3, 4, 5, 6];

// Only change code below this line
let total = 0;

for (let i = 0; i < myArr.length; i++) {
   total += myArr[i];
}
```
