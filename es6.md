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