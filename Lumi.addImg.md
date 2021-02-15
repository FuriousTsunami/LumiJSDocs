<h1>Lumi.addImg()</h1>
<p>Method Description: Adds an image to the canvas</p>
<table>
  <thead>
    <tr>
      <th>Parameter</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>img</td>
      <td>The image to render</td>
    </tr>
    <tr>
      <td>x</td>
      <td>The X-Coordinate of the image</td>
    </tr>
    <tr>
      <td>y</td>
      <td>The Y-Coordinate of the image</td>
    </tr>
    <tr>
      <td>width</td>
      <td>The width of the image</td>
    </tr>
    <tr>
      <td>height</td>
      <td>The height of the image</td>
    </tr>
    <tr>
      <td>config</td>
      <td>(Optional) The settings for this image containing restitution (how much velocity and object will retain on impact), collision.collide (if it can be collided with), collision.affect (if it is affected by collisions), mass, and color.</td>
    </tr>
  </tbody>
</table>
<h2>Example</h2>
<pre><code class="language-JavaScript">
var img = document.createElement(&quot;IMG&quot;);
var rect = Lumi.addImage(img, 10, 50, 50, {
  color: red,
  mass: 0.3,
  restitution: 0.9,
  collision: {
    affect: true,
    collide: true,
  },
})
</code></pre>