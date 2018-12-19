[slide]
# Transforming Collections

Using `Select()` to transform all elements of a collection:

```csharp
var nums = Console.ReadLine()
               .Split()
               .Select(number => double.Parse(number));
// or          .Select(double.Parse);
```

The above turns a collection of `string` values to a collection of `double` (number) values.
[/slide]

[slide]
# Converting Collections

Using `ToArray()`, `ToList()` to convert collections:

```csharp
int[] nums = Console.ReadLine()
              .Split()
              .Select(number => int.Parse(number))
              .ToArray();
```

Or, if you want a list:

```csharp
List<double> nums = Console.ReadLine()
              .Split()
              .Select(double.Parse)
              .ToList();
```

There are also `ToDictionary()` and `ToCharArray()` methods that we will see later.
[/slide]

[slide]
# Sorting Collections

Using `OrderBy()` to sort collections:

```csharp
List<int> nums = new List<int> { 1, 5, 2, 4, 3 };
nums = nums
          .OrderBy(num => num)
          .ToList();
		  
// nums = { 1, 2, 3, 4, 5 }
```

Using `OrderByDescending()` to sort collections:

```csharp
List<int> nums = new List<int> { 1, 5, 2, 4, 3 };
nums = nums
          .OrderByDescending(num => num)
          .ToList();
		  
// nums = { 5, 4, 3, 2, 1 }
```

[/slide]

[slide]
# Sorting Collections (2)

Using `ThenBy()` to sort collections by more than 1 criteria:

```csharp
Dictionary<int, string> products = new Dictionary<int, string>();
Dictionary<int, string> sortedDict = products
                   .OrderBy(pair => pair.Value)
                   .ThenBy(pair => pair.Key)
                   .ToDictionary(pair => pair.Key, pair => pair.Value);
```

Similar to `OrderByDescending()`, there is also `ThenByDescending()`.
[/slide]

[slide]
# Take/Skip N Elements from Collection

Using `Take()`:

```csharp
int[] nums = { 1, 2, 3, 4, 5, 6};
nums = nums
       .Take(3)
       .ToArray(); 

// nums = [1, 2, 3]
```

Using `Skip()`:

```csharp
int[] nums = { 1, 2, 3, 4, 5, 6};
nums = nums
       .Skip(3)
       .ToArray(); 

// nums = [4, 5, 6]
```

[/slide]

[slide]
# Problem: Largest 3 Numbers

Read a **list of real numbers** and **print the largest 3 of them**.

Input: 10 **30** 15 **20** **50** 5
Output: 50 30 20

Input: 20 30
Output: 30 20

Input: 0 -5 -1 -3 -2
Output: 0 -1 -2

Check your solution here:
[code-task title="Working with collections" executionStrategy="csharp-code" requiresInput]
[code-editor language=csharp]
```csharp
using System;
using System.Collections.Generic; // needed for List<T>
using System.Linq;  // needed for Select(), OrderBy(), etc.

class Program
{
  static void Main(string[] args)
  {
    string[] strings = Console.ReadLine().Split(' ');
    // List<int> nums = ...
  }
}
```
[/code-editor]
[task-description]Read a **list of real numbers** and **print the largest 3 of them**[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Largest 3 Numbers

[code-task title="Working with collections" executionStrategy="csharp-code" requiresInput]
[code-editor language=csharp]
```csharp
using System;
using System.Collections.Generic; // needed for List<T>
using System.Linq;  // needed for Select(), OrderBy(), etc.

class Program
{
  static void Main(string[] args)
  {
    string[] strings = Console.ReadLine().Split(' ');
    List<int> nums = strings
                     .Select(int.Parse)
                     .ToList();

    var sortedNums = nums.OrderByDescending(x => x);
    var largest3Nums = sortedNums.Take(3);
    Console.WriteLine(string.Join(" ", largest3Nums));
  }
}
```
[/code-editor]
[task-description]Read a **list of real numbers** and **print the largest 3 of them**[/task-description]
[code-io /]
[/code-task]
[/slide]
