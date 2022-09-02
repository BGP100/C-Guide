<a href="/BreakAndContinue.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Strings.md">Next &gt;</a>
<hr>
Arrays are used to store multiple values in a single variable, instead of declaring separate variables for each value.
<br>
To create an array, define the data type (like int) and specify the name of the array followed by square brackets [].
<br>
To insert values to it, use a comma-separated list, inside curly braces:
<pre>int myNumbers[] = {25, 50, 75, 100};</pre>
We have now created a variable that holds an array of four integers.
<h1>Access the Elements of an Array</h1>
To access an array element, refer to its index number.
<br>
Array indexes start with 0: <code>[0]</code> is the first element. <code>[1]</code> is the second element, etc.
<br>
This statement accesses the value of the first element <code>[0]</code> in myNumbers:
<pre>
int myNumbers[] = {25, 50, 75, 100};
printf("%d", myNumbers[0]);<br>
// Outputs 25
</pre>
<h1>Change an Array Element</h1>
To change the value of a specific element, refer to the index number:
<pre>myNumbers[0] = 33;</pre>
<pre>
int myNumbers[] = {25, 50, 75, 100};
myNumbers[0] = 33;<br>
printf("%d", myNumbers[0]);<br>
// Now outputs 33 instead of 25
</pre>
<h1>Loop Through an Array</h1>
You can loop through the array elements with the for loop.
<br>
The following example outputs all elements in the myNumbers array:
<pre>
int myNumbers[] = {25, 50, 75, 100};
int i;<br>
for (i = 0; i &lt; 4; i++) {
  printf("%d\n", myNumbers[i]);
}
</pre>
<h1>Set Array Size</h1>
Another common way to create arrays, is to specify the size of the array, and add elements later:
<pre>
// Declare an array of four integers:
int myNumbers[4];<br>
// Add elements
myNumbers[0] = 25;
myNumbers[1] = 50;
myNumbers[2] = 75;
myNumbers[3] = 100;
</pre>
Using this method, you should know the size of the array, in order for the program to store enough memory.
<br>
You are not able to change the size of the array after creation.
