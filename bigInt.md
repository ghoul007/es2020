# ES2020
## BigInt

is a new javascript type, we can use to make calculations which are bigger than Number.MAX_SAFE_INTEGER

```js

const max =  Number.MAX_SAFE_INTEGER // 9007199254740991
// ~ Math.pow(2.53)-1

// We lost precision, look at the values, same when we add 1 and when we add 2
console.log(max +1); // 9007199254740992
console.log(max +2);// 9007199254740992


// With BigInt we have precision (note to use "n")
console.log(BigInt(max) + 1n); // 9007199254740992n
console.log(BigInt(max) + 2n); // 9007199254740993n


```

 

[see more](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/BigInt)