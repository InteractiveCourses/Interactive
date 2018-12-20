[slide]
# Exercises: Data Types and Variables

Problems for exercises and homework for the “Programming Fundamentals” course @ SoftUni.

You can check your solutions here:

[anchor href=https://judge.softuni.bg/Contests/206/Data-Types-and-Variables-Exercises]https://judge.softuni.bg/Contests/206/Data-Types-and-Variables-Exercises[/anchor]

## 1. Practice Integer Numbers

Create a new C\# project and create a program that **assigns integer values** to **variables**. Be sure that each **value** is stored in the **correct variable type** (try to find the most suitable variable type in order to save memory). Finally, you need to **print** all variables
to the console.

### Examples

+----------------------+----------------------+
| **Input**            | **Output**           |
+======================+======================+
| -100                 | -100                 |
|                      |                      |
| 128                  | 128                  |
|                      |                      |
| -3540                | -3540                |
|                      |                      |
| 64876                | 64876                |
|                      |                      |
| 2147483648           | 2147483648           |
|                      |                      |
| -1141583228          | -1141583228          |
|                      |                      |
| -1223372036854775808 | -1223372036854775808 |
+----------------------+----------------------+

### Hints

Follow the idea in the code below:

[image src=https://github.com/InteractiveCourses/Interactive/blob/master/assets/programming-fundamentals-data-types-and-variables-exercises-01.png alt="exercises01png" /]

## 2. Practice Floating Point Numbers
Create a new C\# project and create a program that **assigns floating
point values** to **variables**. Be sure that each **value** is stored
in the **correct variable type** (try to find the most suitable variable
type in order to save memory). Finally, you need to **print** all
variables to the console.

### Examples

+--------------------------------+--------------------------------+
| **Input**                      | **Output**                     |
+================================+================================+
| **3.141592653589793238**       | **3.141592653589793238**       |
|                                |                                |
| 1.60217657                     | 1.60217657                     |
|                                |                                |
| 7.8184261974584555216535342341 | 7.8184261974584555216535342341 |
+--------------------------------+--------------------------------+

### Hints

Just like at the previous problem, declare several variables of appropriate **floating-point data type**, assign the above listed values and **print** them.

## 3. Practice Characters and Strings

Create a new C\# project and create a program that **assigns character**
and **string values** to **variables**. Be sure that each **value** is
stored in the **correct variable**. Finally, you need to **print** all
variables to the console.

### Examples

+-------------------------+-------------------------+
| **Input**               | **Output**              |
+=========================+=========================+
| **Software University** | **Software University** |
|                         |                         |
| **B**                   | **B**                   |
|                         |                         |
| **y**                   | **y**                   |
|                         |                         |
| **e**                   | **e**                   |
|                         |                         |
| **I love programming**  | **I love programming**  |
+-------------------------+-------------------------+

### Hints

Like at the previous problem, declare variables of type **char** or
**sting**, assign the above values and **print** them.

## 4. Variable in Hexadecimal Format

Write a program that reads a number in **hexadecimal format** /(**0x\#\#**) convert it to **decimal format** and prints it.

### Examples
+-------------------------+-------------------------+
| **Input**               | **Output**              |
+=========================+=========================+
| **0xFE**                | **254**                 |
|                         |                         |
| **0x37**                | **55**                  |
|                         |                         |
| **0x10**                | **16**                  |
+-------------------------+-------------------------+

### Hints


- Use 
[anchor href=https://msdn.microsoft.com/en-us/library/1k20k614(v=vs.110).aspx]**Convert.ToInt32(string, 16)**[/anchor]
     

## 5. Boolean Variable

Write a program that reads a **string**, converts it to **Boolean** variable and **prints** "**Yes**" if the variable is **true** and "**No**" if the variable is **false**.

### Examples

+-------------------------+-------------------------+
| **Input**               | **Output**              |
+=========================+=========================+
| **True**                | **Yes**                 |
|                         |                         |
| **False**               | **No**                  |
+-------------------------+-------------------------+


### Hints

- Use 
[anchor href=https://msdn.microsoft.com/en-us/library/86hw82a3(v=vs.110).aspx]**Convert.ToBoolean(string)**[/anchor]


## 6. Strings and Objects

Declare two **string variables** and assign them with "**Hello**" and
"**World**". Declare an **object variable** and assign it with the
**concatenation** of the first two variables (mind adding an interval
between). Declare a third **string** variable and initialize it with the
value of the object variable (you should perform type **casting**).

### Examples

+-----------+-----------------+
| **Input** | **Output**      |
+===========+=================+
| **Hello** | **Hello World** |
|           |                 |
| **World** |                 |
+-----------+-----------------+



## 7. Exchange Variable Values

Declare two integer variables **a** and **b** and assign them with 5 and
10 and after that **exchange their values** by using some programming
logic. Print the variable values before and after the exchange, as shown
below:

### Examples

+-----------+------------+
| **Input** | **Output** |
+===========+============+
| 5         | Before:    |
|           |            |
| 10        | a = 5      |
|           |            |
|           | b = 10     |
|           |            |
|           | After:     |
|           |            |
|           | a = 10     |
|           |            |
|           | b = 5      |
+-----------+------------+

### Hints

You may use a **temporary variable** to remember the old value of **a**,
then assign the value of **b** to **a**, then assign the value of the
temporary variable to **b**.

## 8. Employee Data

A marketing company wants to keep record of its employees. Each record
would have the following characteristics:
- First name
- Last name
- Age (0\...100)
- Gender (**m** or **f**)
- Personal ID number (e.g. 8306112507)
- Unique employee number (27560000...27569999)

Declare the **variables** needed to keep the information for a single employee using appropriate primitive data types. Use descriptive names. **Print** the data at the console.

### Examples

+------------+----------------------------------+
| **Input**  | **Output**                       |
+============+==================================+
| Amanda     | First name: Amanda               |
|            |                                  |
| Jonson     | Last name: Jonson                |
|            |                                  |
| 27         | Age: 27                          |
|            |                                  |
| f          | Gender: f                        |
|            |                                  |
| 8306112507 | Personal ID: 8306112507          |
|            |                                  |
| 27563571   | Unique Employee number: 27563571 |
+------------+----------------------------------+

### Hints

[image src=https://github.com/InteractiveCourses/Interactive/blob/master/assets/programming-fundamentals-data-types-and-variables-exercises-02.png alt="picture02" /]

## 9. Reverse Characters


Write a program to ask the user for **3 letters** and print them in
**reversed order**.

### Examples

+-----------+------------+--+-----------+------------+--+-----------+------------+
| **Input** | **Output** |  | **Input** | **Output** |  | **Input** | **Output** |
+===========+============+==+===========+============+==+===========+============+
| **A**     | **CBA**    |  | **x**     | **zYx**    |  | **G**     | **ngG**    |
|           |            |  |           |            |  |           |            |
| **B**     |            |  | **Y**     |            |  | **g**     |            |
|           |            |  |           |            |  |           |            |
| **C**     |            |  | **z**     |            |  | **n**     |            |
+-----------+------------+--+-----------+------------+--+-----------+------------+

## 10. Centuries to Nanoseconds

Write program to enter an integer number of **centuries** and convert it to **years, days, hours, minutes, seconds, milliseconds, microseconds, nanoseconds**.

### Examples

[image src=https://github.com/InteractiveCourses/Interactive/blob/master/assets/DataTypesTable10-1.png alt="DataTypesTable10-1" /]

  
### Hints



-   Use an appropriate data type for every data conversion. Beware of
    **overflows**!

-   Assume that a year has **365.2422 days** at average [anchor href=https://en.wikipedia.org/wiki/Tropical_year] the Tropical year[/anchor].

## 11. Convert Speed Units

Create a program to ask the user for a **distance (in meters)** and the time taken (as three numbers: hours, minutes, seconds), and **print the speed**, in meters per second, kilometers per hour and miles per hour.

Assume 1 mile = 1609 meters.

### Input

- On first line you receive -- **distance in meters**

- On second -- **hours**

- On third -- **minutes**

- On fourth -- **seconds**

### Output


Every number in the output should be precise up to 6 digits after the
floating point

-   On first line -- speed in **meters per second** (m/s)

-   On second line -- speed in **kilometers per hour** (km/h)

-   On third line -- speed in **miles per hour** (mph)

### Examples

+-----------+---------------+--+-----------+--------------+--+------------+--------------+
| **Input** | **Output**    |  | **Input** | **Output**   |  | **Input**  | **Output**   |
+===========+===============+==+===========+==============+==+============+==============+
| **1000**  | **0.2732241** |  | **10000** | **8.130082** |  | **200000** | **26.66667** |
|           |               |  |           |              |  |            |              |
| **1**     | **0.9836066** |  | **0**     | **29.26829** |  | **2**      | **96**       |
|           |               |  |           |              |  |            |              |
| **1**     | **0.6113155** |  | **20**    | **18.19036** |  | **5**      | **59.66439** |
|           |               |  |           |              |  |            |              |
| **0**     |               |  | **30**    |              |  | **0**      |              |
+-----------+---------------+--+-----------+--------------+--+------------+--------------+

### Hints

-   Search in internet how to convert units.

-   The type **float** is big enough for the calculations.

## 12. Rectangle Properties

Create a program to calculate rectangle's **perimeter**, **area** and **diagonal** by given its **width** and **height**.

### Examples

+-----------+----------------------+--+-----------+----------------------+
| **Input** | **Output**           |  | **Input** | **Output**           |
+===========+======================+==+===========+======================+
| **10**    | **30**               |  | **22.1**  | **64.6**             |
|           |                      |  |           |                      |
| **5**     | **50**               |  | **10.2**  | **225.42**           |
|           |                      |  |           |                      |
|           | **11.1803398874989** |  |           | **24.3402958075698** |
+-----------+----------------------+--+-----------+----------------------+

### Hints


-   Use **Math.Sqrt()** to calculate square root for calculating the diagonal (c^2^ = a^2^ + b^2^). See

[anchor href=http://www.mathopenref.com/rectanglediagonals.html]http://www.mathopenref.com/rectanglediagonals.html[/anchor].

## 13. Vowel or Digit

Create a program to check if given symbol is **digit**, **vowel** or any
**other symbol**.

### Examples
[/slide]