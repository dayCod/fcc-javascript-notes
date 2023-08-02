### Convert Celsius to Fahrenheit
```js
function convertCtoF(celsius) {
  let fahrenheit = (celsius * (9/5)) + 32;
  return fahrenheit;
}

convertCtoF(30);
```

### Reverse a String
```js
function reverseString(str) {
  return str.split("").reverse().join("");
}

reverseString("hello");
```