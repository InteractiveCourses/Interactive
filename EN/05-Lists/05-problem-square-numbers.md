[slide]
# Problem: Square Numbers 
- Read a **list of integers** and print all **square numbers** in the list in descending order
A "**square number**" **s** is a square of some other integer: **s** = **x** * **x**

```csharp
3 16 4 5 6 8 9

16 9 4
```

```csharp
var squares = new List<int>();
foreach (var num in nums)
  if (√num == (int)√num) squares.Add(num);
// TODO: sort squares descending and print them
```
[/slide]

Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/397#5]https://judge.softuni.bg/Contests/Practice/Index/397#5[/anchor]

[/slide]

[slide]
# Try it yourself!

[code-task title="Problem: Square Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]

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
Read a list of integers and print all square numbers in the list in descending order. A "square number" s is a square of some other integer: s = x * x.
[/task-description]

[code-io /]
[/code-task]
[/slide]


