# ES2020
## MatchAll

The matchAll() method returns an iterator of all results matching a string against a regular expression, including capturing groups.

Example 1:

```js

const allMatched = "abcdefg".matchAll(/[a-c]/g);
for (let v of allMatched) {
  console.log(v);
}


// ['a', index: 0, input: 'abcdefg', groups: undefined]
// ['b', index: 1, input: 'abcdefg', groups: undefined]
// ['c', index: 2, input: 'abcdefg', groups: undefined]

```

Example 2:

```js
const regexp = /t(e)(st(\d?))/g;
const str = 'test1test2';

const array = [...str.matchAll(regexp)];

console.log(array[0]);
// expected output: Array ["test1", "e", "st1", "1"]

console.log(array[1]);
// expected output: Array ["test2", "e", "st2", "2"]


```

[see more](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/String/matchAll)