# Lumi.addLight()

Method Description: Adds a light to the canvas

| Parameter | Description                                                                                                                                                                                                                              |
| --------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| x         | The X-Coordinate of the light                                                                                                                                                                                                            |
| y         | The Y-Coordinate of the light                                                                                                                                                                                                            |
| radius    | The radius of the light                                                                                                                                                                                                                  |
| config    | (Optional) The settings for this light containing restitution (how much velocity and object will retain on impact), collision.collide (if it can be collided with), collision.affect (if it is affected by collisions), mass, and color. |

## Example

```JavaScript
var light = Lumi.addLight(10, 10, 50, {
  color: red,
  mass: 0.3,
  restitution: 0.9,
  collision: {
    affect: true,
    collide: true,
  },
})
```