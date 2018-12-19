[slide]
# Lambda Expressions

- A lambda expression is an anonymous function containing expressions and statements
- Lambda expressions use the lambda operator `=>`
    - Read as "goes to"
- The left side specifies the input parameters
- The right side holds the expression or statement  

[/slide]

[slide]
# Lambda Functions

**Lambda functions** are inline methods (functions) that take input parameters and return values:

| Lambda        | Method                                       |
|---------------|----------------------------------------------|
| `x => x / 2`  | `static int Func(int x) { return x / 2; }`   |
| `x => x != 0` | `static bool Func(int x) { return x != 0; }` |
| `() => 42`    | `static int Func() { return 42; }`           |

[/slide]

[slide]
# Filter Collections

Using `Where()`:

```csharp
int[] nums = { 1, 2, 3, 4, 5, 6};
nums = nums
       .Where(num => num % 2 == 0)
       .ToArray(); 

// nums = [2, 4, 6]
```

Using `Count()`:

```csharp
int[] nums = { 1, 2, 3, 4, 5, 6};
int count = nums.Count(num => num % 2 == 0); 
// count = 3
```

[/slide]

[slide]
# Filtering and Sorting with Lambda Functions

```csharp
int[] nums = { 11, 99, 33, 55, 77, 44, 66, 22, 88 };
nums.OrderBy(x => x).Take(3); 
// 11 22 33
nums.Where(x => x < 50);
// 11 33 44 22
nums.Count(x => x % 2 == 1); 
// 5
nums.Select(x => x * 2).Take(5); 
// 22 198 66 110 154
```

[/slide]

[slide]
# Getting Unique Elements from Collection

Using `Distinct()`:

```csharp
int[] nums = { 1, 2, 2, 3, 4, 5, 6, -2, 2, 0, 15, 3, 1, 0, 6};
nums = nums
        .Distinct()
        .ToArray(); 

// nums = [1, 2, 3, 4, 5, 6, -2, 0, 15]
```

[/slide]
