<a href="/User-Input.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Pointers.md">Next &gt;</a>
<hr>
When a variable is created in C, a memory address is assigned to the variable.
<br>
The memory address is the location of where the variable is stored on the computer.
<br>
When we assign a value to the variable, it is stored in this memory address.
<br>
To access it, use the reference operator (&), and the result will represent where the variable is stored:
<pre>
int myAge = 43;
printf("%p", &myAge); // Outputs 0x7ffe5367e044
</pre>
<b>Note:</b> The memory address is in hexadecimal form (0x..). You probably won't get the same result in your program.
<br>
You should also note that &myAge is often called a "pointer". A pointer basically stores the memory address of a variable as its value. To print pointer values, we use the %p format specifier.
<br>
You will learn much more about pointers in the next chapter.
<br>
Why is it useful to know the memory address?
<br>
Pointers are important in C, because they give you the ability to manipulate the data in the computer's memory - this can reduce the code and improve the performance.
<br>
Pointers are one of the things that make C stand out from other programming languages, like Python and Java.
