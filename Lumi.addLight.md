<h1>Lumi.addLight()</h1>
<p>Method Description: Adds a light to the canvas</p>
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
      <td>The X-Coordinate of the light</td>
    </tr>
    <tr>
      <td>y</td>
      <td>The Y-Coordinate of the light</td>
    </tr>
    <tr>
      <td>radius</td>
      <td>The radius of the light</td>
    </tr>
    <tr>
      <td>config</td>
      <td>(Optional) The settings for this light containing restitution (how much velocity and object will retain on impact), collision.collide (if it can be collided with), collision.affect (if it is affected by collisions), mass, and color.</td>
    </tr>
  </tbody>
</table>
<h2>Example</h2>
<pre><code class="language-JavaScript">
var light = Lumi.addLight(10, 10, 50, {
  color: red,
  mass: 0.3,
  restitution: 0.9,
  collision: {
    affect: true,
    collide: true,
  },
})
</code></pre>