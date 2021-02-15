<h1>Lumi.checkCollision()</h1>
<p>Method Description: Checks if two objects are colliding</p>
<table>
  <thead>
    <tr>
      <th>Parameter</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>obj1</td>
      <td>The first collision object</td>
    </tr>
    <tr>
      <td>obj2</td>
      <td>The second collision object</td>
    </tr>
  </tbody>
</table>
<h2>Example</h2>
<pre><code class="language-JavaScript">
var obj1 = Lumi.addRect(10, 10, 50, 50);
var obj2 = Lumi.addRect(100, 100, 50, 50);
if (Lumi.checkCollision(obj1, obj2)) {
  console.log(&quot;Collision Detected!&quot;);
} else {
  console.log(&quot;No Collision.&quot;);
}
</code></pre>