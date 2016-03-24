<!-- section start -->
<!-- attr: { id:'', class:'slide-title', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Primitive DataTypes and Variables
## Integer, Floating-Point, Text Data, Variables, Literals
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic00.png" style="top:50.52%; left:59.88%; width:44.96%; z-index:-1" /> -->
<div class="signature">
	<p class="signature-course"></p>
	<p class="signature-initiative"></p>
	<a href="" class="signature-link"></a>
</div>




<!-- section start -->
<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 40px' } -->
# Table of Contents
- [Primitive Data Types](#primitive)
  - [Integer](#integer)
  - [Floating-Point / Decimal Floating-Point](#float)
  - [Boolean](#bool)
  - [Character](#char)
  - [String](#string)
  - [Object](#object)
- [Declaring and Using Variables](#declaring)
  - [Identifiers](#identifiers)
  - [Declaring Variables and Assigning Values](#assign)
  - [Literals](#literals)
- [Nullable Types](#nullable)
- [Dynamic Types](#dynamic)

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic01.png" style="top:33.50%; left:75.79%; width:28.21%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'primitive', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# <a id="primitive"></a>Primitive Data Types
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic02.png" style="top:41.08%; left:67.11%; width:35.41%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic03.png" style="top:41.08%; left:7.22%; width:52.01%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# How Computing Works?
- Computers are machines that process data
  - Data is stored in the computer memory in **variables**
  - Variables have **name**, **data type** and **value**
- _Example_ of variable definition and assignment in C#

```cs
int count = 5;
```

<div class="fragment balloon" style="top:61.75%; left:0%; width:22.04%">Data type</div>
<div class="fragment balloon" style="top:50%; left:10%; width:38.79%">Variable name</div>
<div class="fragment balloon" style="top:55%; left:27%; width:35.26%">Variable value</div>


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# What Is a Data Type?
- A **data type**:
  - Is a domain of values of similar characteristics
  - Defines the type of information stored in the computer memory (in a variable)
- _Examples_:
  - Positive integers: **1**, **2**, **3**, **…**
  - Alphabetical characters: **a**, **b**, **c**, **…**
  - Days of week: **Monday**, **Tuesday**, **…**

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic04.png" style="top:48.55%; left:86.08%; width:18.51%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Data Type Characteristics
- A data type has:
  - Name (C# keyword or .NET type)
  - Size (how much memory is used)
  - Default value
- _Example_:
  - Integer numbers in C#
  - Name: **int**
  - Size: 32 bits (4 bytes)
  - Default value: **0**

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic05.png" style="top:40.99%; left:90.76%; width:14.10%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'integer', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# <a id="integer"></a>Integer Types
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic06.png" style="top:42%; left:26.81%; width:50.38%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# What are Integer Types?
- Integer types:
  - Represent whole numbers
  - May be signed or unsigned
  - Have range of values, depending on the size of memory used
- The default value of integer types is:
  - **0** – for integer types, except
  - **0L** – for the **long** type

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic07.png" style="top:56.42%; left:77.66%; width:28.21%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Integer Types
- Integer types are:
  - **sbyte** (-128 to 127): signed 8-bit
  - **byte** (0 to 255): unsigned 8-bit
  - **short** (-32,768 to 32,767): signed 16-bit
  - **ushort** (0 to 65,535): unsigned 16-bit
  - **int** (-2,147,483,648 to 2,147,483,647): signed 32-bit
  - **uint** (0 to 4,294,967,295): unsigned 32-bit


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Integer Types -->
- More integer types:
  - **long** (-9,223,372,036,854,775,808 to 9,223,372,036,854,775,807): signed 64-bit
  - **ulong** (0 to 18,446,744,073,709,551,615): unsigned 64-bit

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic08.png" style="top:46.72%; left:60.82%; width:43.20%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Measuring Time – _Example_
- Depending on the unit of measure we may use different data types:

```cs
byte centuries = 20;    // Usually a small number
ushort years = 2000;
uint days = 730480;
ulong hours = 17531520; // May be a very big number
Console.WriteLine("{0} centuries is {1} years, or {2} days,
or {3} hours.", centuries, years, days, hours);
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Integer Types
## [Demo]() -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic09.png" style="top:40.55%; left:67.37%; width:36.80%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'float', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# <a id="float"></a>Floating-Point and Decimal Floating-Point Types
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic10.png" style="top:52.43%; left:30.88%; width:47.15%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# What are Floating-Point Types?
- **Floating-point** types:
  - Represent real numbers
  - May be signed or unsigned
  - Have range of values and different **precision** depending on the size of memory used
  - Can behave abnormally in the calculations

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic11.png" style="top:59.06%; left:13.10%; width:40%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Floating-Point Types
- Floating-point types are:
  - **float** (±1.5 × 10−45 to ±3.4 × 1038): 32-bits, precision of 7 digits
  - **double** (±5.0 × 10−324 to ±1.7 × 10308): 64-bits, precision of 15-16 digits
- The default value of floating-point types:
  - Is **0.0F** for the **float** type
  - Is **0.0D** for the **double** type


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# PI Precision – _Example_
- See below the difference in precision when using **float** and **double**:
- _Note_: The “**f**” suffix in the first statement!
  - Real numbers are by default interpreted as **double**!
  - One should **explicitly** convert them to **float**

```cs
float floatPI = 3.141592653589793238f;
double doublePI = 3.141592653589793238;
Console.WriteLine("Float PI is: {0}", floatPI);
Console.WriteLine("Double PI is: {0}", doublePI);
```

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic12.png" style="top:75%; left:43.41%; width:41.98%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Abnormalities in the Floating-Point Calculations
- Sometimes abnormalities can be observed when using floating-point numbers
  - Comparing floating-point numbers can not be performed directly with the **==** operator
- _Example_:

```cs
double a = 1.0f;
double b = 0.33f;
double sum = 1.33f;
bool equal = (a+b == sum); // False!!!
Console.WriteLine("a+b={0}  sum={1}  equal={2}",
    a+b, sum, equal);
```

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic13.png" style="top:40.55%; left:83.27%; width:22.04%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Decimal Floating-Point Types
- There is a special decimal floating-point		 real number type in C#:
  - **decimal** (±1,0 × 10-28 to ±7,9 × 1028): 128-bits, precision of 28-29 digits
  - Used for financial calculations
  - No round-off errors
  - Almost no loss of precision
- The default value of **decimal** type is:
  - **0.0M** (**M** is the suffix for decimal numbers)

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic14.png" style="top:13.66%; left:95.44%; width:11.02%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic15.png" style="top:37.87%; left:78.60%; width:25.86%; z-index:-1" /> -->


<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Floating-Point and Decimal Floating-Point Types
## [Demo]() -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic16.png" style="top:50%; left:70%; width:35%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'bool', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# <a id="bool"></a>Boolean Type
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic17.png" style="top:42.31%; left:53.33%; width:46.72%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic18.png" style="top:42.31%; left:14.03%; width:24.68%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# The Boolean Data Type
- The **Booleandata type**:
  - Is declared by the **bool** keyword
  - Has two possible values: **true** and **false**
  - Is useful in logical expressions
- The default value is **false**

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic19.png" style="top:43.20%; left:70.17%; width:34.71%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Boolean Values – _Example_
- _Example_ of boolean variables taking values of **true** or **false**:

```cs
int a = 1;
int b = 2;
bool greaterAB = (a > b);
Console.WriteLine(greaterAB);  // False
bool equalA1 = (a == 1);
Console.WriteLine(equalA1);    // True
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Boolean Type
## [Demo]() -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic20.png" style="top:50%; left:10%; width:45%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'char', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# <a id="char"></a>Character Type
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic21.png" style="top:42.31%; left:9.36%; width:40%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic22.png" style="top:9.43%; left:43.98%; width:54.66%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# The Character Data Type
- The **character data type**:
  - Represents symbolic information
  - Is declared by the **char** keyword
  - Gives each symbol a corresponding integer code
  - Has a **'\0'** default value
  - Takes 16 bits of memory (from **U+0000** to **U+FFFF**)

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic23.png" style="top:60.57%; left:64.56%; width:39.67%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Characters and Codes
- The example below shows that every symbol has an unique Unicode code:

```cs
char symbol = 'a';
Console.WriteLine("The code of '{0}' is: {1}",
    symbol, (int) symbol);
symbol = 'b';
Console.WriteLine("The code of '{0}' is: {1}",
    symbol, (int) symbol);
symbol = 'A';
Console.WriteLine("The code of '{0}' is: {1}",
    symbol, (int) symbol);
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Character Type
## [Demo]() -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic24.png" style="top:50%; left:30.88%; width:40%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'string', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# <a id="string"></a>String Type
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic25.png" style="top:39.21%; left:24.33%; width:30%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic26.png" style="top:40%; left:60%; width:30%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# The String Data Type
- The **string data type**:
  - Represents a sequence of characters
  - Is declared by the **string** keyword
  - Has a default value **null** (no value)
- Strings are enclosed in quotes:
- Strings can be concatenated
  - Using the **+** operator

```cs
string s = "Microsoft .NET Framework";
```



<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Saying Hello – _Example_
- Concatenating the two names of a person to obtain his full name:
  - _Note_: a space is missing between the two names! We have to add it manually

```cs
string firstName = "Ivan";
string lastName = "Ivanov";
Console.WriteLine("Hello, {0}!\n", firstName);

string fullName = firstName + " " + lastName;
Console.WriteLine("Your full name is {0}.",
  fullName);
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # String Type
## [Demo]() -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic27.png" style="top:40.33%; left:40.23%; width:40%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'object', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# <a id="object"></a>Object Type
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic28.png" style="top:40%; left:27%; width:45%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# The Object Type
- The object type:
  - Is declared by the **object** keyword
  - Is the base type of all other types
  - Can hold values of any type

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic29.png" style="top:52.01%; left:73.61%; width:28.72%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic30.png" style="top:51.13%; left:28.07%; width:34.38%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Using Objects
- _Example_ of an object variable taking different types of data:

```cs
object dataContainer = 5;
Console.Write("The value of dataContainer is: ");
Console.WriteLine(dataContainer);

dataContainer = "Five";
Console.Write("The value of dataContainer is: ");
Console.WriteLine(dataContainer);
```

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic31.png" style="top:59.94%; left:31.70%; width:45.95%; z-index:-1" /> -->


<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Objects
## [Demo]() -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic32.png" style="top:30%; left:50.53%; width:35%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Introducing Variables
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic33.png" style="top:43.20%; left:37.43%; width:38.79%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic34.png" style="top:7.05%; left:81.40%; width:22.43%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# What Is a Variable?
- A variable is a:
  - Placeholder of information that can usually be changed at run-time
- Variables allow you to:
  - Store information
  - Retrieve the stored information
  - Manipulate the stored information

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic35.png" style="top:29.09%; left:72.98%; width:32.52%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Variable Characteristics
- A variable has:
  - Name
  - Type (of stored data)
  - Value
- _Example_:
  - Name: **counter**
  - Type: **int**
  - Value: **5**

```cs
int counter = 5;
```

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic36.png" style="top:14.10%; left:67.37%; width:35.37%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'assign', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# <a id="declaring"></a>Declaring And Using Variables
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic37.png" style="top:50%; left:50.53%; width:35%; z-index:-1" /> -->


<!-- attr: { id:'declaring', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Declaring Variables
- When declaring a variable we:
  - Specify its type
  - Specify its name (called identifier)
  - May give it an initial value
- The syntax is the following:
- _Example_:

```cs
<data_type> <identifier> [= <initialization>];
```


```cs
int height = 200;
```



<!-- attr: { id:'identifiers', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# <a id="identifiers"></a>Identifiers
- Identifiers may consist of:
  - Letters (Unicode)
  - Digits [0-9]
  - Underscore "\_"
- Identifiers
  - Can begin only with a letter or an underscore
  - Cannot be a C# keyword

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic38.png" style="top:19.39%; left:67.37%; width:30%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
<!-- # Identifiers -->
- Identifiers
  - Should have a descriptive name
  - It is recommended to use only Latin letters
  - Should be neither too long nor too short
- _Note_:
  - In C# small letters are considered different than the capital letters (case sensitivity)


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Identifiers – _Examples_
- _Examples_ of correct identifiers:
- _Examples_ of incorrect identifiers:

```cs
int new;	// new is a keyword
int 2Pac;	// Cannot begin with a digit
```


```cs
int New = 2; // Here N is capital
int _2Pac; // This identifiers begins with _
string поздрав = "Hello"; // Unicode symbols used
// The following is more appropriate:
string greeting = "Hello";
int n = 100; // Undescriptive
int numberOfClients = 100; // Descriptive
// Overdescriptive identifier:
int numberOfPrivateClientOfTheFirm = 100;
```





<!-- section start -->
<!-- attr: { id:'assign', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# <a id="assign"></a>Assigning Values To Variables
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic39.png" style="top:51.57%; left:30%; width:40%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic40.png" style="top:-1.97%; left:80.69%; width:15.89%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Assigning Values
- Assigning of values to variables
  - Is achieved by the **=** operator
- The **=** operator has
  - Variable identifier on the left
  - Value of the corresponding data type on the right
  - Could be used in a cascade calling, where assigning is done from right to left

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic41.png" style="top:14.10%; left:83.27%; width:21.16%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Assigning Values – _Examples_
- Assigning values example:

```cs
int firstValue = 3;
int secondValue;
int thirdValue;

// Using an already declared variable:
secondValue = firstValue;

// The following cascade calling assigns
// 3 to firstValue and then firstValue
// to thirdValue, so both variables have
// the value 3 as a result:

thirdValue = firstValue = 3; // Avoid this!
```

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic42.png" style="top:18.91%; left:84.21%; width:18.95%; z-index:0" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Initializing Variables
- Initializing
  - Is assigning of initial value
  - Must be done before the variable is used!
- Several ways of initializing:
  - By using the **new** keyword
  - By using a literal expression
  - By referring to an already initialized variable

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic43.png" style="top:38.79%; left:89.54%; width:13.58%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Initialization – _Examples_
- _Example_ of some initializations:

```cs
// The following would assign the default
// value of the int type to num:
int num = new int(); // num = 0

// This is how we use a literal expression:
float heightInMeters = 1.74f;

// Here we use an already initialized variable:
string greeting = "Hello World!";
string message = greeting;
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Assigning and Initializing Variables
## [Demo]() -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic44.png" style="top:40.55%; left:9.27%; width:25.65%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic45.png" style="top:40.55%; left:76.72%; width:23.80%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'literals', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# <a id="literals"></a>Literals
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic46.png" style="top:40%; left:25.85%; width:54.99%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# What are Literals?
- Literals are:
  - Representations of values in the source code
- There are six types of literals
  - Boolean
  - Integer
  - Real
  - Character
  - String
  - The **null** literal

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic47.png" style="top:39.67%; left:55.20%; width:43.81%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Boolean and Integer Literals
- The boolean literals are:
  - **true**
  - **false**
- The integer literals:
  - Are used for variables of type **int**, **uint**, **long**, and **ulong**
  - Consist of digits
  - May have a sign (**+**,**-**)
  - May be in a hexadecimal format

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic48.png" style="top:10.58%; left:80.67%; width:21.61%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Integer Literals
- _Examples_ of integer literals
  - The **'0x'** and **'0X'** prefixes mean a hexadecimal value, e.g. **0xA8F1**
  - The **'u'** and **'U'** suffixes mean a **ulong** or **uint** type, e.g. **12345678U**
  - The **'l'** and **'L'** suffixes mean a **long** or **ulong** type, e.g. **9876543L**

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic49.png" style="top:54.35%; left:73.92%; width:29.97%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Integer Literals – _Example_
- _Note_: the letter ‘**l**’ is easily confused with the digit ‘**1**’ so it’s better to use ‘**L**’!!!

```cs
// The following variables are
// initialized with the same value:
int numberInHex = -0x10;
int numberInDec = -16;

// The following causes an error,
because 234u is of type uint
int unsignedInt = 234u;

// The following causes an error,
because 234L is of type long
int longInt = 234L;
```



<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Real Literals
- The real literals:
  - Are used for values of type **float**, **double** and **decimal**
  - May consist of digits, a sign and “**.**”
  - May be in exponential notation: **6.02e+23**
- The “**f**” and “**F**” suffixes mean **float**
- The “**d**” and “**D**” suffixes mean **double**
- The “**m**” and “**M**” suffixes mean **decimal**
- The default interpretation is **double**


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Real Literals – _Example_
- _Example_ of incorrect **float** literal:
- A correct way to assign floating-point value (using also the exponential format):

```cs
// The following causes an error
// because 12.5 is double by default
float realNumber = 12.5;
```


```cs
// The following is the correct
// way of assigning the value:
float realNumber = 12.5f;
// This is the same value in exponential format:
realNumber = 1.25e+7f;
```



<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Character Literals
- The character literals:
  - Are used for values of the **char** type
  - Consist of two single quotes surrounding the character value: **'<value>'**
- The value may be:
  - Symbol
  - The code of the symbol
  - Escaping sequence

<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic50.png" style="top:44.52%; left:64.99%; width:39.27%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Escaping Sequences
- Escaping sequences are:
  - Means of presenting a symbol that is usually interpreted otherwise (like **'**)
  - Means of presenting system symbols (like the new line symbol)
- Common escaping sequences are:
  - **\'** for single quote	**\"** for double quote
  - **\\** for backslash		**\n** for new line
  - **\uXXXX** for denoting any other Unicode symbol


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Character Literals – _Example_
- _Examples_ of different character literals:

```cs
char symbol = 'a'; // An ordinary symbol
symbol = '\u006F'; // Unicode symbol code in a			      // hexadecimal format (letter 'o')
symbol = '\u8449'; // 葉 (Leaf in Traditional Chinese)
symbol = '\''; // Assigning the single quote symbol
symbol = '\\'; // Assigning the backslash symbol
symbol = '\n'; // Assigning new line symbol
symbol = '\t'; // Assigning TAB symbol
symbol = "a"; // Incorrect: use single quotes
```



<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# String Literals
- String literals:
  - Are used for values of the string type
  - Consist of two double quotes surrounding the value: **"<value>"**
  - May have a **@** prefix which ignores the used escaping sequences: **@"<value>"**
- The value is a sequence of character literals

```cs
string s = "I am a sting literal";
```



<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# String Literals – _Example_
- Benefits of quoted strings (the **@** prefix):
- In quoted strings **\"** is used instead of **""**!

```cs
// Here is a string literal using escape sequences
string quotation = "\"Hello, Jude\", he said.";
string path = "C:\\WINNT\\Darts\\Darts.exe";

// Here is an example of the usage of @
quotation = @"""Hello, Jimmy!"", she answered.";
path = @"C:\WINNT\Darts\Darts.exe";

string str = @"some
		text";
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # String Literals
## [Demo]() -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic51.png" style="top:17.67%; left:46.13%; width:18.40%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Nullable Types -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic52.png" style="top:44.74%; left:5.61%; width:56.31%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic53.png" style="top:40.56%; left:70.20%; width:27.88%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic54.png" style="top:2.45%; left:75.79%; width:19.56%; z-index:-1" /> -->


<!-- attr: { id:'nullable', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# <a id="nullable"></a>Nullable Types
- **Nullable** types are instances of the **System.Nullable** struct
  - Wrapper over the **primitive** **types**
  - E.g. **int?**, **double?**, etc.
- **Nullabe** type can represent the normal range of values for its underlying value type, plus an additional **null** value
- Useful when dealing with **Databases** or other structures that have default value **null**


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# Nullable Types – _Example_
- _Example_ with **Integer**:

```cs
int? someInteger = null;
Console.WriteLine(
  "This is the integer with Null value -> " + someInteger);
someInteger = 5;
Console.WriteLine(
  "This is the integer with value 5 -> " +  someInteger);
```


```cs
double? someDouble = null;
Console.WriteLine(
  "This is the real number with Null value -> "
  + someDouble);
someDouble = 2.5;
Console.WriteLine(
  "This is the real number with value 5 -> " +
  someDouble);
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Nullable Types
## [Demo]() -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic55.png" style="top:45.84%; left:8.56%; width:37.13%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic56.png" style="top:49.18%; left:61.45%; width:33.81%; z-index:-1" /> -->




<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Dynamic Types in _C#_
## Types Holding Anything & Evaluated at Runtime -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic57.png" style="top:55%; left:10%; width:35%; z-index:-1" /> -->


<!-- attr: { id:'dynamic', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'' } -->
# <a id="dynamic"></a>Dynamic Types
- **Dynamic types**in C# (keyword **dynamic**)
  - Can hold anything (string, number, object, function / method reference)
  - Operations evaluated at runtime
  - Behave like types in JavaScript / PHP

```cs
dynamic a = 5;
dynamic b = 3;
Console.WriteLine(a + b); // 8 (sum of integers)
a = "5";
b = 3;
Console.WriteLine(a + b); // 53 (string concatenation)
```



<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Dynamic Types
## [Demo]() -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic58.png" style="top:45%; left:15%; width:35%; z-index:-1" /> -->


<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
<!-- # Primitive Data Types and Variables
## Questions? -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic59.png" style="top:47.60%; left:1.87%; width:29.97%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic60.png" style="top:46.21%; left:77.66%; width:29.97%; z-index:-1" /> -->


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'' } -->
# Free Trainings @ Telerik Academy
- Fundamentals of C# ProgrammingTrack of Courses
    - csharpfundamentals.telerik.com
  - Telerik Software Academy
    - [academy.telerik.com](academy.telerik.com)
  - Telerik Academy @ Facebook
    - [facebook.com/TelerikAcademy](facebook.com/TelerikAcademy)
  - Telerik Academy Learning System
    - [telerikacademy.com](telerikacademy.com)
    
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic63.png" style="top:58.18%; left:90.52%; width:16.97%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic64.png" style="top:34.35%; left:68.14%; width:36.30%; z-index:-1" /> -->
<!-- <img class="slide-image" showInPresentation="true"  src="imgs/pic65.png" style="top:48.92%; left:75.91%; width:10.85%; z-index:-1" /> -->
