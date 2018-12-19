[slide]
# Math Operations on Collections

`Min()` – Finds the smallest element in a collection

```text
{1, 2, 3, 4, -1, -5, 0, 50} => -5
```

`Max()` – Finds the largest element in a collection

```text
{1, 2, 3, 4, -1, -5, 0, 50} => 50
```

`Sum()` – Finds the sum of all elements in a collection

```text
{1, 2, 3, 4, -1, -5, 0, 50} => 54
```

`Average()` – Finds the average of all elements in a collection

```text
{1, 2, 3, 4, -1, -5, 0, 50} => 6.75
```

[/slide]

[slide]
# Problem: Sum, Min, Max, Average

Write a program to read **n** integers and print their **sum**, **min**, **max** and **average** values:

Input:
```text
5
12
20
-5
37
8
```

Output:
```text
Sum = 72
Min = -5
Max = 37
Average = 14.4
```

Input:
```text
4
50
20
25
40
```

Output:
```text
Sum = 135
Min = 20
Max = 50
Average = 33.75
```

Check your solution here:
[code-task title="Calculating sum, min, max, average" executionStrategy="csharp-code" requiresInput]
[code-editor language=csharp]
[/code-editor]
[task-description]Write a program to read **n** integers and print their **sum**, **min**, **max** and **average** values[/task-description]
[code-io /]
[/code-task]

[/slide]

[slide]
# Solution: Sum, Min, Max, Average

[code-task title="Calculating sum, min, max, average" executionStrategy="csharp-code" requiresInput]
[code-editor language=csharp]
```csharp
using System;
using System.Linq; // you need this for Sum(), Min(), etc.

class Program
{
  static void Main(string[] args)
  {
    int n = int.Parse(Console.ReadLine());
    int[] nums = new int[n];
    for (int i = 0; i < n; i++)
    {
      nums[i] = int.Parse(Console.ReadLine());
    }

    Console.WriteLine("Sum = {0}", nums.Sum());
    Console.WriteLine("Min = {0}", nums.Min());  
    // TODO: print also max and average values
  }
}
```
[/code-editor]
[task-description]Write a program to read **n** integers and print their **sum**, **min**, **max** and **average** values[/task-description]
[code-io /]
[/code-task]

[/slide]