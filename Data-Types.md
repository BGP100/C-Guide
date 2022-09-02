<a href="/Variables.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Constants.md">Next &gt;</a>
<hr>
As explained in the <a href="/Variables.md">Variables chapter</a>, a variable in C must be a specified data type, and you must use a format specifier inside the printf() function to display it:
<pre>
// Create variables
int myNum = 5;          // Integer (whole number)
float myFloatNum = 5.99; // Floating point number
char myLetter = 'D';      // Character<br>
// Print variables
printf("%d\n", myNum);
printf("%f\n", myFloatNum);
printf("%c\n", myLetter);
</pre>
<h1>Basic Data Types</h1>
The data type specifies the size and type of information the variable will store.
<br>
In this tutorial, we will focus on the most basic ones:
<table>
  <tr>
    <th>Data Type</th>
    <th>Size</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><code>int</code></td>
    <td>2 or 4 bytes</td>
    <td>Stores whole numbers, without decimals</td>
  </tr>
  <tr>
    <td><code>float</code></td>
    <td>4 bytes</td>
    <td>Stores fractional numbers, containing one or more decimals. Sufficient for storing 7 decimal digits</td>
  </tr>
  <tr>
    <td><code>double</code></td>
    <td>8 bytes</td>
    <td>Stores fractional numbers, containing one or more decimals. Sufficient for storing 15 decimal digits</td>
  </tr>
  <tr>
    <td><code>char</code></td>
    <td>1 byte</td>
    <td>Stores a single character/letter/number, or ASCII values</td>
  </tr>
</table>
<h1>Basic Format Specifiers</h1>
There are different format specifiers for each data type. Here are some of them:
<table>
  <tr>
    <th>Format Specifier</th>
    <th>Data Type</th>
  </tr>
  <tr>
    <td><code>%d</code> or <code>%i</code></td>
    <td><code>int</code></td>
  </tr>
  <tr>
    <td><code>%f</code></td>
    <td><code>float</code></td>
  </tr>
  <tr>
    <td><code>%lf</code></td>
    <td><code>double</code></td>
  </tr>
  <tr>
    <td><code>%c</code></td>
    <td><code>char</code></td>
  </tr>
  <tr>
    <td><code>%s</code></td>
    <td>Used for <b>strings</b>, which you will learn more about in a later chapter</td>
  </tr>
</table>
