# GameCraftJS 🎮

Lightweight JavaScript game-making library built on the HTML5 Canvas. It abstracts the boring boilerplate (game loop, input handling, timing) so you can focus on gameplay.

[![License](https://img.shields.io/badge/License-BSD_2--Clause-blue.svg)](https://opensource.org/licenses/BSD-2-Clause)
[![GitHub - sunbyte16](https://img.shields.io/badge/GitHub-@sunbyte16-181717?logo=github)](https://github.com/sunbyte16)
[![LinkedIn - Sunil Sharma](https://img.shields.io/badge/LinkedIn-Sunil%20Sharma-0A66C2?logo=linkedin)](https://www.linkedin.com/in/sunil-kumar-bb88bb31a/)
[![Portfolio](https://img.shields.io/badge/Portfolio-Visit-success?logo=vercel)](https://lively-dodol-cc397c.netlify.app)

### ✨ Features
- ⚡ Minimal, fast game loop with configurable FPS
- 🎯 Simple lifecycle hooks: `myinit`, `update`, `draw`
- ⌨️ Keyboard input helpers
- 🖱️ Mouse click handling with coordinates
- 🧰 Zero-dependency, drop-in script for any HTML page

## 🚀 Quick Start
Include a canvas and initialize the engine on page load:

```html
<body onload="NPGinit(50)">
  <canvas id="NPGcanvas" width="500" height="500">Your browser does not support Canvas.</canvas>
</body>
```

## 🛠️ Usage
Implement the core lifecycle and input handlers:

```javascript
// executes once in the beginning
function myinit() { }

// executes every tick, FPS (typically around 30–50) times a second
function update() { }

// executes every tick right after update()
function draw() {
    ctx.clearRect(0, 0, WIDTH, HEIGHT);
}

// event function when a click occurs. x, y coordinates of click are given
function mouseClick(x, y) { }

// events for key up and down. key value is passed in.
function keyUp(key) { }
function keyDown(key) { }
```

The engine binds to a canvas with id `NPGcanvas` and exposes a few globals for convenience:

```javascript
var canvas;
var ctx;
var WIDTH;
var HEIGHT;
var FPS;
```

Check the `demos/` folder for examples of drawing and input.

## 📁 Project Structure
- `demos/` – Example games and snippets
- `include/` – Library source files
- `starter.html` – Minimal example to get started

## 🤝 Contributing
Issues and pull requests are welcome. If you find a bug or have a feature idea, feel free to open an issue or PR.

## 📜 License
BSD 2-Clause License. See header notices in the source files for details.

## 🙏 Acknowledgements
Originally authored by Andrej Karpathy (2012). This version is maintained and documented for ease of use.

---

Created By [❤️Sunil Sharma❤️](https://www.linkedin.com/in/sunil-kumar-bb88bb31a/) · 
 [![GitHub - @sunbyte16](https://img.shields.io/badge/GitHub-@sunbyte16-181717?logo=github)](https://github.com/sunbyte16) ·
 [![Portfolio](https://img.shields.io/badge/Portfolio-lively--dodol--cc397c.netlify.app-success?logo=vercel)](https://lively-dodol-cc397c.netlify.app)
