
## Classes. Prototypes

* [Presentation](https://sulemanof.github.io/js-lectures/js-classes/presentation/#/)
* Practise


**Provide proto chaning**
```
let head = {
  glasses: 1
};

let table = {
  pen: 3
};

let bed = {
  sheet: 1,
  pillow: 2
};

let pockets = {
  money: 2000
};

pockets → bed → table → head
console.log( pockets.pen ); // 3
console.log( bed.glasses ); // 1
console.log( table.money ); // undefined
```

**Write full inheritance for BMW**
```
function Car(color, price) {
  this.color = color
  this.price = price
}

Car.prototype.getInfo = function() {
  return `${this.color} ${this.price}`
}

function BMW() {}

const myBmw = new BMW('bmw', 'black', 1000)

myBmw.getInfo() // bmw: black 1000

```

**Write following function**
```
function Human(name) {
  this.name = name

  // your code here
}

Human.prototype.getName = function() {
  console.log(this.name)
}

const bob = Human('bob')
const jack = new Human('jack')

bob.getName() // 'bob'
jack.getName() // 'jack'

bob instanceof Human // true
jack instanceof Human // true
```

**Create object based on existing object**
```
console.log(obj) // { }
const obj2 = ?
```


**Write reduce method**

```
[1,2,3,4,5].reduce(function(acc, next) {
  return acc + next
}, 0) // 1 + 2 + 3 + 4 + 5 = 15
```

**When we feed one hamster, the other one is also full. Why? How can we fix it?**
```
let hamster = {
  stomach: [],

  eat(food) {
    this.stomach.push(food);
  }
};

let speedy = {
  __proto__: hamster
};

let lazy = {
  __proto__: hamster
};

// This one found the food
speedy.eat("apple");
console.log( speedy.stomach ); // apple

// This one also has it, why? fix please.
console.log( lazy.stomach ); // apple
```

**Borrow method**
```
let obj = {
  0: "Hello",
  1: "world!",
  length: 2,
};

console.og( obj.join(',') ); // Hello,world!
```

**Bind polyfill**
```
const obj = { name: 'alex' }

function getName(surname) {
  console.log(this.name + ' ' + surname)
}

const getFullName = getName.bind(obj) 

getFullName('astafyeu') // alex astafyeu

```


## Hometask
* Clone your **TMS-your-name** repository
* create a branch **js-classes** in your project and checkout it
* create a folder **js-classes**, do your work inside this folder
* Do the task below
* Push branch and open Pull Request

## Task
### Use ES5 syntax
+ create a file `inheritance-es5.js`
+ create a class `Car` : this function should accept 7 params:  
    + name
    + model
    + year
    + color
    + maxSpeed
    + fuelCapacity - optional parameter, use `60` by default
    + fuelConsumption - optional parameter, use `10` by default
+ implement a common car method `getFullName`, which should return a full name (e.x. name + model)
+ implement a common car method `getAge`, which should return your car age (current year - your car year)
+ implement a common car method `changeColor`, which should do:
    - take a parameter (color);
    - if your car already has the same color, show a message with text (up to you);
    - if not, change the color and show a message about it.
+ implement a common car method `calculateWay`, which should do:
    - take 2 params: `kilometers` and `fuel`;
    - check if `fuel` < 10, show a message about refuel;
    - calculate the time that you need to reach the destination, show message about it;
    - check, if you need to refuel on your road and show a message (how many times you need to refuel)
+ create 3 another class, which should inherit from `Car` class in ES5 way (e.x. `BMW`, `Lexus`, etc. <--- up to you)
+ create class properties, which should refers only to that particular car factory, and should not effect others(
    for example all BMW's would have sunroof, all Lexus's would have climateControl and so on (all properties is up 
    to you)
)
+ create methods, which should refers only to that particular car factory, and should not effect others
+ create at least one instance of each class
+ check your solution in browser console (include your js file in any html)
---
### implement inheritance in ES6 way (use the `class` keyword)
Use ES6 syntax only (`let`, `const`, `arrow functions` and so on)
+ create a file `inheritance-es6.js`
+ do the same steps as in ES5 mode, but in ES6 syntax (use the `extends` and `super` keywords for inheritance)



