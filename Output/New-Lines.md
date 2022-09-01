<a href="/Output/Print-Text.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Comments.md">Next &gt;</a>
<hr>
To insert a new line, you can use the <code>\n</code> character:
<pre>
#include &lt;stdio.h&gt;<br>
int main() {
  printf("Hello World!\n");
  printf("I am learning C.");
  return 0;
}
</pre>
You can also output multiple lines with a single <code>printf()</code> function. However, be aware that this will make the code harder to read:
<pre>
#include &lt;stdio.h&gt;<br>
int main() {
  printf("Hello World!\nI am learning C.\nAnd it is awesome!");
  return 0;
}
</pre>
<b>Tip:</b> Two <code>\n</code> characters after each other will create a blank line:
<pre>
#include &lt;stdio.h&gt;<br>
int main() {
  printf("Hello World!\n\n");
  printf("I am learning C.");
  return 0;
}
</pre>
<h1>What is <code>\n</code> exactly?</h1>
The newline character (<code>\n</code>) is called an escape sequence, and it forces the cursor to change its position to the beginning of the next line on the screen. This results in a new line.
<br>
Examples of other valid escape sequences are:
<table>
  <tr>
    <th>Escape Sequence</th>
    <th>Description</th>
  </tr>
  <tr>
    <td><code>\t</code></td>
    <td>Creates a horizontal tab</td>
  </tr>
  <tr>
    <td><code>\\</code></td>
    <td>Inserts a backslash character (<code>\</code>)</td>
  </tr>
  <tr>
    <td><code>\"</code> or <code>\'</code></td>
    <td>Inserts the quotes character</td>
  </tr>
</table>
