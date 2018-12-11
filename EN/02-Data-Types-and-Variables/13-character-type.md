[slide]
# The Character Data Type
Character type is a single character (16-bit number of a Unicode table character). It is declared in C# with the keyword char. The Unicode table is a technological standard that represents any character (letter, punctuation, etc.) from all human languages as writing systems (all languages and alphabets) with an integer or a sequence of integers. The smallest possible value of a char variable is 0, and the largest one is 65535. The values of type char are letters or other characters, and are enclosed in apostrophes.

- The character data type:
    - Represents symbolic information
    - Is declared by the char keyword
    - Gives each symbol a corresponding integer code
    - Has a '\0' default value
    - Takes 16 bits of memory (from U+0000 to U+FFFF)
    - Holds a single Unicode character (or part of character)
[/slide]

[slide]
# Characters and Codes
- Each character has an uniqueUnicode value (int):
```csharp
char ch = 'a';
Console.WriteLine("The code of '{0}' is: {1}", ch, (int) ch);
ch = 'b';
Console.WriteLine("The code of '{0}' is: {1}", ch, (int) ch);
ch = 'A';
Console.WriteLine("The code of '{0}' is: {1}", ch, (int) ch);
ch = 'щ';  // Cyrillic letter 'sht'
Console.WriteLine("The code of '{0}' is: {1}", ch, (int) ch);

```
[/slide]


[slide]

# Problem: Triples of Latin Letters
- Write a program to read an integer n and print all triples of the first n small Latin letters, ordered alphabetically:
```csharp
        aaa acc bcb cca
        aab baa bcc ccb
        aac bab caa ccc
3 ->    aba bac cab 
        abb bba cac 
        abc bbb cba 
        aca bbc cbb 
        acb bca cbc 

```

Check your solution here: 

[/slide]

[slide]
# Solution: Triples of Latin Letters
```csharp
int n = int.Parse(Console.ReadLine());
  for (int i1 = 0; i1 < n; i1++)
    for (int i2 = 0; i2 < n; i2++)
      for (int i3 = 0; i3 < n; i3++)
      {
        char letter1 = (char)('a' + i1);
        char letter2 = // TODO: finish this
        char letter3 = // TODO: finish this
        Console.WriteLine("{0}{1}{2}",
          letter1, letter2, letter3);
      }

```
Check your solution here: 
[/slide]

