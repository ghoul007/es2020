# ES2020
## Nullish coalescing operator

The nullish coalescing operator (??) is a logical operator that returns its right-hand side operand when its left-hand side operand is null or undefined, and otherwise returns its left-hand side operand

```js
user = {
  name: 'es11',
  power: 0
}
power = user.power || 'no power'; // returns 'no power' - checks if value is 'false'
power = user.power ?? 'no power'; // returns 0 - checks if value is null/undefined
```
[see more](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Nullish_coalescing_operator)