# Lumi.config()

Method Description: Configures variables to run the Engine and Renderer

| Parameter | Description                                                                                                                                                                                                                                             |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| config    |A JSON object containing all the configurations for the LumiJS engine, such as canvas (contains "width" and "height", which indicate the canvas width and height. Can be fitToWindow), camera (contains "view", which indicates the view of the camera and can be "top" or "side"), and gravity (the amount of gravity for the engine)) |

## Example

```JavaScript
Lumi.config({
  canvas: {
    width: "fitToWindow",
    height: "fitToWindow",
  },
  camera: {
    view: "side",
  },
  gravity: 1,
});
```