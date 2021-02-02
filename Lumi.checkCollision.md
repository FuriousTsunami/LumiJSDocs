# Lumi.checkCollision()

Method Description: Checks if two objects are colliding

| Parameter | Description                 |
| --------- | --------------------------- |
| obj1      | The first collision object  |
| obj2      | The second collision object |

## Example

```JavaScript
var obj1 = Lumi.addRect(10, 10, 50, 50);
var obj2 = Lumi.addRect(100, 100, 50, 50);
if (Lumi.checkCollision(obj1, obj2)) {
  console.log("Collision Detected!");
} else {
  console.log("No Collision.");
}
```