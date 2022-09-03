<a href="/Structures/Strings.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Structures/Copy.md">Next &gt;</a>
<hr>
You can also assign values to members of a structure variable at declaration time, in a single line.
<br>
Just insert the values in a comma-separated list inside curly braces {}. Note that you don't have to use the strcpy() function for string values with this technique:
<pre>
// Create a structure
struct myStructure {
  int myNum;
  char myLetter;
  char myString[30];
};<br>
int main() {
  // Create a structure variable and assign values to it
  struct myStructure s1 = {13, 'B', "Some text"};<br>
  // Print values
  printf("%d %c %s", s1.myNum, s1.myLetter, s1.myString);<br>
  return 0;
}
</pre>
<b>Note:</b> The order of the inserted values must match the order of the variable types declared in the structure (13 for int, 'B' for char, etc).
