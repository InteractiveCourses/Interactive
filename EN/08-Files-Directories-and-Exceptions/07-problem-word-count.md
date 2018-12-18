[slide]
# Problem: Word Count
- Write a program that **reads a list of words** from the file words.txt and finds **how many times** each of the words is **contained** in another file text.txt. Matching should be **case-insensitive**. Write the **results** in file results.txt. Sort the words by **frequency** in **descending** order. 




```csharp
quick is fault
```

```csharp
-I was quick to judge him, but it wasn't his fault.
-Is this some kind of joke?! Is it?
-Quick, hide here…It is safer.
```

```csharp
is - 3
quick - 2
fault - 1
```
Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/322#3]https://judge.softuni.bg/Contests/Practice/Index/322#3[/anchor]

[/slide]

[slide]
# Solution: Word Count
```csharp
string[] words = File.ReadAllText("words.txt").ToLower().Split();
string[] text = File.ReadAllText("input.txt").ToLower()
         .Split(new char[] {'\n','\r',' ', '.', ',', '!', '?', '-'}, 	StringSplitOptions.RemoveEmptyEntries);

Dictionary<string, int> wordCount = new Dictionary<string, int>();

foreach (string word in words)
    wordCount[word] = 0;

foreach (string word in text)
    if (wordCount.ContainsKey(word))
         wordCount[word]++;

// Save the Output to a file
```

Check your solution here:
[anchor href=https://judge.softuni.bg/Contests/Practice/Index/322#3]https://judge.softuni.bg/Contests/Practice/Index/322#3[/anchor]
[/slide]

[slide]
# Try it yourself!

[code-task title="Problem: Word Count" executionStrategy="csharp-dot-net-core-code" requiresInput]

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
Write a program that reads a list of words from the file words.txt and finds how many times each of the words is contained in another file text.txt. Matching should be case-insensitive. Write the results in file results.txt. Sort the words by frequency in descending order. 
[/task-description]

[code-io /]
[/code-task]
[/slide]