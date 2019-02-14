[slide]
# Logical operators
Logical operators are used to perform logical operation such as and, or. Logical operators operates on boolean expressions (true and false) and returns boolean values. Logical operators are used in decision making and loops which will cover later in the course.
[/slide]
[slide]
# The basic Boolean operators are:
- "AND" (&&)
- "OR" (||)
- "exclusive OR" (^)
- logical negation (!)
[/slide]
[slide]
# Logical operators table
The following table contains the logical operators in C# and the operations that they perform:
| x | y | !x | x AND y | x &#124;&#124; y  | x && y |
|---|---|---|---|---|---|
| true | true | false | true | true | false |
| true | false | false | false | true | true |
| false | true | true | false | true | true |
| false | false | true | false | false | false |
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
        int firstNumber = 10;
        int secondNumber = 20;

        Console.WriteLine((firstNumber == secondNumber) || (firstNumber > 5)); // the result will be true
        Console.WriteLine((firstNumber == secondNumber) && (firstNumber > 5)); // the result will be false
    }
}
```
[/code-editor]
[task-description]
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Problem
[code-task title="Greeting by given time" executionStrategy="csharp-dot-net-core-code"]
[code-editor language=csharp]
```
using System;
class Program
{
    static void Main(string[] args)
    {
        int time = int.Parse(Console.ReadLine());

        if (time >= 5 && time < 12)
        {
            Console.WriteLine("Good Morning");
        }
        else if (time >= 12 && time < 17)
        {
            Console.WriteLine("Good Afternoon");
        }
        else
        {
            Console.WriteLine("Good Evening");
        }
    }
}
```
[/code-editor]
[task-description]
Write a program which prints greeting by given time.
- from 5 (inclusive) to 12 (exclusive) - Good Morning
- from 12 (inclusive) to 17 (exclusive) - Good Afternoon
- from 17 (inclusive) to 5 (exclusive) - Good Evening
[/task-description]
[code-io /]
[/code-task]
[/slide]
