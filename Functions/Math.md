<a href="/Functions/Recursion.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Structures/Main.md">Next &gt;</a>
<hr>
There is also a list of math functions available, that allows you to perform mathematical tasks on numbers.
<br>
To use them, you must include the math.h header file in your program:
<pre>#include &lt;math.h&gt;</pre>
<h1>Square Root</h1>
To find the square root of a number, use the sqrt() function:
<pre>printf("%f", sqrt(16));</pre>
<h1>Round a Number</h1>
The ceil() function rounds a number upwards to its nearest integer, and the floor() method rounds a number downwards to its nearest integer, and returns the result:
<pre>
printf("%f", ceil(1.4));
printf("%f", floor(1.4));
</pre>
<h1>Power</h1>
The pow() function returns the value of x to the power of y (xy):
<pre>printf("%f", pow(4, 3));</pre>
<h1>Other Math Functions</h1>
A list of other popular math functions (from the <code>&lt;math.h&gt;</code> library) can be found in the table below:
<table class="ws-table-all notranslate" style="margin:0">
  <tr>
    <th>Function</th>
    <th>Description</th>
  </tr>
  <tr>
    <td>abs(x)</td>
    <td>Returns the absolute value of x</td>
  </tr>
  <tr>
    <td>acos(x)</td>
    <td>Returns the arccosine of x</td>
  </tr>
  <tr>
    <td>asin(x)</td>
    <td>Returns the arcsine of x</td>
  </tr>
  <tr>
    <td>atan(x)</td>
    <td>Returns the arctangent of x</td>
  </tr>
  <tr>
    <td>cbrt(x)</td>
    <td>Returns the cube root of x</td>
 </tr>
  <tr>
    <td>cos(x)</td>
    <td>Returns the cosine of x</td>
  </tr>
  <tr>
    <td>exp(x)</td>
    <td>Returns the value of E<sup>x</sup></td>
 </tr>
  <tr>
    <td>sin(x)</td>
    <td>Returns the sine of x (x is in radians)</td>
 </tr>
  <tr>
    <td>tan(x)</td>
    <td>Returns the tangent of an angle</td>
  </tr>
</table>
