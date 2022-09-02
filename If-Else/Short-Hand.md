<a href="/If-Else/Main.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Switch.md">Next &gt;</a>
<hr>
There is also a short-hand if else, which is known as the ternary operator because it consists of three operands. It can be used to replace multiple lines of code with a single line. It is often used to replace simple if else statements:
<pre>variable = (condition) ? expressionTrue : expressionFalse;</pre>
Instead of writing:
<pre>
int time = 20;
if (time &lt; 18) {
  printf("Good day.");
} else {
  printf("Good evening.");
}
</pre>
You can simply write:
<pre>
int time = 20;
(time &lt; 18) ? printf("Good day.") : printf("Good evening.");
</pre>
It is completely up to you if you want to use the traditional if...else statement or the ternary operator.
