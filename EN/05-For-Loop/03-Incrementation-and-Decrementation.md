# Incrementation and Decrementation

[slide]
# Definition
Our current knowledge allows us to increment the value of a number in the following way:
```csharp
int number = 5;
number = number + 1;

Console.WriteLine(number); // 6
```

or

```csharp
int number = 5;
number += 1;

Console.WriteLine(number); // 6
```

In this section we will learn how to achieve the same result and write less code. 
[/slide]

[slide]
# Video
[youtube-video videoId=Hxbz656Euyw /]
[/slide]

[slide]
# Increment and Decrement Operators
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

The case is the same for decrement operator (**--**) with the only difference that the value is decreased by 1.
[/slide]

[slide]
# Increment and Decrement Operators in For Loop
We can use increment and decrement operators in the iterator statement of the for loop. Let's go back to the loop which prints numbers from 1 to 5 and see how we can change the iterator statement using the increment operator.

```csharp
for(int i = 1; i <= 5; i++)
{
    Console.WriteLine(i);
}
```

When we run the program we can see that the same result.
[/slide]

[slide]
# Summary
[/slide]