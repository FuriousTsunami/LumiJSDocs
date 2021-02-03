# Introduction
LumiJS is an opensource library under the [MIT](https://opensource.org/licenses/MIT) license.
It was created for the purpose of having a simplistic yet useful game/physics engine. It is object-oriented JavaScript library that uses the HTML5 Canvas API, and has many components that you can add to it. It has the capabilities to power many 2d games and projects. Each component is re-usable, and can adapt to whatever you use them for. If you have any ideas for a new feature, please submit an "enhancement" issue on [GitHub](https://github.com/FuriousTsunami/LumiJS).

# Getting Started

To install LumiJS, all you have to do is import this [code](https://cdn.jsdelivr.net/gh/FuriousTsunami/LumiJS/Lumi.js) into your project.

> Note: The default LumiJS build contains helpful comments, but has a large size (19 KB). To optimize your project's size, use [this](https://cdn.jsdelivr.net/gh/FuriousTsunami/LumiJS/Lumi.min.js) build (8.96 KB).

After you have imported LumiJS, you're ready to start programming!

## Configuring engine

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

OK, we have finished setting up the LumiJS engine. Now, all we need to do is start it! This is as simple as running `Lumi.init()`.

```JavaScript
Lumi.init();
```

## Adding a Square

In the background, LumiJS has just started the animation loop to render entities. Let's try adding a square to the canvas.

```JavaScript
var rect = Lumi.addRect(10, 10, 50, 50);
```
We used the `Lumi.addRect` function to add one to the canvas. There are also 3 more entities, namely `Lumi.addEllipse`, `Lumi.addImg`, and `Lumi.addLight`.

The parameters for a `Lumi.rect` are in this order: `x`, `y`, `width`, `height`. You can find all the other entities and functions in the "Methods" section on the left of this page. Anyways, now you might be wondering, why did we store the rectangle entity it in a variable? Well, storing it inside a variable allows us to dynamically manupulate the rectangle we just created. For example:

```JavaScript
rect.addXVel(1);
```

This will add an X Velocity to the rectangle we just created at a 1px/frame speed.

## Exploring "config" property

I know that earlier I said there are 4 parameters in a `Lumi.rect` are `x`, `y`, `width`, and `height`. But what if you wanted more customization? Well, there is actually a fifth optional parameter called `config`. This time, let's create a `Lumi.ellipse` and add the `config` parameter to it:

```JavaScript
var someCircle = Lumi.addEllipse(10, 10, 50, {
  color: "green",
  mass: 0.4,
  restitution: 0.1,
});
```

The reason that  `someCircle` doesn't have 5 parameters is because a circle only has a radius, not a width and a height. Anyways, let's take a look at the ``config`` object we put in there. As you probably guessed, the `color` property indicates the color of the object. The `mass` property won't affect our code right now, because the camera's view is from the top, which means no gravity. The `restitution` property indicates how much an object should retain its velocity upon impact. For example, if there was an object coming with `10` velocity at `someCircle`, than when it bounced back off the circle, its velocity would be `1`, because `0.1 * 10 = 1`. 

There are also another object inside `config` called `collision`. It controls whether it can even collide with things, or if it is affected by the collision. Sometimes, this is helpful if you want objects to be moving in the "background" of your scene. Let's try adding it to `someCircle`

```JavaScript
var someCircle = Lumi.addEllipse(10, 10, 50, {
  color: "green",
  mass: 0.4,
  restitution: 0.1,
  collision: {
    collide: true,
    affect: false,
  },
});
```

What we just put above tells the physics engine that `someCircle` should be able to collide with things, but not be affected by the collision.

## Conclusion

Well, that's all for the tutorial! To continue learning about LumiJS, and how it works, you can read the methods on this documentation (left side of the page)! Or, to explore the actual source code, you could visit the [GitHub](https://github.com/FuriousTsunami).

### License

LumiJS is licensed under [The MIT License (MIT)](https://opensource.org/licenses/MIT)  
Copyright (c) 2020 Sunay Komarla