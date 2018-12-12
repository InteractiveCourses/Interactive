[slide]
# Simple Methods

- **Methods** are **named pieces of code** that can be invoked later
- Sample method **definition**:

```csharp
static void PrintHeader()
{
  Console.WriteLine("----------");
}
```

- **Invoking** (calling) the method several times:

```csharp
PrintHeader();
PrintHeader();
```
[/slide]

[slide]
# Why Use Methods?

- More **managable programming**
    - Splits large problems into small pieces
    - Better organization of the program
    - Improves code readability
    - Improves code understandability
- Avoiding repeating code
    - Improves code maintainability
- Code reusability
    - Using existing methods several times
[/slide]

[slide]
# Defining Methods

Method definitions follow this general structure:

```
[modifiers] [return type] [Name]([parameters])
{
  [method body]
}
```

For example:

```csharp
static double GetSquare(double num)
{
  return num * num;
}
```

- Methods are defined **inside a class**
- `Main()` is also a method:

```csharp
class Program
{
  static void Main(string[] args)
  {
    // code
  }
}
```

- Variables inside a method are **local**
[/slide]

[slide]
# Invoking a Method

- Methods are first **defined**, then **invoked** (many times); here's a method definition:

```csharp
static void PrintHeader()
{
  Console.WriteLine("----------");
}
```

- Methods can be invoked (called) by their name + `()`:

```csharp
static void Main()
{
  PrintHeader(); // <-- method invocation
}
```
[/slide]

[slide]
# Invoking a Method (2)

A method can be invoked from:

- The main method - `Main()`:

```csharp
static void Main()
{
  PrintHeader();
}
```

- Some other method:

```csharp
static void PrintHeader()
{
  PrintHeaderTop();
  PrintHeaderBottom();
}
```

- Its own body (recursion)

```csharp
static void Crash()
{
  Crash();
}
```
[/slide]