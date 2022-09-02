<a href="/Memory-Address.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Functions/Main.md">Next &gt;</a>
<hr>
You learned from the previous chapter, that we can get the memory address of a variable with the reference operator &:
<pre>
int myAge = 43; // an int variable<br>
printf("%d", myAge);  // Outputs the value of myAge (43)
printf("%p", &myAge); // Outputs the memory address of myAge (0x7ffe5367e044)
</pre>
In the example above, &myAge is also known as a pointer.
<br>
A pointer is a variable that stores the memory address of another variable as its value.
<br>
A pointer variable points to a data type (like int) of the same type, and is created with the * operator. The address of the variable you're working with is assigned to the pointer:
<pre>
int myAge = 43;  // An int variable
int* ptr = &amp;myAge; // A pointer variable, with the name ptr, that stores the address of myAge<br>
// Output the value of myAge (43)
printf("%d\n", myAge);<br>
// Output the memory address of myAge (0x7ffe5367e044)
printf("%p\n", &myAge);<br>
// Output the memory address of myAge with the pointer (0x7ffe5367e044)
printf("%p\n", ptr);
</pre>
<h2>Example explained</h2>
Create a pointer variable with the name ptr, that points to an int variable (myAge). Note that the type of the pointer has to match the type of the variable you're working with.
<br>
Use the & operator to store the memory address of the myAge variable, and assign it to the pointer.
<br>
Now, ptr holds the value of myAge's memory address.
<h1>Dereference</h1>
In the example above, we used the pointer variable to get the memory address of a variable (used together with the & reference operator).
<br>
However, you can also get the value of the variable the pointer points to, by using the * operator (the dereference operator):
<pre>
int myAge = 43;     // Variable declaration
int* ptr = &amp;myAge;  // Pointer declaration<br>
// Reference: Output the memory address of myAge with the pointer (0x7ffe5367e044)
printf("%p\n", ptr);<br>
// Dereference: Output the value of myAge with the pointer (43)
printf("%d\n", *ptr);
</pre>
Note that the <code>*</code> sign can be confusing here, as it does two different things in our code:
<ul>
  <li>When used in declaration (<code>int* ptr</code>), it creates a pointer variable.</li>
  <li>When not used in declaration, it act as a dereference operator.</li>
</ul>
Why Should I Learn About Pointers? Pointers are important in C, because they give you the ability to manipulate the data in the computer's memory - this can reduce the code and improve the performance.
<br>
Pointers are one of the things that make C stand out from other programming languages, like Python and Java.
<br>
<b>Note:</b> Pointers must be handled with care, since it is possible to damage data stored in other memory addresses.
<br>
<b>Good To Know:</b> There are three ways to declare pointer variables, but the first way is mostly used:
<pre>
int* myNum; // Most used
int *myNum;
int * myNum;
</pre>
