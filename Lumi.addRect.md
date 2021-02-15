<h1>Lumi.addRect()</h1>
<p>Method Description: Adds a rectangle to the canvas</p>
<table>
  <thead>
    <tr>
      <th>Parameter</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>x</td>
      <td>The X-Coordinate of the rectangle</td>
    </tr>
    <tr>
      <td>y</td>
      <td>The Y-Coordinate of the rectangle</td>
    </tr>
    <tr>
      <td>width</td>
      <td>The width of the rectangle</td>
    </tr>
    <tr>
      <td>height</td>
      <td>The height of the rectangle</td>
    </tr>
    <tr>
      <td>config</td>
      <td>(Optional) The settings for this rectangle containing restitution (how much velocity and object will retain on impact), collision.collide (if it can be collided with), collision.affect (if it is affected by collisions), mass, and color.</td>
    </tr>
  </tbody>
</table>
<h2>Example</h2>
<pre><code class="language-JavaScript">
var rect = Lumi.addRect(10, 10, 50, 50, {
  color: red,
  mass: 0.3,
  restitution: 0.9,
  collision: {
    affect: true,
    collide: true,
  },
})
</code></pre>