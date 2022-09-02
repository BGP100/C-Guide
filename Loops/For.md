<a href="/Switch.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Loops/For.md">Next &gt;</a>
<hr>
When you know exactly how many times you want to loop through a block of code, use the for loop instead of a while loop:
<pre>
for (statement 1; statement 2; statement 3) {
  // code block to be executed
}
</pre>
Statement 1 is executed (one time) before the execution of the code block.
<br>
Statement 2 defines the condition for executing the code block.
<br>
Statement 3 is executed (every time) after the code block has been executed.
<br>
The example below will print the numbers 0 to 4:
<pre>
int i;<br>
for (i = 0; i &lt; 5; i++) {
  printf("%d\n", i);
}
</pre>
<h1>Example explained</h1>
Statement 1 sets a variable before the loop starts (<code>int i = 0</code>).
<br>
Statement 2 defines the condition for the loop to run (i must be less than 5). If the condition is true, the loop will start over again, if it is false, the loop will end.
<br>
Statement 3 increases a value (<code>i++</code>) each time the code block in the loop has been executed.
<h1>Another Example</h1>
This example will only print even values between 0 and 10:
<pre>
for (i = 0; i &lt;= 10; i = i + 2) {
  printf("%d\n", i);
}
</pre>
