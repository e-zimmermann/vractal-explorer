<h2>Installation</h2>
<ol>
  <li>Download or clone repository.</li>
  <li>Use for instance <a href="https://docs.npmjs.com/downloading-and-installing-node-js-and-npm">npm</a> to run local webserver. After installation of Nodejs / npm open folder with downloaded files in terminal and write
<code>npm install</code>. </li>
  <li>Afterwards use <code>npm run dev</code> in terminal and access webpage via shown url.</li>
</ol>

<h2>Instruction Manual</h2>
<ol>
  <li>Using key <code>y</code> on the keyboard toggles the settings display.</li>
  <li>A small icon on the bottom right corner allows to switch to VR mode (either using an HMD like the Meta Quest and running the local webserver on the device or by using the WebXR browser plugin, which allows to emulate an HMD). In the VR mode the controller button <code>y</code> toggles the settings display.</li>
  <li>The slider <i>mult</i> controls the iteration schemes. There are three schemes available.</li>
  <li>The slider <i>f, g</i> controls the function pair choices. The last option allows to define own functions f and g which get evaluated when selecting <i>Apply</i>.</li>
  <li>The parameter <i>#iterations</i> controls the number of iterations used to determine whether a point belongs to the object or not. The parameter ranges from 0 up to 100.</li>
  <li>The parameter <i>eps</i> controls the initial step size for the raymarching. The parameter ranges from 1.e-5 up to 1.e-2.</li>
  <li>The parameter <i>radius</i> controls the sphere radius. All objects are rendered inside the sphere centered at the origin. The radius is also used for the membership test of a point. The parameter ranges from 0 up to 10.</li>
  <li>The parameter <i>Julia constant</i> provides the option to provide a constant which is used in the iteration scheme 3 called <i>f x g + const</i>.</li>
</ol>

<h2>Bug</h2>
<ol>
  <li>Currently there is a bug when selecting a function pair f, g from the second slider on the left panel. Then the shader does not compile reliably with the respective code snippet. A current workaround is to manually set the desired pair in the file main.js in the variable <code>const initialFunctionPairChoice;</code>.</li>
</ol>
