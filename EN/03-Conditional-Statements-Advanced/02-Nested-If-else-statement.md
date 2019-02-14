[slide]
# Usage and Definition
An if...else statement can exist within another if...else statement. Such statements are called nested if...else statement.

The general structure of nested if…else statement is:
```cs
if (boolean-expression)
{
	if (nested-expression-1)
	{
		// code to be executed
	}
	else
	{
	    // code to be executed
	}
}
else
{
	if (nested-expression-2)
	{
		// code to be executed
	}
	else
	{
		// code to be executed
	}
}
```
Nested if statements are generally used when we have to test one condition followed by another. In a nested if statement, ***if the outer if statement returns true***, it ***enters the body to check the inner if statement***.

It’s not a good practice to exceed ***three nested levels***, i.e. we should not nest more than three conditional statements into one another.
[/slide]


[slide]
# Problem

[code-task title="Read 3 integers and sort them in descending order." executionStrategy="csharp-dot-net-core-code" requiresInput]
[code-editor language=csharp]
```
using System;
class Program
{
    static void Main(string[] args)
    {
        int first = int.Parse(Console.ReadLine());
        int second = int.Parse(Console.ReadLine());
        int third = int.Parse(Console.ReadLine());
        if (first > second)
        {
            if (first > third)
            {
                Console.WriteLine("{0} is the largest", first);
            }
            else
            {
                Console.WriteLine("{0} is the largest", third);
            }
        }
        else
        {
            if (second > third)
            {
                Console.WriteLine("{0} is the largest", second);
            }
            else
            {
                Console.WriteLine("{0} is the largest", third);
            }
        }
    }
}
```
[/code-editor]
[task-description]
Read 3 integers and sort them in descending order.
[/task-description]
[code-io /]
[/code-task]
[/slide]