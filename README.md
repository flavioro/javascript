<img src="https://sujeitoprogramador.com/wp-content/uploads/2019/08/jsjsjs.png" width="700px">
JavaScript - Tips and tricks


### module.exports vs export default
```
module.exports = 1
module.exports = NaN
module.exports = 'foo'
module.exports = { foo: 'bar' }
module.exports = [ 'foo', 'bar' ]
module.exports = function foo () {}
module.exports = () => {}
```
Export padrão
```
export default = 1
export default = NaN
export default = 'foo'
export default = { foo: 'bar' }
export default = [ 'foo', 'bar' ]
export default = function foo () {}
export default = () => {}
```
 
### count the number of keys/properties of an object in JavaScript###
 ``` 
var obj = { name: "John", age: 30, city: "New York" };
Object.keys(obj).length //
 ``` 
 
 
 ** JSON.stringify() ** 
   ``` 
 var obj = { name: "John", age: 30, city: "New York" };
var myJSON = JSON.stringify(obj);
RESULT: {"name":"John","age":30,"city":"New York"}
 ``` 
 
 ** JSON.parse() **
 ``` 
 const json = '{"result":true, "count":42}';
const obj = JSON.parse(json);

console.log(obj.count);
// expected output: 42

console.log(obj.result);
// expected output: true
 ``` 


### Array splice (remove, insert and replace)
```js
const months = ['Jan', 'March', 'April', 'June'];
months.splice(1, 0, 'Feb');
// inserts at index 1
console.log(months);
// expected output: Array ["Jan", "Feb", "March", "April", "June"]

months.splice(4, 1, 'May');
// replaces 1 element at index 4
console.log(months);
// expected output: Array ["Jan", "Feb", "March", "April", "May"]

// Remove after March
months.splice(3, 2);
```

### Array Find
```js
const array1 = [5, 12, 8, 130, 44];

const found = array1.find(element => element > 10);

console.log(found);
// expected output: 12
```

### Push Array
```js
const animals = ['pigs', 'goats', 'sheep'];

const count = animals.push('cows');
```
Other examples to splice, pop
https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Array

### Remove Property from an Object
```
var person = {
  firstName:"John",
  lastName:"Doe",
  age:50,
  eyeColor:"blue"
};

delete person.age;  // or delete person["age"];
```

### Ways to Clone Objects in JavaScript (object.assign vs spread operator)
```
const food = { beef: '🌽', bacon: '🥓' };

Object.assign(food, { beef: '🥩' });
```

console.log(food);
// { beef: '🥩', bacon: '🥓' }

```
const food = { beef: '🌽', bacon: '🥓' };

const newFood = {
  ...food,
  beef: '🥩',
}
```

console.log(newFood);
// { beef: '🥩', bacon: '🥓' }
