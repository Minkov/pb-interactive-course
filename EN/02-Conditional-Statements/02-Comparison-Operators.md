[slide]
# Usage and Definition
Before we learn how to test a condition, we need to learn how to compare two variables. In the following section we will learn how to use the basic comparison operators in the C# language. They are important, because we use them to describe conditions in our conditional statements.
There are several comparisons operators in C#, which are used to compare pairs of integers, floating-point numbers, characters, strings and other types and the result of the operation is boolean:
| Operator   |      Action      |
|----------|:-------------:|
| == |  Equal to |
| != |    Not equal to   |
| > | Greater than |
| >= | Greater than or equal to |
| < | Less than |
| <= | Less than or equal to |
[/slide]

[slide]
# Example
Let's look at examples of using comparisons:
```cs
int weight = 700;
Console.WriteLine(weight >= 500); // True

char gender = 'm';
Console.WriteLine(gender <= 'f'); // False

double colorWaveLength = 1.630;
Console.WriteLine(colorWaveLength > 1.621); // True

int a = 5;
int b = 7;
bool condition = (b > a) && (a + b < a * b);
Console.WriteLine(condition); // True
```
[/slide]

[slide]
# Comparing Different Data Types

In C# several types of data that can be compared:
- numbers (int, float, double)
    - compared by size 
- char
    - compared by their lexicographical order
- string
- bool
    - strings and booleans can be compared **only for equality**

[/slide]