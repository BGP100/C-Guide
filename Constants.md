<a href="/Data-Types.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Operators.md">Next &gt;</a>
<hr>
When you don't want others (or yourself) to override existing variable values, use the const keyword (this will declare the variable as "constant", which means unchangeable and read-only):
<pre>
const int myNum = 15; // myNum will always be 15
myNum = 10; // error: assignment of read-only variable 'myNum'
</pre>
You should always declare the variable as constant when you have values that are unlikely to change:
<pre>
const int minutesPerHour = 60;
const float PI = 3.14;
</pre>
<h1>Notes On Constants</h1>
When you declare a constant variable, it must be assigned with a value:
<pre>const int minutesPerHour = 60;</pre>
This however, will not work:
<pre>
const int minutesPerHour;
minutesPerHour = 60; // error
</pre>
<h1>Good Practice</h1>
Another thing about constant variables, is that it is considered good practice to declare them with uppercase. It is not required, but useful for code readability and common for C programmers:
<pre>const int BIRTHYEAR = 1969;</pre>
