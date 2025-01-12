# react-without-nodejs-example
https://pulgasari.github.io/react-without-nodejs-example/

## Get started

index.html file
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>React without NodeJS Example</title>
</head>
<body>
  <div id="app"></div>
  <script src="https://unpkg.com/@babel/standalone/babel.min.js"></script>
  <script type="text/babel" data-type="module" src="app.js"></script>
</body>
</html>
```

app.js file
```js
import React from "https://esm.sh/react@19/?dev"
import ReactDOMClient from "https://esm.sh/react-dom@19/client?dev"

var Header = <div id='Header'>... Header ...</div>;
var MainArea = <div id='MainArea'>... MainArea ...</div>;

// RENDER IT
var rootElement = <div id='root'><Header/><MainArea/></div>;
ReactDOMClient.createRoot( 
  document.getElementById('app') 
).render(rootElement);
```
