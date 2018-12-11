[slide]
# Finding a character or substring within given string
When we have a string with a specified content, it is often necessary to process only a **part** of its value. The .NET platform provides us with **two methods** to search a string within another string: **IndexOf(…)** and **LastIndexOf(…)**. They search into the string and check whether the passed as a parameter substring occurs in its content. The **result** of those methods is an **integer**. If the result is **not a negative** value, then this is the position where the first character of the substring is found. If the method returns value of **-1**, it means that the substring was **not found**. Remember that in C# indexing into strings **start from 0**. The methods IndexOf(…) and LastIndexOf(…) search the contents of the text sequence, but in a different direction.

- Finding a character or substring within given string
    - **str.IndexOf(string term)** – returns the index of the first occurrence of term in str
        - Returns -1 if there is no match
  

```csharp
string email = "vasko@gmail.org";
int firstIndex = email.IndexOf("@"); // 5
int noIndex = email.IndexOf("/"); // -1
```
    - **str.LastIndexOf(string term)** – returns the index of the last occurrence of **term** in **str**

```csharp
string verse = "To be or not to be..";
int lastIndex = verse.LastIndexOf("be"); // 16
```
## Try it yourself!

[/slide]


[slide]
# Problem: Count substring occurrences
- You are given a text and a pattern
    - Find how many times that pattern is in the text.
        - Overlapping is allowed

```csharp
ababa caba
aba
3
```

```csharp
aaaaaa
aa
5
```

```csharp
Welcome to SoftUni
Java
0
```
Check your solution here:

[/slide]


[slide]
# Solution: Count substring occurrences

```csharp
string input = Console.ReadLine().ToLower();
string pattern = Console.ReadLine().ToLower();
int counter = 0;
int index = input.IndexOf(pattern);
while (index != -1)
{
   counter++;
   index = input.IndexOf(pattern, index + 1)
}
Console.WriteLine(counter);
```

[/slide]


