<a href="/Structures/Copy.md">&lt; Previous</a>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<a href="/Structures/Example.md">Next &gt;</a>
<hr>
If you want to change/modify a value, you can use the dot syntax (.).
<br>
And to modify a string value, the strcpy() function is useful again:
<pre>
struct myStructure {
  int myNum;
  char myLetter;
  char myString[30];
};<br>
int main() {
  // Create a structure variable and assign values to it
  struct myStructure s1 = {13, 'B', "Some text"};<br>
  // Modify values
  s1.myNum = 30;
  s1.myLetter = 'C';
  strcpy(s1.myString, "Something else");<br>
  // Print values
  printf("%d %c %s", s1.myNum, s1.myLetter, s1.myString);<br>
  return 0;
}
</pre>
Modifying values are especially useful when you copy structure values:
<pre>
// Create a structure variable and assign values to it
struct myStructure s1 = {13, 'B', "Some text"};<br>
// Create another structure variable
struct myStructure s2;<br>
// Copy s1 values to s2
s2 = s1;<br>
// Change s2 values
s2.myNum = 30;
s2.myLetter = 'C';
strcpy(s2.myString, "Something else");<br>
// Print values
printf("%d %c %s\n", s1.myNum, s1.myLetter, s1.myString);
printf("%d %c %s\n", s2.myNum, s2.myLetter, s2.myString);
</pre>
<h1>Ok, so, how are structures useful?</h1>
Imagine you have to write a program to store different information about Cars, such as brand, model, and year. What's great about structures is that you can create a single "Car template" and use it for every cars you make. See below for a real life example.
