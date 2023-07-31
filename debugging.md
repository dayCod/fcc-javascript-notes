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