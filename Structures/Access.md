<a href="/Structures/Create.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Structures/Strings.md">Next &gt;</a>
<hr>
To access members of a structure, use the dot syntax (.):
<pre>
// Create a structure called myStructure
struct myStructure {
  int myNum;
  char myLetter;
};<br>
int main() {
  // Create a structure variable of myStructure called s1
  struct myStructure s1;<br>
  // Assign values to members of s1
  s1.myNum = 13;
  s1.myLetter = 'B';<br>
  // Print values
  printf("My number: %d\n", s1.myNum);
  printf("My letter: %c\n", s1.myLetter);<br>
  return 0;
}
</pre>
Now you can easily create multiple structure variables with different values, using just one structure:
<pre>
// Create different struct variables
struct myStructure s1;
struct myStructure s2;<br>
// Assign values to different struct variables
s1.myNum = 13;
s1.myLetter = 'B';<br>
s2.myNum = 20;
s2.myLetter = 'C';
</pre>
