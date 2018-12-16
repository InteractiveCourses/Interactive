[slide]
# Problem: Reverse Array of Strings
- Read an **array of strings** (space separated values), reverse it and **print** its elements:

```csharp
a b c d e  =>  e d c b a
```
```csharp
-1 hi ho w  =>  w ho hi -1
```
- Reversing array elements:

Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/172#5]https://judge.softuni.bg/Contests/Practice/Index/172#5[/anchor]
[/slide]

[slide]
# Solution: Reverse Array of Strings

```csharp
var nums = Console.ReadLine().Split(' ').ToArray();
for (int i = 0; i < nums.Length / 2; i++)
  SwapElements(nums, i, nums.Length - 1 - i);
Console.WriteLine(string.Join(" ", nums));

static void SwapElements(string[] arr, int i, int j)
{
  var oldElement = arr[i];
  arr[i] = arr[j];
  arr[j] = oldElement;
}
```
Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/172#5]https://judge.softuni.bg/Contests/Practice/Index/172#5[/anchor]
[/slide]

[slide]
# Try it yourself!

[code-task title="Reverse Array of Strings" executionStrategy="csharp-dot-net-core-code" requiresInput]

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
Read an array of strings (space separated values), reverse it and print its elements.
[/task-description]

[code-io /]
[/code-task]
[/slide]