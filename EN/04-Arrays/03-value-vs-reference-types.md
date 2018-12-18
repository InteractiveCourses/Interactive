[slide]
# Value vs Reference Types
## Value types
- List of Value Types - 
[anchor href=https://msdn.microsoft.com/en-us/library/bfft1t3c.aspx]https://msdn.microsoft.com/en-us/library/bfft1t3c.aspx[/anchor]
- Variables of value types **directly** contain their data
- With **value types**, each variable has its own copy of the data, and it is not possible for operations on one variable to affect the other

[/slide]

[slide]
# Reference types
- Some of the reference types – **string**, **DateTime**, **TimeSpan**, **Random**, any other classes, interfaces, delegates and more 
- Variables of **reference types** store references to their data
- With reference types, two variables can reference the **same object**; therefore, operations on one variable can affect the object referenced by the other variable


[/slide]



[slide]
# Value vs Reference Types

[image src=https://github.com/InteractiveCourses/Interactive/blob/master/assets/arraysValueVSReferenceTypes.png alt="Value VS Reference Types" /]
## Example: Value Types 

```csharp
public static void Main(string[] args)
{
    int num = 5;
    Increment(num, 15);
    Console.WriteLine(num);
}

private static void Increment(int num, int value)
{
     num += value;
}

```

[/slide]

[slide]
# Example: Reference Types 
```csharp
public static void Main(string[] args)
{
    int[] nums = { 5 };
    Increment(nums, 15);
    Console.WriteLine(nums[0]);
}

private static void Increment(int[] nums, int value)
{
     nums[0] += value;
}
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


