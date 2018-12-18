[slide]
# Problem: Count Numbers 
- Read a **list of integers** in range [0…1000] and **print them in ascending order** along with their **number of occurrences**

```csharp
8 2 2 8 2 2 3 7
```
```csharp
2 -> 4
3 -> 1
7 -> 1
8 -> 2
```
 

```csharp
10 8 8 10 10
```
```csharp
8 -> 2
10 -> 3
```

```csharp
0 5 0 0 1 0
```
```csharp
0 -> 4
1 -> 1
5 -> 1
```
 

Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/397#6]https://judge.softuni.bg/Contests/Practice/Index/397#6[/anchor]

[/slide]

[slide]
# Solution: Count Numbers (Simple)

```csharp
var nums = Console.ReadLine().Split(' ')
  .Select(int.Parse).ToList();
var counts =
  new int[nums.Max() + 1]; // counts[num] holds how many times num occurs in the list
foreach (var num in nums)
    counts[num]++;
for (int i = 0; i < counts.Length; i++)
    if (counts[i] > 0)
        Console.WriteLine($"{i} -> {counts[i]}");
```
Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/397#6]https://judge.softuni.bg/Contests/Practice/Index/397#6
[/slide]

[slide]
# Solution: Count Numbers (by Sorting)

```csharp
List<int> nums = ReadNumbers();
nums.Sort();
var pos = 0; // Sort the numbers
while (pos < nums.Count)
{
  int num = nums[pos], count = 1;
  while (pos + count < nums.Count && 
         nums[pos + count] == num) // Count how times num occurs starting from position pos
    count++;
  pos = pos + count;
  Console.WriteLine($"{num} -> {count}");
}
```
Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/397#6]https://judge.softuni.bg/Contests/Practice/Index/397#6
[/slide]

[slide]
# Try it yourself!

[code-task title="Problem: Count Numbers" executionStrategy="csharp-dot-net-core-code" requiresInput]

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
Read a list of integers in range [0…1000] and print them in ascending order along with their number of occurrences.
[/task-description]

[code-io /]
[/code-task]


[/slide]


