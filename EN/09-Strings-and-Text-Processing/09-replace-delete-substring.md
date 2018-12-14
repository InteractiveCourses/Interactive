[slide]
# Replacing & Deleting Substrings
    - The text processing in .NET Framework provides ready methods for replacing a substring with another. **str.Replace(string match, string term)** – replaces all occurrences of given string with another
        -The result is a new string (strings are immutable)


```csharp
string cocktail = "Vodka + Martini + Cherry";
string replaced = cocktail.Replace("+", "and");
// Vodka and Martini and Cherry
```
    - **str.Remove(int index, int length)** – deletes part of a string and produces a new string as result


```csharp
string price = "$ 1234567";
string lowPrice = price.Remove(2, 3);
// $ 4567
```
[/slide]





[slide]
# Problem: Text filter
- You are given a text and a string of banned words
    - Replace all banned words in the text.
        - You should replace with "*", equal to the word's length
```csharp
Linux, Windows
It is not Linux, it is GNU/Linux. Linux is merely the kernel, while GNU adds the functionality...

```
will be:

```csharp
It is not *****, it is GNU/*****. ***** is merely the kernel, while GNU adds the functionality...
```

## Try it yourself!

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


[slide]
# Solution: Text Filter
```csharp
string[] banWords = Console.ReadLine()
 			.Split(…); // ToDo: Add seprators
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