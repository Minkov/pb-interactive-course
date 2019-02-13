# For-Loop

## Objective
After this lesson students will know how to work with ***for loop***.

## Motivation
In programming, it is often desired to **execute certain block of statements for a specified number of times**. A possible solution will be to type those statements for the required number of times. However, the number of repetition may not be known in advance or maybe large enough (say 10000). The best solution to such problem is ***for loop***.

## Content

### Introduction
In this lesson will learn how to execute certain block of statements for a **specified number of times**.

### Sections

#### For Definition
The **for** keyword is used to create for loop in C#. The syntax for **for loop** is:
```csharp
for (initialization; condition; iterator)
{
	// body of for loop
}
```
##### Initialization
Executed at first and only once. Here, the variable is usually declared and initialized

##### Condition
Boolean expression, i.e. it returns either ***true*** or ***false***.
    - If the condition is evaluated to true the statements inside the for loop are executed, then, the iterator statement is executed which usually changes the value of the initialized variable and finally the condition is evaluated again.
    - If the condition is evaluated to false, the for loop ***terminates***.

##### Iterator
Executed at each iteration, after the loop's body has been executed. It is most commonly used to update the value of the counter-variable.

##### The Body of the Loop
The body of the loop contains a block with source code. The loop variables, declared in the initialization block of the loop are available in it. The body is executed at each iteration.

##### Simple For Loop Example
```csharp
for (int i = 1; i <= 5; i += 1)
{
    Console.WriteLine(i);
}
```

When we run the program, the output will be:
```
1
2
3
4
5
```

In this program:
- initialization statement is int i = 1
- condition statement is i <= 5
- iterator statement is i += 1
    - The iterator statement could be anything that updates the initialized variable, but the actual result will be different. For example:
        - i += 2;
        - i += 3;
        - i += 5; 

When the program runs:
- First, the variable i is declared and initialized to 1.
- Then, the condition (i <= 5) is evaluated.
- Since, the condition returns **true**, the program then **executes** the body of the for loop. It prints the given line with Iteration 1.
- Now, the iterator (i += 1) is evaluated. This **increments the value of i to 2**.
- The condition (i <=5 ) is evaluated again. The condition will evaluate to **true** for the **first 5 times**.
- When the value of i will be 6 and the condition will be **false**, hence the loop will **terminate**.

**Problem: Calculate the sum of first *n* natural numbers.**
```csharp
int n = int.Parse(Console.ReadLine());
int sum = 0;

for (int i = 1; i <= n; i += 1)
{
    sum += i;
}

Console.WriteLine($"Sum: {sum}");
```

When we run the program and enter 6, the output will be:
```
Sum: 21
```

Here, the value of sum and n are initialized to 0 and 6 respectively. The iteration variable i is initialized to 1 and incremented on each iteration.

Let's see what happens in the given program on each iteration:

| Iteration | Value of i | i <= 6 | sum |
|---|---|---|---|
| 1 | 1 | true | 0 + 1 = 1 |
| 2 | 2 | true | 1 + 2 = 3 |
| 3 | 3 | true | 3 + 3 = 6 |
| 4 | 4 | true | 6 + 4 = 10  |
| 5 | 5 | true | 10 + 5 = 15 |
| 6 | 6 | true | 15 + 6 = 21 |
| 7 | 7 |  false | Loop terminates |

So, the final value of sum will be 21 when n = 6.

#### Incrementation and Decrementation

##### Increment and Decrement operators
Our current knowledge allows us to increment the value of a number in the following way:
```csharp
int number = 5;
number = number + 10;

Console.WriteLine(number); // 15
```

or

```csharp
int number = 5;
number += 10;

Console.WriteLine(number); // 15
```

In C#, we have (**++**) and decrement (**--**) operators which can be used to increase or decrease the value of a number by **1**.

For instance:

```csharp
int number = 5;
number++;
Console.WriteLine(number); // 6

number--;
Console.WriteLine(number); // 5
```

The operators can be used as prefix and postfix.If used as prefix, the change in value of variable is seen on the same line and if used as postfix, the change in value of variable is seen on the next line. This will be clear by the example below:

```csharp
int number = 5;

Console.WriteLine(number++); // 5
Console.WriteLine(number); // 6

Console.WriteLine(++number); // 7
Console.WriteLine(number); // 7
```

The case is same for decrement operator (**--**).

##### Operators in for loop
We can use increment and decrement operators in the iterator statement of the for loop. Let's go back to the loop which prints numbers from 1 to 5 and see how we can change the iterator statement using the increment operator.

```csharp
for(int i = 1; i <= 5; i++)
{
    Console.WriteLine(i);
}
```

When we run the program we can see that the result is same.

#### Decreasing For Loop
How we can print numbers from 10 to 5 inclusive with current knowledge?

```csharp
int startingNumber = 10;
for (int i = 0; i <= 5; i++)
{
    int currentNumber = startingNumber - i;
    Console.WriteLine(currentNumber);
}
```

We can use decreasing for loop to simplify the code from the previous example. Decreasing for loop is a for loop which starts from given value and the loop is executed until the value is greater or equal to another value. After all, we have a loop which is executed for a specified number of times.

```csharp
for (int i = 10; i >= 5; i--)
{
    Console.WriteLine(i);
}
```

#### Infinite For loop
If the condition in a for loop is always true, for loop will run forever. This is called **infinite loop**.
```cs
for (int i = 1 ; i > 0; i++)
{
    Console.WriteLine("Iteration {0}", i);
}
```

Here, **i** is initialized to 1 and the condition is **i > 0**. On each iteration we are incrementing the value of i by 1, so the condition will never be false. This will cause the loop to execute **infinitely**.

We can also create an infinite loop by replacing the condition with a blank. For example:
```csharp
for ( ; ; )
{
	// body of for loop
}
```

or 

```csharp
for (initialization ; ; iterator)
{
	// body of for loop
}
```

Using an infinite loop is **rarely needed** and should be **avoided**.
### Conclusion & Summary

## Resources
- [Programiz](https://www.programiz.com/csharp-programming/for-loop)
- [for (C# reference)](https://docs.microsoft.com/en-us/dotnet/csharp/language-reference/keywords/for)
- [Fundamentals of Computer Programing with C# - Conditional Statements](https://introprogramming.info/english-intro-csharp-book/read-online/chapter-6-loops/)


## Exercise
- Write a program that prints on the console the numbers from 1 to N. The number N should be read from the standard input.
- Write a program that prints on the console the numbers from 1 to N, which are not divisible by 3 and 7 simultaneously. The number N should be read from the standard input.
- Write a program that reads from the console a series of integers and prints the smallest and largest of them.
- Write a program that finds factorial of an integer entered by user.

## Evaluation & Exam