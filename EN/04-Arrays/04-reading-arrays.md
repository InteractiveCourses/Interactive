[slide]
# Reading Arrays
## Reading Arrays From the Console
- First, read from the console the array length:
```csharp
int n = int.Parse(Console.ReadLine());
```
- Next, create an array of given size n and read its elements:
```csharp
int[] arr = new int[n];

for (int i = 0; i < n; i++)
{
   arr[i] = int.Parse(Console.ReadLine());
}
```

[/slide]

[slide]
# Reading Array Values from a Single Line
- Arrays can be read from a single line of space separated values:
```csharp
2 8 30 25 40 72 -2 44 56
```

```csharp
string values = Console.ReadLine();

string[] items = values.Split(' ');

int[] arr = new int[items.Length];

for (int i = 0; i < items.Length; i++)
   arr[i] = int.Parse(items[i]);

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
Try it yourself!
[/task-description]

[code-io /]
[/code-task]


[/slide]


