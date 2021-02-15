<h1>Lumi.config()</h1>
<p>Method Description: Configures variables to run the Engine and Renderer</p>
<table>
  <thead>
    <tr>
      <th>Parameter</th>
      <th>Description</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>config</td>
      <td>A JSON object containing all the configurations for the LumiJS engine, such as canvas (contains &quot;width&quot; and &quot;height&quot;, which indicate the canvas width and height. Can be fitToWindow), camera (contains &quot;view&quot;, which indicates the view of the camera and can be &quot;top&quot; or &quot;side&quot;), and gravity (the amount of gravity for the engine))</td>
    </tr>
  </tbody>
</table>
<h2>Example</h2>
<pre><code class="language-JavaScript">
Lumi.config({
  canvas: {
    width: &quot;fitToWindow&quot;,
    height: &quot;fitToWindow&quot;,
  },
  camera: {
    view: &quot;side&quot;,
  },
  gravity: 1,
});
</code></pre>