<img src="https://sujeitoprogramador.com/wp-content/uploads/2019/08/jsjsjs.png" width="700px">
JavaScript - Tips and tricks

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
