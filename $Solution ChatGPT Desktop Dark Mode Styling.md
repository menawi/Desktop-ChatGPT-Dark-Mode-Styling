
```js
function injectCSS(css) {
  let style = document.createElement('style');
  style.type = 'text/css';
  style.appendChild(document.createTextNode(css));
  document.head.appendChild(style);
}

const cssSnippet = `
div {
    background-image: linear-gradient(to bottom, black, black) !important; 
    background-color: black !important;
}

button {
    background-color: black !important;  
}

a {
    background-color: black !important;
}

h3 {
    background-color: black !important;
}

#chatgpt-app-window-top {
    background-color: black !important;
    background-image: black !important;
}
`;

injectCSS(cssSnippet);
```