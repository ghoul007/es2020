# ES2020
## Dynamic import

Dynamic imports in JavaScript give you the option to import JS files dynamically as modules in your application natively.  

```js

if (condition) {
  const calculator = import("./calculator.js");

  calculator.add(1, 2);
}


```

==> Dynamic Import will help you implement code splitting without Webpack or other module bundlers. 