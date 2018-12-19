[slide]
# Problem: Odd Occurrences

Write a program to extract from a given **sequence of words** all elements that are present in it an **odd number of times** (case-insensitive).

- Words are given in a single line, space separated
- Print the result elements in lowercase, in their order of appearance

Example:

Java C# PHP PHP JAVA C java -> java, c#, c
3 5 5 hi pi HO Hi 5 ho 3 hi pi -> 5, hi
a a A SQL xx a xx a A a XX c -> a, sql, xx, c

Check your solution here: 
[code-editor language=csharp]
[/code-editor]

[/slide]

[slide]
# Solution: Odd Occurrences

```csharp
string input = Console.ReadLine().ToLower();
string[] words = input.Split(' ');
var counts = new Dictionary<string, int>();

foreach (var word in words)
{
  if (counts.ContainsKey(word))
  {
    counts[word]++;
  }
  else
  {
    counts[word] = 1;
  }
}

var results = new List<string>();
foreach (var pair in counts)
{
  // TODO: add pair.Key to results if pair.Value is odd
}

Console.WriteLine(string.Join(", ", results));
```

Check your solution here: 
[code-editor language=csharp]
[/code-editor]

[/slide]