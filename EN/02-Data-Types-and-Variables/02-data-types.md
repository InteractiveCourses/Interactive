[slide]
# Data Types
## How Computing Works?
- Computers are machines that process data
- Instructions and data are stored in the computer memory
[/slide]

[slide]
# Variables
A typical program uses various values that change during its execution. For example, we create a program that performs some calculations on the values that user enters in. The values entered by one user will obviously be different from those entered in by another user. 
1. Variables have name, data type and value
    - Assignment is done by the operator "=" 
    - Example of variable definition and assignment in C#
2. When processed, data is stored back into variables

[/slide]

[slide]
# What Is a Data Type?
Data types are sets (ranges) of values that have similar characteristics. For instance byte type specifies the set of integers in the range [0 … 255].

- A data type: 
    - Is a domain of values of similar characteristics
    - Defines the type of information stored in the computer memory (in a variable)

- Basic data types in C# are distributed into the following types:
    - Integer types – sbyte, byte, short, ushort, int, uint, long, ulong;
    - Real floating-point types – float, double;
    - Real type with decimal precision – decimal;
    - Boolean type – bool;
    - Character type – char;
    - String – string;
    - Object type – object.  

- Examples:
    - Positive integers: 1, 2, 3, …
    - Alphabetical characters: a, b, c, …
    - Days of week: Monday, Tuesday, …
[/slide]


[slide]
# Data Type Characteristics
- A data type has:
    - Name (C# keyword or .NET type), can be any of our choice but must follow certain rules defined in the C# language specification:
        - Variable names can contain the letters a-z, A-Z, the digits 0-9 as well as the character '_'
        - Variable names cannot start with a digit
        - Variable names cannot coincide with a keyword of the C# language. For example, base, char, default, int, object, this, null and many others cannot be used as variable names
    - Size (how much memory is used) – for example, 4 bytes
    - Default value
- Example:
    - Integer numbers in C#
    - Name: int
    - Size: 32 bits (4 bytes)
    - Default value: 0
[/slide]
