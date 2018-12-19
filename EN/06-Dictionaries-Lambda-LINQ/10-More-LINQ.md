[slide]
# Take Single Element from Collection

Using `First()`:

```csharp
int[] nums = { 1, 2, 3, 4, 5, 6};
int num = nums.First(x => x % 2 == 0); 
// num = 2
```

Using `Last()`:

```csharp
int[] nums = { 1, 2, 3, 4, 5, 6};
int num = nums.Last(x => x % 2 == 1); 
// num = 5
```

Using `Single()`:

```int[] nums = { 1, 2, 3, 4, 5, 6};
int num = nums.Single(x => x == 4); 
// num = 4
```

`Single()` is similar to `First()`, but will throw an exception if more than one result is found.
[/slide]

[slide]
# Other Operations on Collections

Using `Reverse()`:

```csharp
int[] nums = { 1, 2, 3, 4, 5, 6};
nums = nums.Reverse(); 
// nums = 6, 5, 4, 3, 2, 1
```

Using `Concat()`:

```csharp
int[] nums = { 1, 2, 3, 4, 5, 6 };
int[] otherNums = { 7, 8, 9, 0 };
nums = nums.Concat(otherNums); 
// nums = 1, 2, 3, 4, 5, 6, 7, 8, 9, 0
```

[/slide]

[slide]
# Problem: Fold and Sum

Read an array of **4\*k integers**, **fold it** like shown below, and print the **sum** of the upper and lower rows (2\*k integers).

Input: 5 2 3 6
Folded:
```text
5 6
2 3
```
Sums:
```text
7 9
```

Input: 1 2 3 4 5 6 7 8
Folded:
```text
2 1 8 7
3 4 5 6
```
Sums:
```text
5 5 13 13
```

Input: 4 3 -1 2 5 0 1 9 8 6 7 -2
Folded:
```text
-1 3 4 -2 7 6
 2 5 0  1 9 8
```
Sums:
```text
1 8 4 -1 16 14
```

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
    int[] arr = Console.ReadLine()
        .Split(' ').Select(int.Parse).ToArray();
    // ...
  }
}
```
[/code-editor]
[task-description]Read an array, fold it, and print the sums of the columns.[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution: Fold and Sum

[code-task title="Fold and sum" executionStrategy="csharp-code" requiresInput]
[code-editor language=csharp]
```csharp
using System;
using System.Collections.Generic;
using System.Linq;

class Program
{
  static void Main(string[] args)
  {
    int[] arr = Console.ReadLine()
        .Split(' ').Select(int.Parse).ToArray();
    int k = arr.Length / 4;
    int[] row1left = arr.Take(k).Reverse().ToArray();
    int[] row1right = arr.Reverse().Take(k).ToArray();
    int[] row1 = row1left.Concat(row1right).ToArray();
    int[] row2 = arr.Skip(k).Take(2 * k).ToArray();
    var sumArr = row1.Select((x, index) => x + row2[index]);
    Console.WriteLine(string.Join(" ", sumArr));
  }
}
```
[/code-editor]
[task-description]Read an array, fold it, and print the sums of the columns.[/task-description]
[code-io /]
[/code-task]
[/slide]