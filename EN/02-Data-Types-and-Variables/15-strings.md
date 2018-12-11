[slide]
# The String Data Type
Strings are sequences of characters. In C# they are declared by the keyword string. Their default value is null. Strings are enclosed in quotation marks. Various text-processing operations can be performed using strings: concatenation (joining one string with another), splitting by a given separator, searching, replacement of characters and others. 
- The string data type:
    - Represents a sequence of characters
    - Is declared by the string keyword
    - Has a default value null (no value)
- Strings are enclosed in quotes:
```csharp
string s = "Hello, C#";
```

- Strings can be concatenated
    - Using the + operator

[/slide]

[slide]
# Verbatim and Interpolated Strings
- Strings are enclosed in quotes "":

```csharp
string file = "C:\\Windows\\win.ini";

```
- Strings can be verbatim (no escaping):
```csharp
string file = @"C:\Windows\win.ini";

```
- Interpolated strings insert variable values by pattern:
```csharp
string firstName = "Svetlin";
string lastName = "Nakov";
string fullName = $"{firstName} {lastName}";
```

[/slide]

[slide]
# Saying Hello – Examples
- Combining the names of a person to obtain the full name:
```csharp
string firstName = "Ivan";
string lastName = "Ivanov";
Console.WriteLine(@"Hello, ""{0}""!", firstName);
string fullName = $"{firstName} {lastName}";
Console.WriteLine("Your full name is {0}.", fullName);
```
- We can concatenate strings and numbers by the + operator:

```csharp
int age = 21;
Console.WriteLine("Hello, I am " + age + " years old");

```
[/slide]

[slide]
# Problem: Greeting by Name and Age
- Write a program that enters first name, last name and age and prints "Hello, <first name> <last name>. You are <age> years old."

```csharp
string firstName = Console.ReadLine();
string lastName = Console.ReadLine();
string ageStr = Console.ReadLine();
int age = int.Parse(ageStr); // Parse string  int
Console.WriteLine($"Hello, {firstName} {lastName}.\r\nYou are {age} years old.");
```
Check your solution here: 
[/slide]



