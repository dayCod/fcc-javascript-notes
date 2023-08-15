### Create a Basic JavaScript Object
```js
let dog = {
  name: "You",
  numLegs: 4
};
```

### Use Dot Notation to Access the Properties of an Object
```js
let dog = {
  name: "Spot",
  numLegs: 4
};
// Only change code below this line
console.log('Dog Name:'+dog.name, 'Num of Legs:'+dog.numLegs)
```

### Create a Method on an Object
```js
let dog = {
  name: "Spot",
  numLegs: 4,
  sayLegs: function () {
    return "This dog has " + dog.numLegs + " legs.";
  }
};

console.log(dog.sayLegs());
```

### Make Code More Reusable with the this Keyword
```js
let dog = {
  name: "Spot",
  numLegs: 4,
  sayLegs: function() {return "This dog has " + this.numLegs + " legs.";}
};

dog.sayLegs();
```

### Define a Constructor Function
```js
function Dog() {
  this.name = '';
  this.color = '';
  this.numLegs = 4;
}
```

### Use a Constructor to Create Objects
```js
function Dog() {
  this.name = "Rupert";
  this.color = "brown";
  this.numLegs = 4;
}
// Only change code below this line
let hound = new Dog();
```

### Extend Constructors to Receive Arguments
```js
function Dog(name, color) {
  this.name = name;
  this.color = color;
  this.numLegs = 4;
}

let terrier = new Dog('You', 'Grey');
```

### Verify an Object's Constructor with instanceof
```js
function House(numBedrooms) {
  this.numBedrooms = numBedrooms;
}
let myHouse = new House(4);
console.log(myHouse instanceof House);
```

### Understand Own Properties
```js
function Bird(name) {
  this.name = name;
  this.numLegs = 2;
}

let canary = new Bird("Tweety");
let ownProps = [];
for (let property in canary) {
  if (canary.hasOwnProperty(property)) {
    ownProps.push(property);
  }
}
```