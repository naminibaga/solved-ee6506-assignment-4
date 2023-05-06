Download Link: https://assignmentchef.com/product/solved-ee6506-assignment-4
<br>



Consider a one-dimensional material and an electromagnetic wave travelling through it. We are interested in the reflection and transmission coefficients as a function of wavelength for two kinds of structures suspended in air.

One, is a periodic arrangement of the type (from left to right): <em>NANANANANANAN</em>, where <em>N </em>denotes a layer with refractive index 3.5, and <em>A </em>denotes a layer of air (note there are 7 layers of ‘N’).

The second structure is based on the Fibonacci sequence (<em>f</em><sub>1 </sub>= 0, <em>f</em><sub>2 </sub>= 1, <em>f<sub>n</sub></em><sub>+2 </sub>= <em>f<sub>n</sub></em><sub>+1</sub>+ <em>f<sub>n</sub></em>).

Let <em>f</em><sub>1 </sub>= <em>A</em>, <em>f</em><sub>2 </sub>= <em>N</em>, and interpret ‘+<sup>0 </sup>to be string addition. So, <em>f</em><sub>3 </sub>= <em>NA</em>, <em>f</em><sub>4 </sub>= <em>NAN</em>, <em>f</em><sub>5 </sub>= <em>NANNA</em>, and so on. Our structure corresponds to <em>f</em><sub>7 </sub>(compute this).

√

The length of <em>N </em>to <em>A </em>is the golden ratio <em>τ </em>= ( 5 + 1)/2. You may assume a plane wave source. Report the reflection and transmission spectra for some range <em>λ</em><sub>0 </sub>± 0.5<em>λ</em><sub>0 </sub>that captures the interesting physics of the problem in both cases. How do you arrive at this ”interesting” range? Hint: You can solve the first case exactly without FEM. Or solve the first case and vary the wavelength w.r.t. thickness of <em>A </em>till you see some resonant phenomena in the reflection/transmission, and maintain the same thickness for the second case. Be sure to include some air gap between the boundaries and the structure. Prepare a comprehensive report outlining how you arrived at each design parameter, along with the results and the code in the appendix. Remember to include some validation result that shows your code to be working. Plan the entire exercise before beginning to code.

[Trivia: Such a structure has recently been used in fabricating quantum well structures:

<a href="https://link.aps.org/doi/10.1103/PhysRevB.77.113306">http://link.aps.org/doi/10.1103/PhysRevB.77.113306</a><a href="https://link.aps.org/doi/10.1103/PhysRevB.77.113306">]</a>

<ol start="2">

 <li><strong>Calculating the coupling terms of a 2D FEM matrix</strong></li>

</ol>

Write a code that computes the main parts of the matrix coefficients in the 2D scalar (node based) FEM case. Particularly, if the FEM basis functions are <em>L<sub>i</sub><sup>e</sup></em>(<strong>r</strong>) for <em>i </em>= 1,2,3, your code must compute:

<em>A<sub>ij </sub></em><em>dxdy </em>and <em>B<sub>ij </sub></em><em>dxdy</em>, where <em>e </em>is an arbitrary triangle given as user input. The derivation must be shown, along with the output of the code, and some method by which you have verified that the code is correct. Hint: An arbitrary triangle can be mapped to a unit triangle to make integration easier. Find the transformation.