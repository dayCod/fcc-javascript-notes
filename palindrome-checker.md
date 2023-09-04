### Palindrome Checker
```js
function palindrome(str) {
  var sentence = str.replace(/[\W_]/g, '');
  for(var i = 0, count = sentence.length - 1; i < count/2; i++) {
    if(sentence[i].toLowerCase() !== sentence[count-i].toLowerCase()) {
      return false;
    }
  }
  return true;
};

palindrome("eye");
```