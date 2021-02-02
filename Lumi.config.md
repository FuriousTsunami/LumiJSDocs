# Lumi.config()

Method Description: Configures variables to run the Engine and Renderer

| Parameter | Description                                                                                                                                                                                                                                             |
| --------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| config    | A JSON object containing all the configurations for the LumiJS engine, such as canvasWidth (can be "fitToWindow"), canvasHeight (can be "fitToWindow"), and camera (contains "view", which indicates the view of the camera and can be "top" or "side") |

## Example

```JavaScript
Lumi.config({
  canvasWidth: 400,
  canvasHeight: 400,
  camera: {
    view: "top",
  },
});
```