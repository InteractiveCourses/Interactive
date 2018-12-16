[slide]
# File – Output Operations
- **WriteAllText()** – takes a string and writes it to a file


```csharp
File.WriteAllText("output.txt", "Files are fun");
```

- **WriteAllLines()** – takes a collection and writes every element on a new line

```csharp
string[] names = {"pesho", "ivan", "stamat", "mariika"};
File.WriteAllLines("output.txt", names);
```
- There are also **AppendAllText()** and **AppendAllLines()** methods, that just add additional text to a file.


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


