[slide]
# Splitting Strings
One of the most flexible methods for working with strings is **Split(…)**. It allows us to split a string by a separator or an array of possible separators.
- To split a string by given separator(s) use the following method:

```csharp
string[] Split(params char[] separator)

```
    - Example:


```csharp
string listOfBeers = "Amstel, Zagorka, Tuborg, Becks.";
string[] beers = listOfBeers.Split(' ', ',', '.');

Console.WriteLine("Available beers are:");
foreach (string beer in beers)
{
    Console.WriteLine(beer);
}
```
## Try it yourself!

[code-task title="Try it yourself!" executionStrategy="csharp-dot-net-core-code" requiresInput]

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
Test your code.
[/task-description]

[code-io /]
[/code-task]

[/slide]


