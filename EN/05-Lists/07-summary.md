[slide]
# What did we learn today?
- **Lists** hold a variable sequence of elements
    - Can change number of elements (add/remove)
- Creating (allocating) a list:
```c#
List<int> numbers = new List<int>();
List<int> nums = 
	new List<int>() { 1, 2, 3 };
```
- Accessing list elements by index:
```c#
numbers[5] = 10;
```
- Printing list elements:
```c#
Console.Write(string.Join(" ", arr));
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
Test your code.
[/task-description]

[code-io /]
[/code-task]
[/slide]