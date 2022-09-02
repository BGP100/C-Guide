<a href="/Strings.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Memory-Address.md">Next &gt;</a>
<hr>
You have already learned that printf() is used to output values in C.
<br>
To get user input, you can use the scanf() function:
<pre>
// Create an integer variable that will store the number we get from the user
int myNum;<br>
// Ask the user to type a number
printf("Type a number: \n");<br>
// Get and save the number the user types
scanf("%d", &myNum);<br>
// Output the number the user typed
printf("Your number is: %d", myNum);
</pre>
The scanf() function takes two arguments: the format specifier of the variable (%d in the example above) and the reference operator (&myNum), which stores the memory address of the variable.
<br>
<b>Tip:</b> You will learn more about memory addresses and functions in the next chapter.
<h1>User Input Strings</h1>
You can also get a string entered by the user:
<pre>
// Create a string
char firstName[30];<br>
// Ask the user to input some text
printf("Enter your first name: \n");<br>
// Get and save the text
scanf("%s", firstName);<br>
// Output the text
printf("Hello %s.", firstName);
</pre>
Note that you must specify the size of the string/array (we used a very high number, 30, but atleast then we are certain it will store enough characters for the first name), and you don't have to specify the reference operator (&) when working with strings in scanf().
