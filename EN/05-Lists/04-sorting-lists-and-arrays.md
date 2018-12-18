[slide]
# Sorting Lists and Arrays
## Sorting Lists
- **Sorting** a list == reorder its elements incrementally
    - List items should be **comparable**, e.g. numbers, strings, dates, …


```csharp
var names = new List<string>() { 
  "Nakov", "Angel", "Ivan", "Atanas", "Boris" };
names.Sort(); // Sort in natural order (ascending)
Console.WriteLine(string.Join(", ", names)); 
// Angel, Atanas, Boris, Ivan, Nakov
names.Sort();
names.Reverse(); // Sort in descending order
Console.WriteLine(string.Join(", ", names));
// Nakov, Ivan, Boris, Atanas, Angel
```
[/slide]

[slide]
# Problem: Sort Numbers 
- Read a **list of decimal numbers** and **sort** them

```csharp
8 2 7 3
```
```csharp
2 <= 3 <= 7 <= 8
```
 

```csharp
1 1
```
```csharp
1 <= 1
```

```csharp
2 4 -9
```
```csharp
-9 <= 2 <= 4
```
 

```csharp
1 -0.5
```
```csharp
-0.5 <= 1
```

Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/397#4]https://judge.softuni.bg/Contests/Practice/Index/397#4[/anchor]

[/slide]

[slide]
# Solution: Sort Numbers

```csharp
string[] input = Console.ReadLine().Split(' ');
List<double> nums = new List<double>();
foreach(string num in input)
{
    nums.Add(double.Parse(num));
}
nums.Sort();
Console.WriteLine(string.Join(" <= ", nums));
```
Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/397#4]https://judge.softuni.bg/Contests/Practice/Index/397#4[/anchor]
[/slide]

[slide]
# Try it yourself!

[code-task title="Problem: Sort Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]

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
Read a list of decimal numbers and sort them.
[/task-description]

[code-io /]
[/code-task]


[/slide]


