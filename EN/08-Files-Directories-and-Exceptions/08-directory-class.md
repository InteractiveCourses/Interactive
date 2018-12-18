[slide]
# Directory Class in .NET
## Basic Operations
- **CreateDirectory()** – creates the directory and all subdirectories at the specified path, unless they already exist
```csharp
Directory.CreateDirectory("Test");
```

- **Delete()** – deletes an empty directory
```csharp
Directory.Delete("Test");
```

- **Move()** – moves a file or directory to a new location
```csharp
Directory.Move("Test", "New Folder");
```
[/slide]

[slide]
# Basic Operations(2)
- **GetFiles()** – returns the names of files (including their paths) in the specified directory
```csharp
string[] filesInDir = Directory.GetFiles("TestFolder");
```

- **GetDirectories()** – returns the names of subdirectories (including their paths) in the specified directory

```csharp
string[] subDirs = Directory.GetDirectories("TestFolder");
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


