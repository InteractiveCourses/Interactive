[slide]
# Problem: Line Numbers
- Write a program that **reads** a text file and **inserts** line numbers in front of each of its **lines**. The **result** should be written to another text file. 




```csharp
Two households, both alike in dignity,In fair Verona, where we lay our scene,From ancient grudge break to new mutiny,Where civil blood makes civil hands unclean.
```
```csharp
1. Two households, both alike in dignity,
2. In fair Verona, where we lay our scene,
3. From ancient grudge break to new mutiny,
4. Where civil blood makes civil hands unclean.
```
Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/322#1]https://judge.softuni.bg/Contests/Practice/Index/322#1[/anchor]

[/slide]

[slide]
# Solution: Line Numbers
```csharp
string[] text = File.ReadAllLines("input.txt");

for (int i = 0; i < text.Length; i++)
{
  File.AppendAllText("output.txt", 
		      $"{i + 1}. {text[i]}{Environment.NewLine}");
}
```

Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/322#1]https://judge.softuni.bg/Contests/Practice/Index/322#1[/anchor]
[/slide]

[slide]
# Try it yourself!

[code-task title="Problem: Line Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]

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
Write a program that reads a text file and inserts line numbers in front of each of its lines. The result should be written to another text file. 
[/task-description]

[code-io /]
[/code-task]
[/slide]