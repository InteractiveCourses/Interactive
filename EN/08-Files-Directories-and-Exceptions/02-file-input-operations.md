[slide]
# File – Input Operations
## Input Operations
**File Class** in **System.IO** namespace provides static methods for the **creation**, **copying**, **deletion**, **moving**, and **opening** of a single **file**, and aids in the creation of **FileStream objects**.
- **ReadAllText()** – reads everything at once and returns a string

```csharp
using System.IO;
…
string file = File.ReadAllText("file.txt");

```

- **ReadAllLines()** – reads line by line and returns a collection


```csharp
using System.IO;
…
String[] file = File.ReadAllLines("file.txt");


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


