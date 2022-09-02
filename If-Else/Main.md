<a href="/Operators.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/If-Else/Short-Hand.md">Next &gt;</a>
<hr>
You learned from the operators comparison chapter, that C supports the usual logical conditions from mathematics:
<ul>
  <li>Less than: <code>a &lt; b</code></li>
  <li>Less than or equal to: <code>a &lt;= b</code></li>
  <li>Greater than: <code>a &gt; b</code></li>
  <li>Greater than or equal to: <code>a &gt;= b</code></li>
  <li>Equal to: <code>a == b</code></li>
  <li>Not Equal to: <code>a != b</code></li>
</ul>
You can use these conditions to perform different actions for different decisions.
<br>
C has the following conditional statements:
<ul>
  <li>Use if to specify a block of code to be executed, if a specified condition is true</li>
  <li>Use else to specify a block of code to be executed, if the same condition is false</li>
  <li>Use else if to specify a new condition to test, if the first condition is false</li>
  <li>Use switch to specify many alternative blocks of code to be executed</li>
</ul>
<h1>The if Statement</h1>
Use the if statement to specify a block of C code to be executed if a condition is true.
<pre>
if (<i>condition</i>) {
  // block of code to be executed if the condition is true
}
</pre>
Note that if is in lowercase letters. Uppercase letters (If or IF) will generate an error.

In the example below, we test two values to find out if 20 is greater than 18. If the condition is true, print some text:
<pre>
if (20 &gt; 18) {
  printf("20 is greater than 18");
}
</pre>
We can also test variables:
<pre>
int x = 20;
int y = 18;
if (x > y) {
  printf("x is greater than y");
}
</pre>
<h2>Example explained</h2>
In the example above we use two variables, x and y, to test whether x is greater than y (using the <code>&gt;</code> operator). As x is 20, and y is 18, and we know that 20 is greater than 18, we print to the screen that "x is greater than y".
<h1>The else Statement</h1>
Use the else statement to specify a block of code to be executed if the condition is false.
<pre>
if (<i>condition</i>) {
  // block of code to be executed if the condition is true
} else { 
  // block of code to be executed if the condition is false
} 
</pre>
<pre>
int time = 20;
if (time &lt; 18) {
  printf("Good day.");
} else {
  printf("Good evening.");
}
// Outputs "Good evening."
</pre>
<h2>Example explained</h2>
In the example above, time (20) is greater than 18, so the condition is false. Because of this, we move on to the else condition and print to the screen "Good evening". If the time was less than 18, the program would print "Good day".
<h1>The else if Statement</h1>
Use the else if statement to specify a new condition if the first condition is false.
<pre>
if (<i>condition1</i>) {
  // block of code to be executed if condition1 is true
} else if (<i>condition2</i>) {
  // block of code to be executed if the condition1 is false and condition2 is true
} else {
  // block of code to be executed if the condition1 is false and condition2 is false
}
</pre>
<pre>
int time = 22;
if (time &lt; 10) {
  printf("Good morning.");
} else if (time &lt; 20) {
  printf("Good day.");
} else {
  printf("Good evening.");
}
// Outputs "Good evening."
</pre>
<h2>Example explained</h2>
In the example above, time (22) is greater than 10, so the first condition is false. The next condition, in the else if statement, is also false, so we move on to the else condition since condition1 and condition2 is both false - and print to the screen "Good evening".
<br>
However, if the time was 14, our program would print "Good day."
<h2>Another Example</h2>
This example shows how you can use if..else if to find out if a number is positive or negative:
<pre>
int myNum = 10; // Is this a positive or negative number?<br>
if (myNum &gt; 0)
  printf("The value is a positive number.");
else if (myNum &lt; 0)
  printf("The value is a negative number.");
else
  printf("The value is 0.");
