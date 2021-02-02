# Lumi.addImg()

Method Description: Adds an image to the canvas

| Parameter | Description                                                                                                                                                                                                                              |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| img       | The image to render                                                                                                                                                                                                                      |
| x         | The X-Coordinate of the image                                                                                                                                                                                                            |
| y         | The Y-Coordinate of the image                                                                                                                                                                                                            |
| width     | The width of the image                                                                                                                                                                                                                   |
| height    | The height of the image                                                                                                                                                                                                                  |
| config    | (Optional) The settings for this image containing restitution (how much velocity and object will retain on impact), collision.collide (if it can be collided with), collision.affect (if it is affected by collisions), mass, and color. |

## Example

```JavaScript
var img = document.createElement("IMG");
var rect = Lumi.addImage(img, 10, 50, 50, {
  color: red,
  mass: 0.3,
  restitution: 0.9,
  collision: {
    affect: true,
    collide: true,
  },
})
```