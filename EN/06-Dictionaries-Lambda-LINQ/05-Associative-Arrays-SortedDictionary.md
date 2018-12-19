[slide]
# SortedDictionary<K, V>

Like `Dictionary<K, V>`, but keeps elements sorted by the key - using a `foreach` will give elements in order, instead of randomly (like a normal `Dictionary` would do).
[/slide]

[slide]
# Events – SortedDictionary Example

```csharp
var events = new SortedDictionary<DateTime, string>();

events[new DateTime(1998, 9, 4)] = "Google's birth date";
events[new DateTime(2013, 11, 5)] = "SoftUni's birth date";
events[new DateTime(1975, 4, 4)] = "Microsoft's birth date";
events[new DateTime(2004, 2, 4)] = "Facebook's birth date";
events[new DateTime(2013, 11, 5)] = "SoftUni was founded";

foreach (var entry in events)
{
   Console.WriteLine("{0:dd-MMM-yyyy}: {1}", 
      entry.Key, entry.Value);
}
```
[/slide]

[slide]
# Problem: Count Real Numbers 

Read a **list of real numbers** and **print them in ascending order** along with their **number of occurrences**.

Examples:

Input: 8 2.5 2.5 8 2.5
Output:
```text
2.5 -> 3 times
8 -> 2 times
```

Input: -2 0.33 0.33 2
Output:
```text
-2 -> 1 times
0.33 -> 2 times
2 -> 1 times
```

Check your solution here: 
[code-editor language=csharp]
[/code-editor]

[/slide]

[slide]
# Solution: Count Real Numbers

```csharp
string[] nums = Console.ReadLine().Split(' ');
var counts = new SortedDictionary<double, int>();

foreach (var num in nums)
{
  double parsedNum = double.Parse(num);
  if (counts.ContainsKey(parsedNum))
  {
    counts[parsedNum]++;
  }
  else
  {
    counts[parsedNum] = 1;
  }
}

foreach (var num in counts.Keys)
{
  Console.WriteLine($"{num} -> {counts[num]}");
}
```

Check your solution here: 
[code-editor language=csharp]
[/code-editor]

[/slide]