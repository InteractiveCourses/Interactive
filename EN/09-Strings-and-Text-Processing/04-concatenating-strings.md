[slide]
# Concatenating Strings
- Gluing two strings and obtaining a new one as a result is called concatenation. It could be done in several ways: through the method Concat(…) or with the operators + and +=. Please note that string concatenation does not change the existing strings but returns a new string as a result. If we try to concatenate two strings without storing them in a variable, the changes would not be saved.
- 
    - Using the Concat() method

```csharp
string str = string.Concat(str1, str2); 
```
    - Using the + or the += operators
```csharp
string str = str1 + str2 + str3;
string str += str1;
```
- Any object can be appended to a string

```csharp
string name = "Peter";
int age = 22;
string s = name + " " + age; //  "Peter 22"
```

## Try it yourself!

[/slide]



