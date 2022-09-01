<a href="/Comments.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Data-Types.md">Next &gt;</a>
<hr>
Variables are containers for storing data values.
<br>
In C, there are different types of variables (defined with different keywords), for example:
<ul>
  <li><code>int</code> - stores integers (whole numbers), without decimals, such as 123 or -123
  <li><code>float</code> - stores floating point numbers, with decimals, such as 19.99 or -19.99
  <li><code>char</code> - stores single characters, such as 'a' or 'B'. Char values are surrounded by single quotes
</ul>
<h1>Declaring Variables</h1>
To create a variable, specify the type and assign it a value:
<pre>type variableName = value;</pre>
Where type is one of C types (such as <code>int</code>), and variableName is the name of the variable (such as x or myName). The equal sign is used to assign a value to the variable.
<br>
So, to create a variable that should store a number, look at the following example:
<pre>int myNum = 15;</pre>
You can also declare a variable without assigning the value, and assign the value later:
<pre>
int myNum;
myNum = 15;
</pre>
<b>Note:</b> If you assign a new value to an existing variable, it will overwrite the previous value:
<pre>
int myNum = 15; // myNum is 15
myNum = 10; // Now myNum is 10
</pre>
<h1>Output Variables</h1>
You learned from the output chapter that you can output values/print text with the printf() function:
<pre>printf("Hello World!");</pre>
In many other programming languages (like Python, Java, and C++), you would normally use a print function to display the value of a variable. However, this is not possible in C:
<pre>
int myNum = 15;
printf(myNum); // Nothing happens
</pre>
To output variables in C, you must get familiar with something called "format specifiers".
<h2>Format Specifiers</h2>
Format specifiers are used together with the printf() function to tell the compiler what type of data the variable is storing. It is basically a placeholder for the variable value.
<br>
A format specifier starts with a percentage sign %, followed by a character.
<br>
For example, to output the value of an int variable, you must use the format specifier %d or %i surrounded by double quotes, inside the printf() function:
<pre>
int myNum = 15;
printf("%d", myNum); // Outputs 15
</pre>
To print other types, use %c for char and %f for float:
<pre>
// Create variables
int myNum = 5;          // Integer (whole number)
float myFloatNum = 5.99; // Floating point number
char myLetter = 'D';      // Character<br>
// Print variables
printf("%d\n", myNum);
printf("%f\n", myFloatNum);
printf("%c\n", myLetter);
</pre>
To combine both text and a variable, separate them with a comma inside the printf() function:
<pre>
int myNum = 5;
printf("My favorite number is: %d", myNum);
</pre>
To print different types in a single printf() function, you can use the following:
<pre>
int myNum = 5;
char myLetter = 'D';
printf("My number is %d and my letter is %c", myNum, myLetter);
</pre>
You will learn more about Data Types in the next chapter.
<h1>Add Variables Together</h1>
To add a variable to another variable, you can use the + operator:
<pre>
int x = 5;
int y = 6;
int sum = x + y;
printf("%d", sum);
</pre>
<h1>Declare Multiple Variables</h1>
To declare more than one variable of the same type, use a comma-separated list:
<pre>
int x = 5, y = 6, z = 50;
printf("%d", x + y + z);
</pre>
You can also assign the same value to multiple variables of the same type:
<pre>
int x, y, z;
x = y = z = 50;
printf("%d", x + y + z);
</pre>
<h1>Variable Names</h1>
All C variables must be identified with unique names.
<br>
These unique names are called identifiers.
<br>
Identifiers can be short names (like x and y) or more descriptive names (age, sum, totalVolume).
<br>
<b>Note:</b> It is recommended to use descriptive names in order to create understandable and maintainable code:
<pre>
// Good
int minutesPerHour = 60;<br>
// OK, but not so easy to understand what m actually is
int m = 60;
</pre>
The general rules for naming variables are:
<ul>
  <li>Names can contain letters, digits and underscores
  <li>Names must begin with a letter or an underscore (<code>_</code>)
  <li>Names are case sensitive (myVar and myvar are different variables)
  <li>Names cannot contain whitespaces or special characters like !, #, %, etc.
  <li>Reserved words (such as int) cannot be used as names
</ul>
