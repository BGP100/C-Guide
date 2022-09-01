<a href="/Home.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Get-Started.md">Next &gt;</a>
<hr>
To start using C, you need two things:
<ul>
  <li>A text editor, like Notepad, to write C code</li>
  <li>A compiler, like GCC, to translate the C code into a language that the computer will understand</li>
</ul>
There are many text editors and compilers to choose from. In this tutorial, we will use an IDE (see below).
<h1>C Install IDE</h1>
An IDE (Integrated Development Environment) is used to edit AND compile the code.
<br>
Popular IDE's include Code::Blocks, Eclipse, and Visual Studio. These are all free, and they can be used to both edit and debug C code.
<br>
<b>Note:</b> Web-based IDE's can work as well, but functionality is limited.
<br>
We will use Code::Blocks in our tutorial, which we believe is a good place to start.
<br>
You can find the latest version of Codeblocks at http://www.codeblocks.org/. Download the mingw-setup.exe file, which will install the text editor with a compiler.
<h1>C Quickstart</h1>
Let's create our first C file.
<br>
Open Codeblocks and go to File &gt; New &gt; Empty File.
<br>
Write the following C code and save the file as <code>myfirstprogram.c</code> (File &gt; Save File as):
<pre>
#include &lt;stdio.h&gt;<br>
int main() {
  printf("Hello World!");
  return 0;
}
</pre>
Don't worry if you don't understand the code above - we will discuss it in detail in later chapters. For now, focus on how to run the code.
<br>
In Codeblocks, it should look like this:
<br>
<img src="https://i.imgur.com/v8pUiPl.png">
<br>
Then, go to Build &gt; Build and Run to run (execute) the program.
<br>
Congratulations! You have now written and executed your first C program.
