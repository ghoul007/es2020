# ES2020
## AllSettled

The ```Promise.allSettled()``` method returns a promise that resolves after all of the given promises have either fulfilled or rejected, with an array of objects that each describes the outcome of each promise.

```js
const p1 = Promise.resolve(3);
const p2 = new Promise((resolve, reject) => setTimeout(reject, 1000, 'foo'));
const promises = [p1, p2];

Promise.all(promises).then(data => console.log(data))
 .catch((rejection) => console.log(`Promise all catch: ${rejection}`));
  // throws error since it expects all promises to be resolved

Promise.allSettled(promises).
  then((results) => results.forEach((result) => console.log(`Promise allSettled: ${result.status}`)));// all good
```
[see more](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Promise/allSettled)