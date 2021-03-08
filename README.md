# javascript
JavaScript - Tips and tricks


![](https://sujeitoprogramador.com/wp-content/uploads/2019/08/jsjsjs.png)

### Ways to Clone Objects in JavaScript
```
const food = { beef: '🌽', bacon: '🥓' };

Object.assign(food, { beef: '🥩' });
```

console.log(food);
// { beef: '🥩', bacon: '🥓' }
