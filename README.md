# My Knowledge

This is just a latex project containing some of the stuff I have learned.

## Dark mode

A quick hack to turn the PDF into dark mode in a web browser

```js
const overlay = document.createElement("div");

const css = `
    position: fixed;
    pointer-events: none;
    top: 0;
    left: 0;
    width: 100vw;
    height: 100vh;
    background-color: white;
    mix-blend-mode: difference;
    z-index: 1;
`
overlay.setAttribute("style", css);
document.body.appendChild(overlay);
```