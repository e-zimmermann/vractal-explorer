<h2>Installation</h2>
<ol>
  <li>Download files from git repository.</li>
  <li>Use <a href="https://docs.npmjs.com/downloading-and-installing-node-js-and-npm">npm</a> to install and run local webserver. After installation of Nodejs / npm open folder with downloaded files in terminal and write
<code>npm install</code>. </li>
  <li>Afterwards use <code>npm run dev</code> in terminal and access webpage via shown url.</li>
</ol>

<h2>Instruction Manual</h2>
<ol>
  <li>Using key <code>y</code> on the keyboard toggles the settings display.</li>
  <li>The slider "mult" controls the iteration schemes.</li>
  <li>The slider "f, g" controls the function pair choices. The last option allows to define own functions f and g which get evaluated when hitting "Apply".</li>
  <li>The parameter "#iterations" controls the number of iterations used to determine whether a point belongs to the object or not. The parameter ranges from 0 up to 100.</li>
  <li>The parameter "eps" controls the initial step size for the raymarching. The parameter ranges from 1.e-5 up to 1.e-2.</li>
  <li>The parameter "radius" controls the sphere radius. All objects are rendered inside the sphere centered at the origin of this radius. The radius is also used for the membership test of a point. The parameter ranges from 0 up to 10.</li>
  <li>The parameter "Julia constant" provides the option for a constant used in the iteration scheme 3 called "f x g + const".</li>
</ol>

<h2>Bug</h2>
<ol>
  <li>Currently there is a bug when selecting a function pair f, g from the second slider on the left panel. Then the shader does not compile with the respective code snippet. A current workaround is to manually set the desired pair in the file main.js in the varible <code>const initialFunctionPairChoice;</code>.</li>
</ol>
