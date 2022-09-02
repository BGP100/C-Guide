<a href="/If-Else/Short-Hand.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Loops/While.md">Next &gt;</a>
<hr>
Instead of writing many <b>if..else</b> statements, you can use the switch statement.
<br>
The switch statement selects one of many code blocks to be executed:
<pre>
switch(expression) {
  case x:
    // code block
    break;
  case y:
    // code block
    break;
  default:
    // code block
}
</pre>
This is how it works:
<ul>
  <li>The <b>switch</b> expression is evaluated once</li>
  <li>The value of the expression is compared with the values of each case</li>
  <li>If there is a match, the associated block of code is executed</li>
  <li>The <b>break</b> statement breaks out of the switch block and stops the execution</li>
  <li>The <b>default</b> statement is optional, and specifies some code to run if there is no case match</li>
</ul>
The example below uses the weekday number to calculate the weekday name:
<pre>
int day = 4;<br>
switch (day) {
  case 1:
    printf("Monday");
    break;
  case 2:
    printf("Tuesday");
    break;
  case 3:
    printf("Wednesday");
    break;
  case 4:
    printf("Thursday");
    break;
  case 5:
    printf("Friday");
    break;
  case 6:
    printf("Saturday");
    break;
  case 7:
    printf("Sunday");
    break;
}<br>
// Outputs "Thursday" (day 4)
</pre>
<h1>The break Keyword</h1>
When C reaches a break keyword, it breaks out of the switch block.
<br>
This will stop the execution of more code and case testing inside the block.
<br>
When a match is found, and the job is done, it's time for a break. There is no need for more testing.
<br>
A break can save a lot of execution time because it "ignores" the execution of all the rest of the code in the switch block.
<h1>The default Keyword</h1>
The default keyword specifies some code to run if there is no case match:
<pre>
int day = 4;<br>
switch (day) {
  case 6:
    printf("Today is Saturday");
    break;
  case 7:
    printf("Today is Sunday");
    break;
  default:
    printf("Looking forward to the Weekend");
}<br>
// Outputs "Looking forward to the Weekend"
</pre>
<b>Note:</b> The default keyword must be used as the last statement in the switch, and it does not need a break.
