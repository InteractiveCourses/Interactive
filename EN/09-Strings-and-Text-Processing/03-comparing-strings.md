[slide]
# Manipulating Strings

## Comparing Strings
- Several ways to compare two strings:
    - Dictionary-based string comparison. If you want to compare two words and get information which one of them is before the other according to their alphabetical order of letters, here comes the method CompareTo(…). It allows us to compare the values of two strings in order to determine their lexicographical order. In order two strings to have the same values, they must have the same length (number of characters) and the all their characters should match accordingly.
        - Case-insensitive

```csharp
int result = string.Compare(str1, str2, true);
// result == 0 if str1 equals str2
// result < 0 if str1 is before str2
// result > 0 if str1 is after str2	
```
        - Case-sensitive

```csharp
int result = string.Compare(str1, str2, false);
```


## Try it yourself!

[/slide]

[slide]
## Comparing Strings (2)
In the C# language the operators == and =! work for strings through an internal calling of Equals(…).
- Equality checking by operator ==
    - Performs case-sensitive comparison
```csharp
if (str1 == str2)
{
    …
}	
```
- Using the case-sensitive Equals() method
    - The same effect like the operator ==
```csharp
if (str1.Equals(str2))
{
    …
}	
```

[/slide]

[slide]
# Problem: Refactor Special Numbers


Try it yourself here: 

[/slide]


