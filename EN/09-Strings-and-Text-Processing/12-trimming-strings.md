[slide]
# Trimming White Space
When entering text in a file or to the console, you can find sometimes some "parasitic" spaces (white-space) at the beginning or at the end of the text – some other space or a tab that cannot be observed at first glance. This may not be essential but if we do not validate the user data, there would be a problem in terms of checking the contents of the input information. In order to solve this problem we can use the method Trim(). It is responsible for eliminating (trimming) the white spaces at the beginning or at the end of a string. The white spaces can be spaces, tabs, line breaks etc.
- **str.Trim()** – trims whitespaces at start and end of string


```csharp
string s = "    example of white space    ";
string clean = s.Trim();
Console.WriteLine(clean); // example of white space
```
- **str.Trim(params char[] chars)**
Please note that we must list all the characters we want to eliminate, including the empty spaces (spaces, tabs, new line, etc.). Without a ' ' in the array trimChars, we would not get the desired result!
```csharp
string s = " \t\nHello!!! \n";
string clean = s.Trim(' ', ',' ,'!', '\n','\t');
Console.WriteLine(clean); // Hello
```

- **str.TrimStart() and str.TrimEnd()**

```csharp
string s = "   C#   ";
string clean = s.TrimStart(); // clean = "C#   ";
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


