<a href="/Switch.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Loops/For.md">Next &gt;</a>
<hr>
Loops can execute a block of code as long as a specified condition is reached.
<br>
Loops are handy because they save time, reduce errors, and they make code more readable.
<h1>While Loop</h1>
The while loop loops through a block of code as long as a specified condition is true:
<pre>
while (<i>condition</i>) {
  // code block to be executed
}
</pre>
In the example below, the code in the loop will run, over and over again, as long as a variable (i) is less than 5:
<pre>
int i = 0;<br>
while (i &lt; 5) {
  printf("%d\n", i);
  i++;
}
</pre>
<b>Note:</b> Do not forget to increase the variable used in the condition (<code>i++</code>), otherwise the loop will never end!
<h1>The Do/While Loop</h1>
The do/while loop is a variant of the while loop. This loop will execute the code block once, before checking if the condition is true, then it will repeat the loop as long as the condition is true.
<pre>
do {
  // code block to be executed
}
while (<i>condition</i>);
</pre>
The example below uses a do/while loop. The loop will always be executed at least once, even if the condition is false, because the code block is executed before the condition is tested:
<pre>
int i = 0;<br>
do {
  printf("%d\n", i);
  i++;
}
while (i &lt; 5);
</pre>
<b>Note:</b> Do not forget to increase the variable used in the condition (<code>i++</code>), otherwise the loop will never end!
