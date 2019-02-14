[slide]
# Conditional Statement "switch-case"
In the following section we will cover the conditional statement ***switch***. It is used for choosing among a list of possibilities. The switch statement is often used as an alternative to an if-else construct ***if a single expression is tested against three or more conditions***.

Let’s take a look at an example of ***switch***:
[/slide]
[slide]
# Example
[code-task title="Example" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
class Program
{
    static void Main(string[] args)
    {
        switch (selector)
        {
            case value_1:
                statements;
                break;
            case value_2:
                statements;
                break;
            default:
                statements;
                break;
        }
    }
}
```
[/code-editor]
[task-description]
[/task-description]
[code-io /]
[/code-task]

The selector must be a value of the following types:
[slide]
# Char
[/slide]
[slide]
# String
[/slide]
[slide]
# Bool
[/slide]
[slide]
# Integer
[/slide]
[/slide]

[slide]
# Problem
[code-task title="From 1 to 7" executionStrategy="csharp-dot-net-core-code"
requiresInput]
[code-editor language=csharp]
```
using System;
class Program
{
    static void Main(string[] args)
    {
        int day = int.Parse(Console.ReadLine());
        switch (day)
        {
            case 1:
                Console.WriteLine("Monday");
                break;
            case 2:
                Console.WriteLine("Tuesday");
                break;
            case 3:
                Console.WriteLine("Wednesday");
                break;
            case 4:
                Console.WriteLine("Thursday");
                break;
            case 5:
                Console.WriteLine("Friday");
                break;
            case 6:
                Console.WriteLine("Saturday");
                break;
            case 7:
                Console.WriteLine("Sunday");
                break;
            default:
                Console.WriteLine("Error!");
                break;
        }
    }
}
```
[/code-editor]
[task-description]
Write a program, which reads an integer from the console and prints the day of week in text form according to the input [1… 7]. If the number is not in the range prints **"Error!"**
[/task-description]
[code-io /]
[/code-task]
[slide]