[slide]
# Problem: Count Substring Occurrences
- You are given a **text** and a **pattern**
    - Find how many **times** that pattern is in the text.
        - Overlapping is allowed


```csharp
ababa caba
aba
```
```csharp
3
```

```csharp
aaaaaa
aa
```
```csharp
5
```

```csharp
Welcome to SoftUni
Java
```
```csharp
0
```

Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/320#1]https://judge.softuni.bg/Contests/Practice/Index/320#1[/anchor]
[/slide]

[slide]
# Solution: Count Substring Occurrences
```csharp
string input = Console.ReadLine().ToLower();
string pattern = Console.ReadLine().ToLower();
int counter = 0;
int index = input.IndexOf(pattern);
while (index != -1)
{
   counter++;
   index = input.IndexOf(pattern, index + 1)
}
Console.WriteLine(counter);
```
[/slide]

[slide]
# Try it yourself!
[code-task title="Count Substring Occurrences" executionStrategy="csharp-dot-net-core-code" requiresInput]

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
Find how many **times** that pattern is in the text.
Overlapping is allowed.
[/task-description]

[code-io /]
[/code-task]
[/slide]