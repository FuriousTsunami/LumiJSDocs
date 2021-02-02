# Lumi.addRect()

Method Description: Adds a rectangle to the canvas

| Parameter | Description                                                                                                                                                                                                                                  |
| --------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| x         | The X-Coordinate of the rectangle                                                                                                                                                                                                            |
| y         | The Y-Coordinate of the rectangle                                                                                                                                                                                                            |
| width     | The width of the rectangle                                                                                                                                                                                                                   |
| height    | The height of the rectangle                                                                                                                                                                                                                  |
| config    | (Optional) The settings for this rectangle containing restitution (how much velocity and object will retain on impact), collision.collide (if it can be collided with), collision.affect (if it is affected by collisions), mass, and color. |

## Example

```JavaScript
var rect = Lumi.addRect(10, 10, 50, 50, {
  color: red,
  mass: 0.3,
  restitution: 0.9,
  collision: {
    affect: true,
    collide: true,
  },
})
```