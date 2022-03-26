# ES2020
## GlobalThis

After ES2020, globalThisyou can get the global scope of the current execution environment as long as you use it in Javascript 

```js
button.addEventListener("click", function () {
    console.log(this); // button
    console.log(globalThis); // window
});

// in web worker
globalThis === self; // true
globalThis === window; // true

// in node.js
globalThis === global; // true

// in browser
globalThis === window; // true
```
[see more](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/globalThis)