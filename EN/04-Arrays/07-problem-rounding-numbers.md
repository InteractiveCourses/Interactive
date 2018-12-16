[slide]
# Problem: Rounding Numbers
- Read an **array of real numbers** (space separated values), round them in "**away from 0**" style and **print** the output as in the examples:



```csharp
0.9 1.5 2.4 2.5 3.14
```
```csharp
0.9 => 1
1.5 => 2
2.4 => 2
2.5 => 3
3.14 => 3
```
```csharp
-5.01 -1.599 -2.5 -1.50 0
```
```csharp
-5.01 => -5
-1.599 => -2
-2.5 => -3
-1.50 => -2
0 => 0
```
Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/172#4]https://judge.softuni.bg/Contests/Practice/Index/172#4[/anchor]
[/slide]

[slide]
# Solution: Rounding Numbers
- Rounding turns each value to the nearest integer

```csharp
double[] nums = ReadNumbers();
int[] roundedNums = new int[nums.Length];

for (int i = 0; i < nums.Length; i++)
  roundedNums[i] = (int) Math.Round(nums[i],
  MidpointRounding.AwayFromZero);

for (int i = 0; i < nums.Length; i++)
   Console.WriteLine($"{nums[i]} -> {roundedNums[i]}");
```
Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/172#4]https://judge.softuni.bg/Contests/Practice/Index/172#4[/anchor]
[/slide]

[slide]
# Try it yourself!

[code-task title="Rounding Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]

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
Read an array of real numbers (space separated values), round them in "away from 0" style and print the output.
[/task-description]

[code-io /]
[/code-task]


[/slide]


