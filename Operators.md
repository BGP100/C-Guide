<a href="/Data-Types.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Operators.md">Next &gt;</a>
<hr>
Operators are used to perform operations on variables and values.
<br>
In the example below, we use the <code>+</code> operator to add together two values:
<pre>int myNum = 100 + 50;</pre>
Although the <code>+</code> operator is often used to add together two values, like in the example above, it can also be used to add together a variable and a value, or a variable and another variable:
<pre>
int sum1 = 100 + 50;    // 150 (100 +  50)
int sum2 = sum1 + 250;  // 400 (150 + 250)
int sum3 = sum2 + sum2; // 800 (400 + 400)
</pre>
C divides the operators into the following groups:
<ul>
  <li>Arithmetic operators</li>
  <li>Assignment operators</li>
  <li>Comparison operators</li>
  <li>Logical operators</li>
  <li>Bitwise operators</li>
</ul>
<h1>Arithmetic Operators</h1>
Arithmetic operators are used to perform common mathematical operations.
<table>
<tr>
<th>Operator</th>
<th>Name</th>
<th>Description</th>
<th>Example</th>
</tr>
<tr>
<td>+</td>
<td>Addition</td>
<td>Adds together two values</td>
<td>x + y</td>
</tr>
<tr>
<td>-</td>
<td>Subtraction</td>
<td>Subtracts one value from another</td>
<td>x - y</td>
</tr>
<tr>
<td>*</td>
<td>Multiplication</td>
<td>Multiplies two values</td>
<td>x * y</td>
</tr>
<tr>
<td>/</td>
<td>Division</td>
<td>Divides one value by another</td>
<td>x / y</td>
</tr>
<tr>
<td>%</td>
<td>Modulus</td>
<td>Returns the division remainder</td>
<td>x % y</td>
</tr>
<tr>
<td>++</td>
<td>Increment</td>
<td>Increases the value of a variable by 1</td>
<td>++x</td>
</tr>
<tr>
<td>--</td>
<td>Decrement</td>
<td>Decreases the value of a variable by 1</td>
<td>--x</td>
</tr>
</table>
<h1>Assignment Operators</h1>
Assignment operators are used to assign values to variables.
<br>
In the example below, we use the assignment operator (<code>=</code>) to assign the value 10 to a variable called x:
<pre>int x = 10;</pre>
The addition assignment operator (<code>+=</code>) adds a value to a variable:
<pre>
int x = 10;
x += 5;
</pre>
A list of all assignment operators:
<table class="ws-table-all notranslate">
<tr>
<th>Operator</th>
<th>Example</th>
<th>Same As</th>
</tr>
<tr>
<td>=</td>
<td>x = 5</td>
<td>x = 5</td>
</tr>
<tr>
<td>+=</td>
<td>x += 3</td>
<td>x = x + 3</td>
</tr>
<tr>
<td>-=</td>
<td>x -= 3</td>
<td>x = x - 3</td>
</tr>
<tr>
<td>*=</td>
<td>x *= 3</td>
<td>x = x * 3</td>
</tr>
<tr>
<td>/=</td>
<td>x /= 3</td>
<td>x = x / 3</td>
</tr>
<tr>
<td>%=</td>
<td>x %= 3</td>
<td>x = x % 3</td>
</tr>
<tr>
<td>&amp;=</td>
<td>x &amp;= 3</td>
<td>x = x &amp; 3</td>
</tr>
<tr>
<td>|=</td>
<td>x |= 3</td>
<td>x = x | 3</td>
</tr>
<tr>
<td>^=</td>
<td>x ^= 3</td>
<td>x = x ^ 3</td>
</tr>
<tr>
<td>&gt;&gt;=</td>
<td>x &gt;&gt;= 3</td>
<td>x = x &gt;&gt; 3</td>
</tr>
<tr>
<td>&lt;&lt;=</td>
<td>x &lt;&lt;= 3</td>
<td>x = x &lt;&lt; 3</td>
</tr>
</table>
<h1>Comparison Operators</h1>
Comparison operators are used to compare two values.
<br>
<b>Note:</b> The return value of a comparison is either true (1) or false (0).
<br>
In the following example, we use the greater than operator (<code>&gt;</code>) to find out if 5 is greater than 3:
<pre>
int x = 5;
int y = 3;
printf("%d", x &gt; y); // returns 1 (true) because 5 is greater than 3
</pre>
A list of all comparison operators:
<table>
<tr>
<th>Operator</th>
<th>Name</th>
<th>Example</th>
</tr>
<tr>
<td>==</td>
<td>Equal to</td>
<td>x == y</td>
</tr>
<tr>
<td>!=</td>
<td>Not equal</td>
<td>x != y</td>
</tr>
<tr>
<td>&gt;</td>
<td>Greater than</td>
<td>x &gt; y</td>
</tr>
<tr>
<td>&lt;</td>
<td>Less than</td>
<td>x &lt; y</td>
</tr>
<tr>
<td>&gt;=</td>
<td>Greater than or equal to</td>
<td>x &gt;= y</td>
</tr>
<tr>
<td>&lt;=</td>
<td>Less than or equal to</td>
<td>x &lt;= y</td>
</tr>
</table>
<h1>Logical Operators</h1>
Logical operators are used to determine the logic between variables or values:
<table>
<tr>
<th>Operator</th>
<th>Name</th>
<th>Description</th>
<th>Example</th>
</tr>
<tr>
<td>&amp;&amp;&nbsp;</td>
<td>Logical and</td>
<td>Returns true if both statements are true</td>
<td>x &lt; 5 &amp;&amp;&nbsp; x &lt; 10</td>
</tr>
<tr>
<td>||&nbsp;</td>
<td>Logical or</td>
<td>Returns true if one of the statements is true</td>
<td>x &lt; 5 || x &lt; 4</td>
</tr>
<tr>
<td>!</td>
<td>Logical not</td>
<td>Reverse the result, returns false if the result is true</td>
<td>!(x &lt; 5 &amp;&amp; x &lt; 10)</td>
</tr>
</table>
<h1>Sizeof Operator</h1>
The memory size (in bytes) of a data type or a variable can be found with the sizeof operator:
<pre>
int myInt;
float myFloat;
double myDouble;
char myChar;<br>
printf("%lu\n", sizeof(myInt));
printf("%lu\n", sizeof(myFloat));
printf("%lu\n", sizeof(myDouble));
printf("%lu\n", sizeof(myChar));
</pre>
Note that we use the %lu format specifer to print the result, instead of %d. It is because the compiler expects the sizeof operator to return a long unsigned int (%lu), instead of int (%d). On some computers it might work with %d, but it is safer to use %lu.
