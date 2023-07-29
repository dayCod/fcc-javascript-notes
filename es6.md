### Compare Scopes of the var and let Keywords
```js
function checkScope() {
  let i = 'function scope';
  if (false) {
    i = 'block scope';
    console.log('Block scope i is: ', i);
  }
  console.log('Function scope i is: ', i);
  return i;
}
```

### Mutate an Array Declared with const
```js
const s = [5, 7, 2];
function editInPlace(s) {
  // Only change code below this line
  s[0] = 2;
  s[1] = 5;
  s[2] = 7;

  return s;
  // Using s = [2, 5, 7] would be invalid

  // Only change code above this line
}

console.log(editInPlace(s));
```

### Prevent Object Mutation
```js
function freezeObj() {
  const MATH_CONSTANTS = {
    PI: 3.14
  };
  // Only change code below this line
  Object.freeze(MATH_CONSTANTS);

  // Only change code above this line
  try {
    MATH_CONSTANTS.PI = 99;
  } catch(ex) {
    console.log(ex);
  }
  return MATH_CONSTANTS.PI;
}
const PI = freezeObj();
```

### Use Arrow Functions to Write Concise Anonymous Functions
```js
const magic = () => {return new Date()};
```

### Write Arrow Functions with Parameters
```js
const myConcat = (arr1, arr2) => {
  return arr1.concat(arr2);
}

console.log(myConcat([1, 2], [3, 4, 5]));
```

### Set Default Parameters for Your Functions
```js
// Only change code below this line
const increment = (number, value = 1) => number + value;
// Only change code above this line
```

### Use the Rest Parameter with Function Parameters
```js
const sum = (...args) => {
  let total = 0;
  for (let i = 0; i < args.length; i++) {
    total += args[i];
  }
  return total;
}

console.log(sum(1, 2, 3, 4));
```

### Use the Spread Operator to Evaluate Arrays In-Place
```js
const arr1 = ['JAN', 'FEB', 'MAR', 'APR', 'MAY'];
let arr2;

arr2 = [...arr1];  // Change this line

console.log(arr2);
```