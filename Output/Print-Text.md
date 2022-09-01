<a href="/Syntax.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Output/New-Lines.md">Next &gt;</a>
<hr>
The <code>printf()</code> function is used to output values/print text:
<pre>
#include &lt;stdio.h&gt;<br>
int main() {
  printf("Hello World!");
  return 0;
}
</pre>
You can add as many <code>printf()</code> functions as you want. However, note that it does not insert a new line at the end of the output:
<pre>
#include &lt;stdio.h&gt;<br>
int main() {
  printf("Hello World!");
  printf("I am learning C.");
  return 0;
}
</pre>
