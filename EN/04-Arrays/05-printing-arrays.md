[slide]
# Printing Arrays
## Printing Arrays on the Console
- To print all array elements, a for-loop can be used
    - Separate elements with white space or a new line
- Example:

```csharp
string[] arr = {"one", "two", "three", "four", "five"};
// Process all array elements
for (int index = 0; index < arr.Length; index++)
{
  // Print each element on a separate line
  Console.WriteLine("arr[{0}] = {1}", index, arr[index]);
}

```
[/slide]

[slide]
# Printing Arrays with foreach / String.Join(…)
- Use **foreach**-loop:

```csharp
int[] arr = { 10, 20, 30, 40, 50};
foreach (var element in arr)
   Console.WriteLine(element)
```
- Use **string.Join(separator, array)**:
```csharp
int[] arr = { 1, 2, 3 };
Console.WriteLine(string.Join(", ", arr)); // 1, 2, 3
string[] strings = { "one", "two", "three", "four" };
Console.WriteLine(string.Join(" - ", strings)); // one - two - three - four
```
[/slide]


[slide]
# Try it yourself!

[code-task title="Try it yourself!" executionStrategy="csharp-dot-net-core-code" requiresInput]

[code-editor language=csharp]
```
using System;

namespace App
{
    class Program
    {
        static void Main(string[] args)
        {
		    // enter your code here
		    
		}
	}
}
```
[/code-editor]

[task-description]
Try it yourself!
[/task-description]

[code-io /]
[/code-task]


[/slide]


