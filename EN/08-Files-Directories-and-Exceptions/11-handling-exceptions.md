[slide]
# Handling Exceptions
Exception handling is a mechanism, which allows exceptions to be **thrown** and **caught**. This mechanism is provided **internally** by the **CLR** (Common Language Runtime). Parts of the exception handling infrastructure are the language constructs in **C#** for throwing and catching exceptions. CLR takes care to propagate each exception to the code that can **handle** it.

## The try-catch Statement
- To **handle** an **exception**, we must **surround** the code that could throw an exception with a **try-catch block**:

```c#
try
{
    // Do some work that can cause an exception
}
catch
{
    // This block will execute if any type of exception occurs
}

```
[/slide]



[slide]
# The try-catch Statement(2)
```c#
try
{
    // Do some work that can cause an exception
}
catch(FormatException formatException)
{
    // This block will execute only if format exception occurs
}
```
[/slide]

[slide]
# The try-finally Statement
Every try block could contain a respective **finally block**. The code within the finally block is **always** executed, **no matter** how the program flow leaves the try block. This **guarantees** that the finally block will be **executed** even if an exception is thrown or a return statement is executed within the try block. 
The code in the finally block **will not be executed** if while executing the try block, CLR is **unexpectedly terminated**, e.g. if we stop the program through Windows Task Manager.
- The statement:
```c#
try
{
    // Do some work that can cause an exception
}
finally
{
    // This block will always execute
}

```
- Ensures execution of given block in all cases
    - When exception is raised or not in the try block
- Used for execution of cleaning-up code, e.g. releasing resources

```c#
try
{
    // Do some work that can cause an exception
}
catch(FileNotFoundException fileNotFoundEx)
{
   // This block will be executed only if file not found       exception occurs
}
finally
{
    // This block will always execute
}

```
[/slide]

[slide]
# Try it yourself!

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