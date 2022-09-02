<a href="/Loops/For.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Arrays.md">Next &gt;</a>
<hr>
<h1>Break</h1>
You have already seen the break statement used in an earlier chapter of this tutorial. It was used to "jump out" of a switch statement.
<br>
The break statement can also be used to jump out of a loop.
<br>
This example jumps out of the loop when i is equal to 4:
<pre>
int i;<br>
for (i = 0; i &lt; 10; i++) {
  if (i == 4) {
    break;
  }
  printf("%d\n", i);
}
</pre>
<h1>Continue</h1>
The continue statement breaks one iteration (in the loop), if a specified condition occurs, and continues with the next iteration in the loop.
<br>
This example skips the value of 4:
<pre>
int i;<br>
for (i = 0; i &lt; 10; i++) {
  if (i == 4) {
    continue;
  }
  printf("%d\n", i);
} 
</pre>
<h1>Break and Continue in While Loop</h1>
You can also use break and continue in while loops:
<pre>
int i = 0;<br>
while (i &lt; 10) {
  if (i == 4) {
    <b>break</b>;
  }
  printf("%d\n", i);
  i++;
} 
</pre>
<pre>
int i = 0;<br>
while (i &lt; 10) {
  if (i == 4) {
    i++;
    <b>continue</b>;
  }
  printf("%d\n", i);
  i++;
}
</pre>
