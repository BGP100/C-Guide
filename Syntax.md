<a href="/Get-Started.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Output/Print-Text.md">Next &gt;</a>
<hr>
You have already seen the following code a couple of times in the first chapters. Let's break it down to understand it better:
<pre>
#include &lt;stdio.h&gt;<br>

int main() {
  printf("Hello World!");
  return 0;
}
</pre>
<h1>Example explained</h1>
Line 1: <code>#include &lt;stdio.h&gt;</code> is a header file library that lets us work with input and output functions, such as <code>printf()</code> (used in line 4). Header files add functionality to C programs.
<br>
<b>Tip:</b> Don't worry if you don't understand how <code>#include &lt;stdio.h&gt;</code> works. Just think of it as something that (almost) always appears in your program.
<br>
Line 2: A blank line. C ignores white space. But we use it to make the code more readable.
<br>
Line 3: Another thing that always appear in a C program, is <code>main()</code>. This is called a function. Any code inside its curly brackets <code>{}</code> will be executed.
<br>
Line 4: <code>printf()</code> is a function used to output/print text to the screen. In our example it will output <code>"Hello World"</code>.
<br>
<b>Note that:</b> Every C statement ends with a semicolon <code>;</code>
<br>
<b>Note:</b> The body of <code>int main()</code> could also been written as: <code>int main(){printf("Hello World!");return 0;}</code>
<br>
<b>Remember</b>: The compiler ignores white spaces. However, multiple lines makes the code more readable.
<br>
Line 5: <code>return 0</code> ends the <code>main()</code> function.
<br>
Line 6: Do not forget to add the closing curly bracket <code>}</code> to actually end the main function.
