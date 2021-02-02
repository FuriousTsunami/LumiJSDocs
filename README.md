<div class="text-align: center"><image src="Icon.png" width="150px" height="150px"></image></div>

# LumiJS


LumiJS was created for the purpose of having a simplistic yet useful game/physics engine. It is object-oriented JavaScript library that uses the HTML5 Canvas API, and has many components that you can add to it. It has the capabilities to power many 2d games and projects. Each component is re-usable, and can adapt to whatever you use them for. If you have any ideas for a new feature, please submit an "enhancement" issue on [GitHub](https://github.com/FuriousTsunami/LumiJS).

# Installation

To install LumiJS, all you have to do is import this [code](https://cdn.jsdelivr.net/gh/FuriousTsunami/LumiJS/Lumi.js) into your project.

> Note: The default LumiJS build contains helpful comments, but has a large size (19 KB). To optimize your project's size, use [this](https://cdn.jsdelivr.net/gh/FuriousTsunami/LumiJS/Lumi.min.js) build (8.96 KB).

After you have imported LumiJS, you're ready to start programming!

# Getting Started

Now that you're done installing LumiJS, we need to configure the engine with `Lumi.config()`. This function takes in a JSON object. The setup below sets the canvas width to 400px, the canvas height to 400px, and the camera view to top, or an overhead view. The full usage for this function can be found [here](/Lumi.config.md).

```JavaScript
Lumi.config({
  canvasWidth: 400,
  canvasHeight: 400,
  camera: {
    view: "top",
  },
});
```
