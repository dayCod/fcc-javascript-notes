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

### Use Prototype Properties to Reduce Duplicate Code
```js
function Dog(name) {
  this.name = name;
}

Dog.prototype.numLegs = 4;

let beagle = new Dog("Snoopy");
```

### Iterate Over All Properties
```js
function Dog(name) {
  this.name = name;
}

Dog.prototype.numLegs = 4;

let beagle = new Dog("Snoopy");

let ownProps = [];
let prototypeProps = [];

for (let property in beagle) {
  if (beagle.hasOwnProperty(property)) {
    ownProps.push(property);
  } else {
    prototypeProps.push(property);
  }
}
```

### Understand the Constructor Property
```js
function Dog(name) {
  this.name = name;
}

function joinDogFraternity(candidate) {
  if (candidate.constructor === Dog) {
    return true;
  } else {
    return false;
  }
}
```

### Change the Prototype to a New Object
```js
function Dog(name) {
  this.name = name;
}

Dog.prototype = {
  // Only change code below this line
  numLegs: 4,
  eat: function () {

  },
  describe: function () {
    
  }
};
```

### Remember to Set the Constructor Property when Changing the Prototype
```js
function Dog(name) {
  this.name = name;
}

// Only change code below this line
Dog.prototype = {
  constructor: Dog,
  numLegs: 4,
  eat: function() {
    console.log("nom nom nom");
  },
  describe: function() {
    console.log("My name is " + this.name);
  }
};
```

### Understand Where an Object’s Prototype Comes From
```js
function Dog(name) {
  this.name = name;
}

let beagle = new Dog("Snoopy");

// Only change code below this line
console.log(Dog.prototype.isPrototypeOf(beagle));
```

### Understand the Prototype Chain
```js
function Dog(name) {
  this.name = name;
}

let beagle = new Dog("Snoopy");

Dog.prototype.isPrototypeOf(beagle);  // yields true

// Fix the code below so that it evaluates to true
Object.prototype.isPrototypeOf(Dog.prototype);
```

### Use Inheritance So You Don't Repeat Yourself
```js
function Cat(name) {
  this.name = name;
}

Cat.prototype = {
  constructor: Cat
};

function Bear(name) {
  this.name = name;
}

Bear.prototype = {
  constructor: Bear
};

function Animal() {}

Animal.prototype = {
  constructor: Animal,
  eat: function() {
    console.log("nom nom nom");
  }
};
```

### Inherit Behaviors from a Supertype
```js
function Animal() { }

Animal.prototype = {
  constructor: Animal,
  eat: function() {
    console.log("nom nom nom");
  }
};

// Only change code below this line

let duck = Object.create(Animal.prototype); // Change this line
let beagle = Object.create(Animal.prototype); // Change this line
```

### Set the Child's Prototype to an Instance of the Parent
```js
function Animal() { }

Animal.prototype = {
  constructor: Animal,
  eat: function() {
    console.log("nom nom nom");
  }
};

function Dog() { }

// Only change code below this line

Dog.prototype = Object.create(Animal.prototype);

let beagle = new Dog();
```

### Reset an Inherited Constructor Property
```js
function Animal() { }
function Bird() { }
function Dog() { }

Bird.prototype = Object.create(Animal.prototype);
Dog.prototype = Object.create(Animal.prototype);

// Only change code below this line
Bird.prototype.constructor = Bird;
Dog.prototype.constructor = Dog;

let duck = new Bird();
let beagle = new Dog();
```

### Reset an Inherited Constructor Property
```js
function Animal() {}
Animal.prototype.eat = function() {
  console.log("nom nom nom");
};

function Dog() {}

// Add your code below this line
Dog.prototype = Object.create(Animal.prototype);
Dog.prototype.constructor = Dog;
Dog.prototype.bark = function() {
  console.log("Woof!");
};
// Add your code above this line

let beagle = new Dog();

beagle.eat(); // Should print "nom nom nom"
beagle.bark(); // Should print "Woof!"
```

### Override Inherited Methods
```js
function Bird() { }

Bird.prototype.fly = function() { return "I am flying!"; };

function Penguin() { }
Penguin.prototype = Object.create(Bird.prototype);
Penguin.prototype.constructor = Penguin;

// Only change code below this line

Penguin.prototype.fly = function() {
  return "Alas, this is a flightless bird.";
};

// Only change code above this line

let penguin = new Penguin();
console.log(penguin.fly());
```

### Use a Mixin to Add Common Behavior Between Unrelated Objects
```js
let bird = {
  name: "Donald",
  numLegs: 2
};

let boat = {
  name: "Warrior",
  type: "race-boat"
};

// Add your code below this line
let glideMixin = function(obj) {
  obj.glide = function() {
    console.log("Gliding!");
  };
};
glideMixin(bird);
glideMixin(boat);
```