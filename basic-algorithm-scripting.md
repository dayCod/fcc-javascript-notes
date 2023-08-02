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

### Factorialize a Number
```js
function factorialize(num) {
  if (num === 0) {
    return 1;
  } else {
    return num * factorialize(num - 1);
  }
}

factorialize(5);
```

### Find the Longest Word in a String
```js
function findLongestWordLength(str) {
    let longestLength = 0;
    let currentLength = 0;

    for (let i = 0; i < str.length; i++) {
      if (str[i] === " ") {
        if (currentLength > longestLength) {
          longestLength = currentLength;
        }
        currentLength = 0;
      } else {
        currentLength++;
      }
    }
    if (currentLength > longestLength) {
      longestLength = currentLength;
    }

    return longestLength;
}

let tes = findLongestWordLength("The quick brown fox jumped over the lazy dog");

console.log(tes);
```

### Return Largest Numbers in Arrays
```js
function largestOfFour(arr) {
  return arr.map(function(group) {
    return group.reduce(function(prev, current) {
      return current > prev ? current : prev;
    });
  });
}

largestOfFour([[4, 5, 1, 3], [13, 27, 18, 26], [32, 35, 37, 39], [1000, 1001, 857, 1]]);
```