# ES2020
## optional chaining operator 

The optional chaining operator (?.) enables you to read the value of a property located deep within a chain of connected objects without having to check that each reference in the chain is valid.

```js
user = {
  name: 'es11',
  power: 0
}
console.log(user.profile);
// expected output: undefined

console.log(user.profile.picture);
// expected output: error

// sol:
console.log(user && user.profile && user.profile.picture);
console.log(user?.profile?.picture);

```



Here are all of the use cases for optional chaining

```
obj?.prop       // optional static property access
obj?.[expr]     // optional dynamic property access
func?.(...args) // optional function or method call
```

[see more](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Operators/Optional_chaining)