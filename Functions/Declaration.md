<a href="/Functions/Parameters.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Functions/Recursion.md">Next &gt;</a>
<hr>
You just learned from the previous chapters that you can create and call a function it the following way:
<pre>
// Create a function
void myFunction() {
  printf("I just got executed!");
}<br>
int main() {
  myFunction(); // call the function
  return 0;
}
</pre>
A function consist of two parts:
<ul>
  <li>Declaration: the function's name, return type, and parameters (if any)</li>
  <li>Definition: the body of the function (code to be executed)</li>
</ul>
<pre>
void myFunction() { // declaration
  // the body of the function (definition)
}
</pre>
For code optimization, it is recommended to separate the declaration and the definition of the function.
<br>
You will often see C programs that have function declaration above main(), and function definition below main(). This will make the code better organized and easier to read:
<pre>
// Function declaration
void myFunction();<br>
// The main method
int main() {
  myFunction(); // call the function
  return 0;
}<br>
// Function definition
void myFunction() {
  printf("I just got executed!");
}
</pre>
<h1>Another Example</h1>
If we use the example from the previous chapter regarding function parameters and return values:
<pre>
int myFunction(int x, int y) {
  return x + y;
}<br>
int main() { 
  int result = myFunction(5, 3); 
  printf("Result is = %d", result);<br>
  return 0;
}
// Outputs 8 (5 + 3)
</pre>
It is considered good practice to write it like this instead:
<pre>
// Function declaration
int myFunction(int, int);<br>
// The main method
int main() { 
  int result = myFunction(5, 3); // call the function
  printf("Result is = %d", result);<br>
  return 0;
}<br>
// Function definition
int myFunction(int x, int y) {
  return x + y;
}
</pre>
