[slide]
# Problem: Odd Lines
- Write a program that **reads** a text file and **writes** its **every odd line** in another file. Line numbers **starts** from 0.



```csharp
Two households, both alike in dignity,In fair Verona, where we lay our scene,From ancient grudge break to new mutiny, Where civil blood makes civil hands unclean.From forth the fatal loins of these two foes A pair of star-cross lovers take their life; Whose misadventured piteous overthrows Do with their death bury their parents strife.

```
```csharp
In fair Verona, where we lay our scene,
Where civil blood makes civil hands unclean.
A pair of star-cross lovers take their life;
Do with their death bury their parents strife
```
Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/322#0]https://judge.softuni.bg/Contests/Practice/Index/322#0[/anchor]

[/slide]

[slide]
# Solution: Odd Lines
```csharp
string[] text = File.ReadAllLines("input.txt");

for (int i = 1; i < text.Length; i+=2)
{
    File.AppendAllText("output.txt", text[i] + Environment.NewLine);
}
```
```csharp
string[] text = File.ReadAllLines("input.txt");

File.WriteAllLines("output.txt", 
                         text.Where((line, index) => index % 2 == 1));
```
Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/322#0]https://judge.softuni.bg/Contests/Practice/Index/322#0[/anchor]
[/slide]

[slide]
# Try it yourself!

[code-task title="Problem: Odd Lines" executionStrategy="csharp-dot-net-core-code" requiresInput]

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
Write a program that reads a text file and writes its every odd line in another file. Line numbers starts from 0. 
[/task-description]

[code-io /]
[/code-task]


[/slide]


