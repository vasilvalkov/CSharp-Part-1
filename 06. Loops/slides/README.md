<!-- section start -->
<!-- attr: { id:'', class:'slide-title', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Loops
## Execute Blocks of Code Multiple Times
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic00.png" style="top:52.01%; left:58.48%; width:44.15%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic01.png" style="top:-1.96%; left:21.73%; width:20.77%; z-index:-1" /> -->
<div class="signature">
	<p class="signature-course"></p>
	<p class="signature-initiative"></p>
	<a href="" class="signature-link"></a>
</div>




<!-- section start -->
<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Table of Contents
- [What is a Loop?](#/whatisloop)
- [Loops in C#](#/1)
  - [**while** loops](#/while)
  - [**do** … **while** loops](#/dowhile)
  - [**for** loops](#/for)
  - [**foreach** loops](#/foreach)
- [Special loop operators](#/specialoperators)
  - [**break**, **continue**, **goto**](#/breakcontinue)
- [Nested loops](#/nestedloops)

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic02.png" style="top:19.39%; left:58.26%; width:42.96%; z-index:-1" /> -->

<!-- section start -->
<!-- attr: { id:'whatisloop', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# <a id="whatisloop"></a>What Is Loop?
- A **loop** is a control statement that allows repeating execution of a block of statements
  - May execute a code block fixed number of times
  - May execute a code block while given condition holds
  - May execute a code block for each member of a collection
- Loops that never end are called an **infiniteloops**




<!-- section start -->
<!-- attr: { id:'while', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# <a id="while"></a>WUsing while(…) Loop
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic03.png" style="top:48.48%; left:30%; width:45%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# How To Use While Loop?
- The simplest and most frequently used loop
- The repeat condition
  - Returns a boolean result of **true** or **false**
  - Also called **loop condition**

```cs
while (condition)
{
    statements;
}
```



<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# While Loop – How It Works?
- true
- condition
- statement
- false


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# While Loop – _Example_

```cs
int counter = 0;
while (counter < 10)
{
    Console.WriteLine("Number : {0}", counter);
    counter++;
}
```

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic04.png" style="top:43.82%; left:7.50%; width:91.13%; z-index:-1" /> -->



<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # While -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic05.png" style="top:40%; left:30%; width:40%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Sum 1..N – _Example_
- Calculate and print the sum of the first N natural numbers

```cs
Console.Write("n = ");
int n = int.Parse(Console.ReadLine());
int number = 1;
int sum = 1;
Console.Write("The sum 1");
while (number < n)
{
   number++;
   sum += number ;
   Console.Write("+{0}", number);
}
Console.WriteLine(" = {0}", sum);
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Calculating Sum 1..N
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic06.png" style="top:43.20%; left:28%; width:45%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Prime Number – _Example_
- Checking whether a number is prime or not

```cs
Console.Write("Enter a positive integer number: ");
string consoleArgument=Console.ReadLine();
uint number = uint.Parse(consoleArgument);
uint divider = 2;
uint maxDivider = (uint) Math.Sqrt(number);
bool prime = true;
while (prime && (divider <= maxDivider))
{
    if (number % divider == 0)
    {
        prime = false;        
    }
    divider++;
}
Console.WriteLine("Prime? {0}", prime);
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Checking Whether a Number Is Prime
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic07.png" style="top:44.96%; left:70.17%; width:28%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic08.png" style="top:44.96%; left:0%; width:35%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Using break Operator
- **break** operator exits the inner-most loop

```cs
static void Main()
{
    int n = Convert.ToInt32(Console.ReadLine());
    // Calculate n! = 1 * 2 * ... * n
    int result = 1;
    while (true)
    {
        if (n == 1)
            break;
        result *= n;
        n--;
    }
    Console.WriteLine("n! = " + result);
}
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Calculating Factorial
## Demo -->

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic09.png" style="top:40%; left:31.81%; width:44.08%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'dowhile', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# <a id="dowhile"></a>Wdo { … } while (…)Loop
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic10.png" style="top:40%; left:25%; width:50%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Using Do-While Loop
- Another loop structure is:
- The block of statements is repeated
  - While the boolean loop condition holds
- The loop is executed at least once

```cs
do
{
    statements;
}
while (condition);
```

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic11.png" style="top:15.13%; left:87.95%; width:18.55%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Do-While Statement
- true
- condition
- statement
- false




<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # do { … } while -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic12.png" style="top:38.92%; left:28%; width:40%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Factorial – _Example_
- Calculating N factorial

```cs
static void Main()
{
   string numberAsString = Console.ReadLine();
   int n = Convert.ToInt32(numberAsString);
   int factorial = 1;

   do
   {
      factorial *= n;
      n--;
   }
   while (n > 0);

   Console.WriteLine("n! = " + factorial);
}
```



<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Factorial with BigInteger – _Example_
- Calculating N factorial with **BigInteger**
<div class="fragment balloon" style="top:22.46%; left:54.66%; width:44.96%">Don't forget to add reference to System.Numerics.dll.</div>


<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Factorial (do ... while)
## Demo -->

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic13.png" style="top:40%; left:28.54%; width:40%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Product[N..M] – _Example_
- Calculating the product of all numbers in the interval [n..m]:

```cs
int n = int.Parse(Console.ReadLine());
int m = int.Parse(Console.ReadLine());
int number = n;
decimal product = 1;
do
{		
    product *= number;
    number++;
}
while (number <= m);
Console.WriteLine("product[n..m] = " + product);
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Product of the Numbers in the Interval [n..m]
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic14.png" style="top:55%; left:30%; width:35%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # for Loops -->

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic15.png" style="top:39.67%; left:15.91%; width:73.17%; z-index:-1" /> -->


<!-- attr: { id:'for', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# <a id="for"></a>WFor Loops
- The typical **for** loop syntax is:
- Consists of
  - Initialization statement
  - Boolean test expression
  - Update statement
  - Loop body block

```cs
for (initialization; test; update)
{
    statements;
}
```



<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# The Initialization Expression
- Executed once, just before the loop is entered
  - Like it is out of the loop, before it
- Usually used to declare a counter variable

```cs
for (int number = 0; ...; ...)
{
        // Can use number here
}
// Cannot use number here
```



<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# The Test Expression
- Evaluated before each iteration of the loop
  - If **true**, the loop body is executed
  - If **false**, the loop body is skipped
- Used as a **loop condition**

```cs
for (int number = 0; number < 10; ...)
{    
    // Can use number here
}
// Cannot use number here
```



<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# The Update Expression
- Executed at each iteration **after** the body of the loop is finished
- Usually used to update the counter

```cs
for (int number = 0; number < 10; number++)
{
       // Can use number here
}
// Cannot use number here
```


<!-- section start -->
<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # for Loop
## Demo -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic16.png" style="top:41.65%; left:28%; width:45%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Simple for Loop – _Example_
- A simple for-loop to print the numbers 0…9:

```cs
for (int number = 0; number < 10; number++)
{
    Console.Write(number + " ");
}
```

- A simple for-loop to calculate n!:

```cs
decimal factorial = 1;
for (int i = 1; i <= n; i++)
{
    factorial *= i;
}
```



<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Complex for Loop – _Example_
- Complex **for**-loops could have several counter variables:

```cs
for (int i=1, sum=1; i<=128; i=i*2, sum+=i)
{
    Console.WriteLine("i={0}, sum={1}", i, sum);
}
```
- Result:

```cs
i=1, sum=1
i=2, sum=3
i=4, sum=7
i=8, sum=15
...
```




<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # For Loops
## Demo -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic17.png" style="top:40%; left:35%; width:30%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# N^M – _Example_
- Calculating **n** to power **m** (denoted as **n^m**):

```cs
static void Main()
{
    int n = int.Parse(Console.ReadLine());
    int m = int.Parse(Console.ReadLine());
    decimal result = 1;
    for (int i=0; i<m; i++)
    {
        result *= n;
    }
    Console.WriteLine("n^m = " + result);
}
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Calculating N^M
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic18.png" style="top:40.08%; left:30%; width:40%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Using continue Operator
- **continue** operator ends the iteration of the inner-most loop
- _Example_: sum all odd numbers in [1, n] that are not divisors of 7:

```cs
int n = int.Parse(Console.ReadLine());
int sum = 0;
for (int i = 1; i <= n; i += 2)
{
   if (i % 7 == 0)
   {
      continue;
   }
   sum += i;
}
Console.WriteLine("sum = {0}", sum);
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Using continue Operator
## Demo -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic19.png" style="top:40%; left:30%; width:40%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # foreach Loop -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic20.png" style="top:40%; left:30%; width:40%; z-index:-1" /> -->


<!-- attr: { id:'foreach', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# <a id="foreach"></a>WForeach Loops
- The typical **foreach** loop syntax is:
- Iterates over all elements of a collection
  - The **element** is the loop variable that takes sequentially all collection values
  - The **collection** can be list, array or other group of elements of the same type

```cs
foreach (Type element in collection){    statements;}
```



<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# foreach Loop – _Example_
- _Example_ of **foreach** loop:

```cs
string[] days = {
  "Monday", "Tuesday", "Wednesday", "Thursday",
  "Friday", "Saturday", "Sunday" };
foreach (string day in days)
{
  Console.WriteLine(day);
}
```

- The above loop iterates of the array of days
  - The variable **day** takes all its values
- In the **foreach** loop we cannot set the value of the current item


<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # foreach Loop
## Demo -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic21.png" style="top:40%; left:33%; width:35%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Nested Loops -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic22.png" style="top:40.55%; left:36.02%; width:36.14%; z-index:-1" /> -->


<!-- attr: { id:'nestedloops', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# <a id="nestedloops"></a>WWhat Is Nested Loop?
- A composition of loops is called a **nested loop**
  - A loop inside another loop
- _Example_:

```cs
for (initialization; test; update)
{
    for (initialization; test; update)
    {			
        statements;
    }
    …
}
```

<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Nested Loops -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic23.png" style="top:38.79%; left:36.78%; width:34.55%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Triangle – _Example_
- Print the following triangle:
    - 1
    - 1 2
    - …
    - 1 2 3 ... n

```cs
int n = int.Parse(Console.ReadLine());
for(int row = 1; row <= n; row++)
{
   for(int column = 1; column <= row; column++)
   {
      Console.Write("{0} ", column);
   }
   Console.WriteLine();
}
```

<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Triangle
## Demo -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic24.png" style="top:39.67%; left:31.81%; width:44.08%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Primes[N, M] – _Example_
- Print all prime numbers in the interval [n, m]:

```cs
int n = int.Parse(Console.ReadLine());
int m = int.Parse(Console.ReadLine());
for (int number = n; number <= m; number++)
{
   bool prime = true;
   int divider = 2;
   int maxDivider = Math.Sqrt(num);
   while (divider <= maxDivider)
   {
      if (number % divider == 0)
      {
         prime = false;
         break;
      }
      divider++;
   }
   if (prime)
   {
      Console.Write("{0} ", number);
   }
}
```

<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Primes in Range [n, m]
## Demo -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic25.png" style="top:40.55%; left:30%; width:45%; z-index:-1" /> -->


<!-- attr: { id:'breakcontinue', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# <a id="breakcontinue"></a>WC# Jump Statements
- Jump statements are:
  - **break**, **continue**, **goto**
- How **continue** works?
  - In **while** and **do-while** loops jumps to the test expression
  - In **for** loops jumps to the update expression
- To exit an inner loop use **break**
- To exit outer loops use **goto** with a label
  - Avoid using **goto**! (it is considered harmful)


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# C# Jump Statements – _Example_

```cs
int outerCounter = 0;
for (int outer = 0; outer < 10; outer++)
{    for (int inner = 0; inner < 10; inner++)
    {        if (inner % 3 == 0)
            continue;        if (outer == 7)
            break;        if (inner + outer > 9)
            goto breakOut;    }
    outerCounter++;
}breakOut:
```

<div class="fragment balloon" style="top:51.11%; left:4.41%; width:14.93%">Label</div>


<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Loops – More _Examples_ -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic26.png" style="top:40%; left:30%; width:50%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Nested Loops – _Examples_
- Print all four digit numbers in format **ABCD** such that **A**+**B** = **C**+**D** (known as happy numbers)

```cs
static void Main()
{
  for (int a =1 ; a <= 9; a++)
    for (int b = 0; b <= 9; b++)
      for (int c = 0; c <= 9; c++)
        for (int d = 0; d <= 9; d++)
          if (a + b == c + d)
            Console.WriteLine("{0}{1}{2}{3}",
              a, b, c, d);
}
```

<div class="fragment balloon" style="top:27.98%; left:66.12%; width:34.99%">Can you improve this algorithm to use 3 loops only?</div>


<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Happy Numbers
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic27.png" style="top:43.20%; left:41.17%; width:26.45%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Nested Loops – _Examples_
- Print all combinations from TOTO 6/49

```cs
static void Main()
{		
  int i1, i2, i3, i4, i5, i6;
  for (i1 = 1; i1 <= 44; i1++)
    for (i2 = i1 + 1; i2 <= 45; i2++)
      for (i3 = i2 + 1; i3 <= 46; i3++)
        for (i4 = i3 + 1; i4 <= 47; i4++)
          for (i5 = i4 + 1; i5 <= 48; i5++)
            for (i6 = i5 + 1; i6 <= 49; i6++)
              Console.WriteLine("{0} {1} {2} {3} {4} {5}",
                i1, i2, i3, i4, i5, i6);
}		
```

<div class="fragment balloon" style="top:21.52%; left:67.00%; width:34.99%">Warning: execution of this code could take too long time.</div>


<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# TOTO 6/49
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic28.png" style="top:40%; left:24.33%; width:58.18%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Summary
- C# supports four types of loops:
  - **while**
  - **do-while**
  - **for** loops
  - **foreach** loops
- Nested loops can be used to implement more complex logic
- The operators **continue**, **break** & **goto** can control the loop execution

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic29.png" style="top:23.63%; left:74.85%; width:28.21%; z-index:-1" /> -->


<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
<!-- # Loops
## Questions? -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Free Trainings @ Telerik Academy
- Fundamentals of C# ProgrammingTrack of Courses
    - [csharpfundamentals.telerik.com](csharpfundamentals.telerik.com)
  - Telerik Software Academy
    - [academy.telerik.com](academy.telerik.com)
  - Telerik Academy @ Facebook
    - [facebook.com/TelerikAcademy](facebook.com/TelerikAcademy)
  - Telerik Academy Learning System
    - telerikacademy.com
    
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic30.png" style="top:58.18%; left:90.52%; width:16.97%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic31.png" style="top:34.35%; left:68.14%; width:36.30%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic32.png" style="top:48.92%; left:75.91%; width:10.85%; z-index:-1" /> -->
