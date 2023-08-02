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

### Confirm the Ending
```js
function confirmEnding(str, target) {
  return str.slice(-target.length) === target
}

confirmEnding("Bastian", "n");
```

### Repeat a String Repeat a String
```js
function repeatStringNumTimes(str, num) {
  return num > 0 ? str + repeatStringNumTimes(str, num - 1) : '';
}

repeatStringNumTimes("abc", 3);
```

### Truncate a String
```js
function truncateString(str, num) {
  return str.length > num ? str.slice(0, num) + "..." : str;
}

let test = truncateString("A-tisket a-tasket A green and yellow basket", 8);

console.log(test);
```

### Finders Keepers
```js
function findElement(arr, func) {
  return arr.find(func);
}

findElement([1, 2, 3, 4], num => num % 2 === 0);
```

### Boo who
```js
function booWho(bool) {
  return (typeof bool == "boolean");
}

console.log(booWho(null));
```