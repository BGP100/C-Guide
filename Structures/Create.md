<a href="/Structures/Main.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Structures/Access.md">Next &gt;</a>
<hr>
You can create a structure by using the struct keyword and declare each of its members inside curly braces:
<pre>
struct MyStructure { // Structure declaration
  int myNum;         // Member (int variable)
  char myLetter;    // Member (char variable)
}; // End the structure with a semicolon
</pre>
To access the structure, you must create a variable of it.
<br>
Use the struct keyword inside the main() method, followed by the name of the structure and then the name of the structure variable:
<br>
Create a struct variable with the name "s1":
<pre>
struct myStructure {
  int myNum;
  char myLetter;
};<br>
int main() {
  struct myStructure s1;
  return 0;
}
</pre>
