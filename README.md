# javascript
JavaScript - Tips and tricks


![](https://sujeitoprogramador.com/wp-content/uploads/2019/08/jsjsjs.png)
<img src="https://sujeitoprogramador.com/wp-content/uploads/2019/08/jsjsjs.png" width="700px">

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
