<!-- section start -->
<!-- attr: { id:'', class:'slide-title', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Introduction to Programming
## Creating and Running Your First C# Program
<img class="slide-image" src="\imgs\pic00.png" style="top:55%; left:30%; width:20.28%; z-index:-1" />
<img class="slide-image" src="\imgs\pic01.png" style="top:55%; left:70%; width:15.87%; z-index:-1" />
<img class="slide-image" src="\imgs\pic02.png" style="top:10%; left:2%; width:12.87%; z-index:-1" />




<!-- section start -->
<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Table of Contents
- What is Computer Programming?
- Your First C# Program
- What is .NET Framework?
- What is Visual Studio?
- What is MSDN Library?
<img class="slide-image" src="\imgs\pic05.png" style="top:32.52%; left:65%; width:26.45%; z-index:-1" />

<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# What is Computer Programming?
<img class="slide-image" src="\imgs\pic06.png" style="top:55%; left:30%; width:40%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Define: Computer Programming
- **Computer programming**: creating a sequence of instructions to enable the computer to do something
    - Definition by <img class="slide-image" src="\imgs\pic08.png" style="top:26%; left:32%; width:20%; z-index:-1" />

<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'font-size: 42px' } -->
# Programming Phases
- `Define` a task/problem **= Specification**
- Plan your solution **= Design**
  - Find suitable algorithm to solve it
  - Find suitable data structures to use
- Write code **= Implementation**
- Fix program error (bugs) **= Testing & Debugging**
- Make your customer happy **= Deployment**

<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Your First C# Program
<img class="slide-image" src="\imgs\pic09.png" style="top:44.96%; left:30%; width:40%; z-index:-1" />

<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# First Look at C# Language
- Sample C# program:

```cs
using System;

class HelloCSharp
{
    static void Main()
    {
        Console.WriteLine("Hello, C#");
    }
}
```

<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# C# Code – How It Works?

```cs
using System;

class HelloCSharp
{
    static void Main()
    {
        Console.WriteLine("Hello, C#");
    }
}
```

<div class="fragment balloon" style="top:14.03%; left:2.64%; width:42.97%">Include the standard namespace "**System**"</div>
<div class="fragment balloon" style="top:12.16%; left:55.54%; width:40.81%">Define a class called "**HelloCSharp**"</div>
<div class="fragment balloon" style="top:29.01%; left:58.18%; width:40.81%">Define the **Main()**method – the program entry point</div>
<div class="fragment balloon" style="top:63.62%; left:25.56%; width:61.65%">Print a text on the console by calling the method "**WriteLine**" of the class "**Console**"</div>


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# C# Code Should Be Well Formatted

```cs
using System;

class HelloCSharp
{
    static void Main()
    {
        Console.WriteLine("Hello, C#");
    }
}
```

