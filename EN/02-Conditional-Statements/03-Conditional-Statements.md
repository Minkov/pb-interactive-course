[slide]
# Conditional Statement "if"

The main format of the conditional statement "if" is as follows:
```csharp
if (boolean expression)
{
    // Body of the conditional statement;
}
```
- The boolean-expression have to return either ***true*** or ***false***.
- If the boolean-expression returns true, the statements inside the body of if ( inside {...} ) will be executed.
- If the boolean-expression returns false, the statements inside the body of if will be ignored.

[/slide]

[slide]
# Problem
[code-task title="Greater integer" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp] 

```
using System;

public class Program
{
    public static void Main()
    {
        int firstNumber = int.Parse(Console.ReadLine());
        int secondNumber = int.Parse(Console.ReadLine());
        // Write your code here
    }
}
```
[/code-editor]
[task-description]
Read two integers and exchange their values if the first one is greater than the second one and print the value of the bigger one in the following format: "The bigger number is: {biggerNumber}".
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]
# Solution

[code-task title="Greater integer" executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
public class Program
{
    public static void Main()
    {
        int firstNumber = int.Parse(Console.ReadLine());
        int secondNumber = int.Parse(Console.ReadLine());
        int biggerNumber = firstNumber;
        if (secondNumber > firstNumber)
        {
            biggerNumber = secondNumber;
        }

        Console.WriteLine("The bigger number is: {0}", biggerNumber);
    }
}
```
[/code-editor]
[task-description]
Read two integers and exchange their values if the first one is greater than the second one and print the value of the bigger one in the following format: "The bigger number is: {biggerNumber}".
[/task-description]
[code-io /]
[/code-task]
[/slide]

[slide]

# Conditional Statement "if" and Curly Brackets

If we have only one operator in the body of the if-statement, the curly brackets denoting the body of the conditional operator may be omitted, as shown below:
```csharp
int a = 6;
if (a > 5)
    Console.WriteLine("The variable is greater than 5.");
```

However, it is a good practice to use them even if we have only one operator. This will make the code ***more readable***.
[/slide]

[slide]
# Conditional Statement "if-else"

The if statement in C# may have an optional else statement. The block of code inside the else statement will be executed **if the expression is evaluated to false**.

The syntax of if...else statement in C# is:
```csharp
if (boolean expression)
{
   // statements executed if boolean-expression is true
}
else
{
   // statements executed if boolean-expression is false
}
```

[/slide]

[slide]
# Example

```csharp
int number = int.Parse(Console.ReadLine());
if (number < 5)
{
	number = number + 5;
}
else
{
	number = number - 5;
}
```

In this example, the statement
```cs
number = number + 5;
```

will be executed only if the value of number is less than 5. 

The statement
```cs
number = number - 5;
```

will be executed if the value of number is greater than or equal to 5.
[/slide]