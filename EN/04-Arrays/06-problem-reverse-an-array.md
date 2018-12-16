[slide]
# Problem: Reverse an Array of Integerss
- Read an **array of integers** (a number **n** + **n** lines of integers), **reverse** it and **print** its elements (on a single line, space separated):


```csharp
3
10
20
30

```
```csharp
30 20 10
```
```csharp
4
-1
20
99
5
```
```csharp
5 99 20 -1
```
Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/172#1]https://judge.softuni.bg/Contests/Practice/Index/172#1[/anchor]
[/slide]

[slide]
# Solution: Reverse an Array of Integers
```csharp
// Read the array (a number n + n lines of integers)
var n = int.Parse(Console.ReadLine());
var arr = new int[n];
for (int i = 0; i < n; i++)
  arr[i] = int.Parse(Console.ReadLine());

// Print the elements from the last to the first
for (int i = n-1; i >= 0; i--)
  Console.Write(arr[i] + " ");
Console.WriteLine();

```
Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/172#1]https://judge.softuni.bg/Contests/Practice/Index/172#1[/anchor]


# Try it yourself!

[code-task title="Reverse an Array of Integers" executionStrategy="csharp-dot-net-core-code" requiresInput]

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
Read an array of integers (a number n + n lines of integers), reverse it and print its elements (on a single line, space separated)
[/task-description]

[code-io /]
[/code-task]


[/slide]


