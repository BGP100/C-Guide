<a href="/Structures/Access.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Structures/Simpler-Syntax.md">Next &gt;</a>
<hr>
Remember that strings in C are actually an array of characters, and unfortunately, you can't assign a value to an array like this:
<pre>
struct myStructure {
  int myNum;
  char myLetter;
  char myString[30];  // String
};<br>
int main() {
  struct myStructure s1;<br>
  // Trying to assign a value to the string
  s1.myString = "Some text";<br>
  // Trying to print the value
  printf("My string: %s", s1.myString);<br>
  return 0;
}
</pre>
An error will occur:
<pre>prog.c:12:15: error: assignment to expression with array type</pre>
However, there is a solution for this! You can use the strcpy() function and assign the value to s1.myString, like this:
<pre>
struct myStructure {
  int myNum;
  char myLetter;
  char myString[30]; // String
};<br>
int main() {
  struct myStructure s1;<br>
  // Assign a value to the string using the strcpy function
  strcpy(s1.myString, "Some text");<br>
  // Print the value
  printf("My string: %s", s1.myString);<br>
  return 0;
}
</pre>
Result:
<pre>My string: Some text</pre>
