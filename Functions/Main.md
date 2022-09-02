<a href="/Pointers.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Functions/Parameters.md">Next &gt;</a>
<hr>
A function is a block of code which only runs when it is called.
<br>
You can pass data, known as parameters, into a function.
<br>
Functions are used to perform certain actions, and they are important for reusing code: Define the code once, and use it many times.
<h1>Predefined Functions</h1>
So it turns out you already know what a function is. You have been using it the whole time while studying this tutorial!
<br>
For example, main() is a function, which is used to execute code, and printf() is a function; used to output/print text to the screen:
<pre>
int main() {
  printf("Hello World!");
  return 0;
}
</pre>
<h1>Create a Function</h1>
To create (often referred to as declare) your own function, specify the name of the function, followed by parentheses () and curly brackets {}:
<pre>
void myFunction() {
  // code to be executed
}
</pre>
<h2>Example Explained</h2>
<ul>
  <li><code>myFunction()</code> is the name of the function</li>
  <li><code>void</code> means that the function does not have a return value. You will learn more about return values later in the next chapter</li>
  <li>Inside the function (the body), add code that defines what the function should do</li>
</ul>
<h1>Call a Function</h1>
Declared functions are not executed immediately. They are "saved for later use", and will be executed when they are called.
<br>
To call a function, write the function's name followed by two parentheses () and a semicolon ;
<br>
In the following example, myFunction() is used to print a text (the action), when it is called:
<pre>
// Create a function
void myFunction() {
  printf("I just got executed!");
}<br>
int main() {
  myFunction(); // call the function
  return 0;
}<br>
// Outputs "I just got executed!"
</pre>
A function can be called multiple times:
<pre>
void myFunction() {
  printf("I just got executed!");
}<br>
int main() {
  myFunction();
  myFunction();
  myFunction();
  return 0;
}<br>
// I just got executed!
// I just got executed!
// I just got executed!
</pre>
