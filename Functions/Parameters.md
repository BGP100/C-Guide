<a href="/Functions/Main.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Functions/Declaration.md">Next &gt;</a>
<hr>
Information can be passed to functions as a parameter. Parameters act as variables inside the function.
<br>
Parameters are specified after the function name, inside the parentheses. You can add as many parameters as you want, just separate them with a comma:
<pre>
returnType functionName(parameter1, parameter2, parameter3) {
  // code to be executed
}
</pre>
The following function that takes a string of characters with name as parameter. When the function is called, we pass along a name, which is used inside the function to print "Hello" and the name of each person.
<pre>
void myFunction(char name[]) {
  printf("Hello %s\n", name);
}<br>
int main() {
  myFunction("Liam");
  myFunction("Jenny");
  myFunction("Anja");
  return 0;
}<br>
// Hello Liam
// Hello Jenny
// Hello Anja
</pre>
When a parameter is passed to the function, it is called an argument. So, from the example above: name is a parameter, while Liam, Jenny and Anja are arguments.
<h1>Multiple Parameters</h1>
Inside the function, you can add as many parameters as you want:
<pre>
void myFunction(char name[], int age) {
  printf("Hello %s. You are %d years old.\n", name, age);
}<br>
int main() {
  myFunction("Liam", 3);
  myFunction("Jenny", 14);
  myFunction("Anja", 30);
  return 0;
}<br>
// Hello Liam. You are 3 years old.
// Hello Jenny. You are 14 years old.
// Hello Anja. You are 30 years old.
</pre>
Note that when you are working with multiple parameters, the function call must have the same number of arguments as there are parameters, and the arguments must be passed in the same order.
<h1>Return Values</h1>
The void keyword, used in the previous examples, indicates that the function should not return a value. If you want the function to return a value, you can use a data type (such as int or float, etc.) instead of void, and use the return keyword inside the function:
<pre>
int myFunction(int x) {
  return 5 + x;
}<br>
int main() {
  printf("Result is: %d", myFunction(3));<br>
  return 0;
}<br>
// Outputs 8 (5 + 3)
</pre>
This example returns the sum of a function with two parameters:
<pre>
int myFunction(int x, int y) {
  return x + y;
}<br>
int main() {
  printf("Result is: %d", myFunction(5, 3));<br>
  return 0;
}<br>
// Outputs 8 (5 + 3)
</pre>
You can also store the result in a variable:
<pre>
int myFunction(int x, int y) {
  return x + y;
}<br>
int main() { 
  int result = myFunction(5, 3); 
  printf("Result is = %d", result);<br>
  return 0;
}<br>
// Outputs 8 (5 + 3)
</pre>
