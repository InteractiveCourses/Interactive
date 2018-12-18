[slide]
# Exceptions
Exception is a **notification** that something **interrupts** the normal program execution. Good programming practices require that the code returns **what is expected** or **throws an exception**. Exceptions provide a programming paradigm for detecting and reacting to **unexpected events**. Let’s assume the file is located on a remote server and during the process of reading it, the connection goes down. The file then will be only partially loaded. The program will not be able to execute normally and show file’s contents on the screen. In this case, we have an exception from the normal (and correct) program execution and this exception must be reported to the user and/or the administrator. When an exception arises, the state of the program is saved, the normal flow is interrupted and the control is passed to an **exception handler** (if such exists in the current context).
- The exceptions in .NET Framework is a powerful mechanism for centralized handling of errors and unusual events
- Simplify code construction and maintenance

[/slide]
[slide]
# The System.Exception Class
- The System.Exception class is base for all exceptions in .NET. Exception in .NET is an **object**, which signals an error or an event, which is not anticipated in the normal program flow.
    - Contains information for the cause of the error / unusual situation. When such unusual event takes place, the executing method ’throws' a special object containing information about the type of the error, the place in the program where the error occurred as well as the program state at the moment of the error.
        - **Message** – text description of the exception
        - **StackTrace** – the snapshot of the stack at the moment of exception throwing. Each exception in .NET contains the so-called stack trace, which gives information of where exactly the error occurred. This will be discussed in more details later in this chapter.

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


