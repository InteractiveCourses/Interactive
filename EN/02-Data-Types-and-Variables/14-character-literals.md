[slide]
# Character Literals
## Escaping Characters
- Escaping sequences are:
    - Represent a special character like ', " or \n (new line)
    - Represent system characters (like the [TAB] character \t)
- Commonly used escaping sequences are:
    - \\' -> for single quote	\" -> for double quote
    - \\ -> for backslash	\n -> for new line
    - \\uXXXX -> for denoting any other Unicode symbol


[/slide]

[slide]
# Character Literals – Example
```csharp
char symbol = 'a'; // An ordinary character
symbol = '\u006F'; // Unicode character code in a
                   // hexadecimal format (letter 'o')
symbol = '\u8449'; // 葉 (Leaf in Traditional Chinese)
symbol = '\''; // Assigning the single quote character
symbol = '\\'; // Assigning the backslash character
symbol = '\n'; // Assigning new line character
symbol = '\t'; // Assigning TAB character
symbol = "a";  // Incorrect: use single quotes!

```
[/slide]


