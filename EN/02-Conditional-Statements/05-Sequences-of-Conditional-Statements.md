[slide]
# Sequences of "if-else-if-else"

When we have only one condition to test, if-then and if-then-else statement works fine. But what if we have a multiple condition to test and execute one of the many block of code.

For such case, we can use **if..else if** statement in C#. The syntax for if...else if statement is:
```csharp
if (boolean-expression-1)
{
	statements executed if boolean-expression-1 is true
}
else if (boolean-expression-2)
{
	statements executed if boolean-expression-2 is true
}
else if (boolean-expression-3)
{
	statements executed if boolean-expression-3 is true
}
else
{
	statements executed if all above expressions are false
}
```

The if...else if statement is executed from the top to bottom. As soon as a test expression is true, the code inside of that if (or else if) block is executed. If none of the expression is true, the code inside the else block is executed.

[/slide]

[slide]

# Problem

[code-task title="Tickets Price" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp] 
```
using System;

public class Program
{
    public static void Main()
    {
        string ticketType = Console.ReadLine();
        // Write your code here
    }
}
```
[/code-editor]
[task-description]
The public transport tickets have different prices based on the age of the traveler as it follows:
| Type   |      Price      |
|----------|:-------------:|
| student |  1.00 |
| retiree |    0.80   |
| regular | 1.60 |
The task is to print the ticket price by given ticket type in the following format: "The price for a ticket is {ticketPrice}$". 
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]

# Solution

[code-task title="Tickets Price" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;

public class Program
{
    public static void Main()
    {
        string ticketType = Console.ReadLine();
        if (ticketType == "student")
        {
            Console.WriteLine("The price for a ticket is 1.00$");
        }
        else if (ticketType == "retiree")
        {
            Console.WriteLine("The price for a ticket is 0.80$");
        }
        else if (ticketType == "regular")
        {
            Console.WriteLine("The price for a ticket is 1.60$");
        }
        else
        {
            Console.WriteLine("Invalid ticket type!");
        }
    }
}
```
[/code-editor]
[task-description]
The public transport tickets have different prices based on the age of the traveler as it follows:
| Type   |      Price      |
|----------|:-------------:|
| student |  1.00 |
| retiree |    0.80   |
| regular | 1.60 |

The task is to print the ticket price by given ticket type in the following format: "The price for a ticket is {ticketPrice}$".
[/task-description]
[code-io /]
[/code-task]
[/slide]