<div class="fragment balloon" style="top:31.81%; left:52.89%; width:44.08%">The **{** symbol should be alone on a new line.</div>
<div class="fragment balloon" style="top:62.69%; left:59.93%; width:38.33%">The block after the **{** symbol should be indented by a **TAB**.</div>
<div class="fragment balloon" style="top:62.69%; left:14.99%; width:40.81%">The **}** symbol should be under the corresponding **{**.</div>
<div class="fragment balloon" style="top:13.10%; left:29.97%; width:68.76%">Class names should use **PascalCase** and start with a **CAPITAL** letter.</div>


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Example of Bad Formatting

```cs
         using 
System
                                                ;

    class         HelloCSharp                   {
	    static 
void       Main(                  )   {   Console   .      WriteLine    ("Hello, C#"     )  ;Console.
   WriteLine        (               "Hello again"
                    )                         ;}}
```

<div class="fragment balloon" style="top:14.97%; left:49.37%; width:35.22%">Such formatting makes the source code unreadable.</div>


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# What is "C#"?
- Programming language
  - A syntax that allow to give instructions to the computer
- C# features:
  - New cutting edge language
  - Extremely powerful
  - Easy to learn
  - Easy to read and understand
  - Object-oriented
<img class="slide-image" src="\imgs\pic11.png" style="top:49.27%; left:74.85%; width:28.21%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# What You Need to Program?
- Knowledge of a programming language
  - **C#**, **Javascript**, **C++**, **Java**, **Python**, etc
- Task to solve
- Development environment, compilers, SDK
  - For **C#** - **VisualStudio**, **.NET Framework SDK**
- Set of useful standard classes
  - **Microsoft .NETFramework FCL**
- Help documentation
  - **MSDN Library**
  
<img class="slide-image" src="\imgs\pic12.png" style="top:49.81%; left:80.00%; width:23.36%; z-index:-1" />

<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Your First C# Program
## [Demo]()

<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# What is .NET Framework?
<img class="slide-image" src="\imgs\pic17.png" style="top:55%; left:35%; width:30%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# What is .NET Framework?
- Environment for execution of .NET programs
- Powerful library of classes
- Programming model
- Common execution engine for many programming languages
  - C#
  - F#
  - Visual Basic .NET
  - Managed C++
  - ... and many others
<img class="slide-image" src="\imgs\pic18.png" style="top:54.11%; left:63.62%; width:37.98%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'font-size: 40px' } -->
# Inside .NET Framework
- Building blocks of .NET Framework

<img class="slide-image" src="\imgs\dot-net-blocks.png" style="top:25%; left:10%; width:80%; z-index:-1" />

<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# CLR – The Heart of .NET Framework
- Common Language Runtime (CLR)
  - Managed execution environment
    - Executes .NET applications
    - Controls the execution process
  - Automatic memory management (garbage collection)
  - Programming languages integration
  - Multiple versions support for assemblies
  - Integrated type safety and security
- CLR
<img class="slide-image" src="\imgs\pic19.png" style="top:15%; left:80%; width:20%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'font-size: 42px' } -->
# Framework Class Library
- Framework Class Library (FCL)
  - Provides basic functionality to developers:
    - Console applications
    - WPF and Silverlight rich-media applications
    - Windows Forms GUI applications
    - Web applications (dynamic Web sites)
    - Web services, communication and workflow
    - Server & desktop applications
    - Applications for mobile devices




<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# What is Visual Studio?
## Compiling, Running and Debugging C# Programs 

<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Visual Studio
- Visual Studio – Integrated Development Environment (IDE)
- Development tool that helps us to:
  - Write code
  - Design user interface
  - Compile code
  - Execute / test / debug applications
  - Browse the help
  - Manage project's files
<img class="slide-image" src="\imgs\pic20.png" style="top:63.47%; left:79.09%; width:26.86%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Benefits of Visual Studio
- Single tool for:
  - Writing code in many languages (C#, VB, …)
  - Using different technologies (Web, WPF, …)
  - For different platforms (.NET CF, Silverlight, …)
- Full integration of most development activities (coding, compiling, testing, debugging, deployment, version control, ...)
- Very easy to use!
<img class="slide-image" src="\imgs\pic20.png" style="top:64.35%; left:79.82%; width:25.95%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Visual Studio – Example
<img class="slide-image" src="\imgs\pic23.png" style="top:12.34%; left:13.10%; width:81.10%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Creating New Console Application
- File &rarr; New &rarr; Project ...
- Choose C# console application
- Choose project directory and name
<img class="slide-image" src="\imgs\pic24.png" style="top:35%; left:30%; width:62.31%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
<!-- # Creating New Console Application -->
- Visual Studio creates some source code for you
<div class="fragment balloon" style="top:25.26%; left:3.53%; width:23.80%">Namespace not required</div>
<div class="fragment balloon" style="top:42.10%; left:52.89%; width:24.15%">Class name should be changed</div>
<div class="fragment balloon" style="top:25.72%; left:48.48%; width:29.09%">Some imports are not required</div>
<img class="slide-image" src="\imgs\pic25.png" style="top:21.13%; left:10.56%; width:85.88%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Compiling Source Code
- The process of **compiling** includes:
  - Syntactic checks
  - Type safety checks
  - Translation of the source code to lower level language (MSIL)
  - Creating of executable files (assemblies)
- You can start compilation by
  - Using **Build->Build Solution/Project**
  - Pressing **[F6]** or **[Shift+Ctrl+B]**
<img class="slide-image" src="\imgs\pic26.png" style="top:59.38%; left:86.08%; width:19.85%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Running Programs
- The process of **running** application includes:
  - Compiling (if project not compiled)
  - Starting the application
- You can run application by:
  - Using **Debug->Start** menu
  - By pressing **[F5]** or **[Ctrl+F5]**
  - _Note_: Not all types of projects are startable!

<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Debugging The Code
- The process of **debugging** application includes:
  - Spotting an error
  - Finding the lines of code that cause the error
  - Fixing the code
  - Testing to check if the error is gone and no errors are introduced
- Iterative and continuous process


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Debugging in Visual Studio
- Visual Studio has built-in debugger
- It provides:
  - Breakpoints
  - Ability to trace the code execution
  - Ability to inspect variables at runtime
<img class="slide-image" src="\imgs\pic31.png" style="top:50.65%; left:19.43%; width:68.96%; z-index:-1" />


<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Visual Studio
## Compiling, Running and Debugging C# Programs 
## [Demo]()




<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Visual Studio  Blank Solution
## Creating a Solution Without Projects
<img class="slide-image" src="\imgs\pic35.png" style="top:55%; left:25%; width:50%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'False', style:'font-size: 42px' } -->
# What Is a Blank Solution?
- A Visual Studio blank solution
  - Solution with no projects in it
    - Projects to be added later
- What is the point?
  - Not making a project just to give proper name
    - And not working in this project


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# VS Blank Solution
<img class="slide-image" src="\imgs\pic36.png" style="top:12.34%; left:8.27%; width:90.19%; z-index:-1" />


<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Visual Studio  Blank Solution
## [Demo]()

<!-- section start -->
<!-- attr: { id:'', class:'slide-section', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# What is MSDN Library?

<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# What is MSDN Library?
- Complete documentation of all classes and their functionality
  - With descriptions of all methods, properties, events, etc.
  - With code examples
- Related articles
- Library of samples
- Use local copy or the Web version at http://msdn.microsoft.com/
<img class="slide-image" src="\imgs\pic41.png" style="top:50.90%; left:60.05%; width:42.16%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# MSDN Library
<img class="slide-image" src="\imgs\pic42.png" style="top:13.22%; left:6.43%; width:93.55%; z-index:-1" />


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# How to Use MSDN Library?
- Offline version (obsolete)
  - Use the table of contents
  - Use the alphabetical index
  - Search for phrase or keyword
  - Filter by technology
  - Browse your favorite articles
- Online version
  - Use the built-in search: [F1]


<!-- attr: { id:'', class:'slide-section demo', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# MSDN Library
## Browsing and Searching Documentation
## [Demo]()


<!-- attr: { id:'', class:'', showInPresentation:'True', hasScriptWrapper:'True', style:'font-size: 42px' } -->
# Introduction to Programming
- Questions?
<img class="slide-image" src="\imgs\pic47.png" style="top:43.21%; left:82.34%; width:19.97%; z-index:-1" />
<img class="slide-image" src="\imgs\pic48.png" style="top:43.20%; left:42.10%; width:24.25%; z-index:-1" />
<img class="slide-image" src="\imgs\pic49.png" style="top:43.20%; left:8.19%; width:23.14%; z-index:-1" />