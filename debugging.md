### Use the JavaScript Console to Check the Value of a Variable
```js
let a = 5;
let b = 1;
a++;
// Only change code below this line


let sumAB = a + b;
console.log(a);
```

### Understanding the Differences between the freeCodeCamp and Browser Console
```js
let output = "Get this to show once in the freeCodeCamp console and not at all in the browser console";
console.log(output);

console.clear()
```

### Use typeof to Check the Type of a Variable
```js
let seven = 7;
let three = "3";
console.log(seven + three);
// Only change code below this line
console.log(typeof seven);
console.log(typeof three);
```

### Catch Misspelled Variable and Function Names
```js
let receivables = 10;
let payables = 8;
let netWorkingCapital = receivables - payables;
console.log(`Net working capital is: ${netWorkingCapital}`);
```

### Catch Unclosed Parentheses, Brackets, Braces and Quotes
```js
let myArray = [1, 2, 3];
let arraySum = myArray.reduce((previous, current) =>  previous + current);
console.log(`Sum of array values is: ${arraySum}`);
```

### Catch Mixed Usage of Single and Double Quotes
```js
let innerHtml = "<p>Click here to <a href='#Home'>return home</a></p>";
console.log(innerHtml);
```

### Catch Use of Assignment Operator Instead of Equality Operator
```js
let x = 7;
let y = 9;
let result = "to come";

if(x == y) {
  result = "Equal!";
} else {
  result = "Not equal!";
}

console.log(result);
```

### Catch Missing Open and Closing Parenthesis After a Function Call
```js
function getNine() {
  let x = 6;
  let y = 3;
  return x + y;
}

let result = getNine();
console.log(result);
```