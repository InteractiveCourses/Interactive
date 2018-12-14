[slide]
# Problem: Text Filter
- You are given a **text** and a **string** of banned words
    - Replace all banned words in the text.
        - You should replace with "**\***", **equal** to the word's length

```csharp
Linux, Windows
It is not Linux, it is GNU/Linux. Linux is merely the kernel, while GNU adds the functionality...
```
```csharp
It is not *****, it is GNU/*****. ***** is merely the kernel, while GNU adds the functionality...
```

Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/320#2]https://judge.softuni.bg/Contests/Practice/Index/320#2[/anchor]
[/slide]

[slide]
# Solution: Text Filter
```csharp
string[] banWords = Console.ReadLine()
 			.Split(…); // ToDo: Add separators
string text = Console.ReadLine();
foreach (var banWord in banWords)
{
   if (text.Contains(banWord))
   {
      text = text.Replace(banWord, new string('*', 						banWord.Length));
   }
}
 Console.WriteLine(text);
```
[/slide]

[slide]
# Try it yourself!
[code-task title="Text Filter" executionStrategy="csharp-dot-net-core-code" requiresInput]

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
Replace all banned words in the text. You should replace with "*", equal to the word's length.
[/task-description]

[code-io /]
[/code-task]
[/slide]