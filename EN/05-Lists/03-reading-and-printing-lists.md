[slide]
# Reading Lists From the Console
- First, read from the console the array **length**:

```csharp
int n = int.Parse(Console.ReadLine());
```

- Next, create a list of given size **n** and read its **elements**:

```csharp
List<int> list = new List<int>();

for (int i = 0; i < n; i++)
{
   list.Add(int.Parse(Console.ReadLine()));
}

```
[/slide]

[slide]
# Reading Array Values from a Single Line
- Arrays can be read from a **single line** of **space separated values**:

```csharp
2 8 30 25 40 72 -2 44 56
```
```csharp
string values = Console.ReadLine();

// string.Split(' ') splits string by space and produces a collection
// .ToList() turn the collection into a List
List<string> items = values.Split(' ').ToList();

List<int> nums = new List<int>();

for (int i = 0; i < items.Count; i++)
{
    nums.Add(int.Parse(items[i]));
}
```
[/slide]

[slide]
# Printing Lists on the Console
- To print all list elements, a **for**-loop can be used
    - Separate elements with white **space** or a **new line**
- Example:

```csharp
List<string> list = new List<string>() {"one", "two", "three", "four", "five"};
// Process all list elements
for (int index = 0; index < list.Count; index++)
{
  // Print each element on a separate line
  Console.WriteLine("arr[{0}] = {1}", index, list[index]);
}

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


