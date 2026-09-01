
# 🚀 Introduction to C#

## 📌 What is C#?

C# (pronounced "C-Sharp") is a modern, object-oriented, type-safe programming language developed by Microsoft.

C# is mainly used with the .NET platform to build different types of applications such as:

- Web Applications
- Desktop Applications
- Web APIs
- Cloud Applications
- Mobile Applications
- Games
- Enterprise Applications
- Database Applications
- Services and Backend Systems

C# was introduced by Microsoft in the early 2000s and has continuously evolved with new features and improvements.

---

# 🧠 Why was C# created?

C# was designed to provide a modern, powerful and developer-friendly programming language for building reliable software.

C# combines ideas from several programming languages while providing features such as:

- Object-Oriented Programming
- Strong Type Safety
- Automatic Memory Management
- Exception Handling
- Generics
- Delegates and Events
- LINQ
- Asynchronous Programming
- Pattern Matching
- Modern Language Features

---

# 🌐 C# and .NET

C# and .NET are related, but they are **not the same thing**.

### C#

C# is a **programming language**.

We use C# to write our program.

### .NET

.NET is a **development platform/runtime and ecosystem** used to build and run applications written in C# and other languages.

Simple way to remember:

```text
C#       → Language
.NET     → Platform
Program  → Written using C#
Runtime  → Runs the application

🖥️ Desktop Applications

C# can be used to create Windows desktop applications.

Examples:

Windows Forms
WPF
🎮 Games

C# is widely used with the Unity game engine for game development.

☁️ Cloud Applications

C# and .NET are commonly used for building cloud-based and distributed applications.

🏢 Enterprise Applications

C# is commonly used in large business applications such as:

Hospital Management Systems
Banking Systems
ERP Systems
Inventory Systems
Billing Systems
Employee Management Systems
⭐ Key Features of C#
1. Object-Oriented

C# supports Object-Oriented Programming (OOP).

The major OOP concepts are:

Encapsulation
Inheritance
Polymorphism
Abstraction
2. Type-Safe

C# is a strongly typed language.

This means the compiler checks whether values are being used with compatible types.

Example:

int age = 22;

Here age is an integer.

3. Automatic Memory Management

C# uses Garbage Collection to automatically manage managed memory.

Developers generally don't need to manually allocate and free memory like in C.

4. Exception Handling

C# provides structured exception handling using:

try
catch
finally
throw

Example:

try
{
    int result = 10 / 0;
}
catch (Exception ex)
{
    Console.WriteLine(ex.Message);
}
5. Generics

Generics allow us to write reusable and type-safe code.

Example:

List<int> numbers = new List<int>();
6. LINQ

LINQ allows us to query collections and other data sources using C# syntax.

Example:

var result = numbers.Where(x => x > 10);
7. Asynchronous Programming

C# supports asynchronous programming using:

async
await
Task

This is useful when working with operations such as:

API calls
Database operations
File operations
Network operations
🔤 C# Name

C# is pronounced:

C-Sharp

The # symbol represents "Sharp" in the name.

🆚 C vs C#

C and C# are different programming languages.

Although C# has roots in the C family of languages, their design and programming models are significantly different.

Feature	C	C#
Type	Procedural	Multi-paradigm, primarily object-oriented
Developed By	Bell Labs / Dennis Ritchie and team	Microsoft
First Released	1970s	2000s
Main Ecosystem	Native/System Programming	.NET
Memory Management	Mostly manual	Garbage Collection for managed code
OOP Support	No native OOP model	Yes
Classes	❌	✅
Objects	❌	✅
Inheritance	❌	✅
Polymorphism	❌	✅
Interfaces	❌	✅
Generics	❌	✅
LINQ	❌	✅
Delegates	❌	✅
Events	❌	✅
Async/Await	❌	✅
Garbage Collection	❌	✅
Pointers	✅	Supported in unsafe code
Typical Use	System/Embedded Programming	Web, Backend, Desktop, Cloud, Games, Enterprise
🔥 C vs C# — Simple Explanation

The biggest difference is the programming model and ecosystem.

C

C is mainly a procedural systems programming language.

You generally think in terms of:

Functions
    ↓
Data
    ↓
Instructions

C gives the programmer much more direct control over memory and hardware.

Example:

#include <stdio.h>

int main()
{
    int age = 22;

    printf("%d", age);

    return 0;
}
C#

C# is a modern, multi-paradigm language with strong support for object-oriented programming and the .NET ecosystem.

Example:

using System;

class Program
{
    static void Main()
    {
        int age = 22;

        Console.WriteLine(age);
    }
}
🧠 C vs C# — Easy Real-Life Analogy

Think about building a house.

C

C gives you more low-level control.

You are closer to the underlying system and are responsible for more details.

Program
   ↓
Memory / Hardware
C#

C provides a higher-level development environment with many built-in features.

C# Program
     ↓
.NET
     ↓
Operating System
     ↓
Hardware

This does not mean C# is simply "better" than C.

They are designed for different purposes.

⚙️ Memory Management Difference

One of the important differences is memory management.

C

In C, programmers commonly manage dynamically allocated memory manually.

Example:

int *ptr = malloc(sizeof(int));

*ptr = 10;

free(ptr);

The programmer is responsible for releasing allocated memory.

C#

C provides automatic garbage collection for managed memory.

Example:

class Student
{
    public string Name;
}

Student student = new Student();

student.Name = "Neeraj";

The .NET runtime's Garbage Collector manages the lifetime of managed objects when they are no longer reachable.

🏗️ Programming Style
C

C mainly follows procedural programming.

Functions
   ↓
Logic
   ↓
Data
C#

C# supports multiple programming styles, with strong support for object-oriented programming.

Class
  ↓
Object
  ↓
Properties
  ↓
Methods
  ↓
Behavior
📌 Important Note

C# is not simply "C with # added to it."

C# belongs to the broader C-family of programming languages, but it is a separate language with its own:

Syntax
Type system
Runtime environment
Object model
Libraries
Features
Development ecosystem
💻 Basic C# Program
using System;

class Program
{
    static void Main()
    {
        Console.WriteLine("Hello World!");
    }
}

Output:

Hello World!
🔍 Understanding the Program
using System;

System is a namespace that contains many commonly used .NET types.

Because of this using directive, we can write:

Console.WriteLine();

instead of:

System.Console.WriteLine();
class Program

This declares a class named Program.

Classes are one of the fundamental building blocks of C# programs.

static void Main()

Main is the entry point of a traditional C# console application.

Execution starts from the program's entry point.

Console.WriteLine()

Console is a .NET type used for console input/output.

WriteLine() writes text to the console and moves to the next line.

;

A semicolon marks the end of a statement in C#.

Example:

int age = 22;
Console.WriteLine(age);
🔤 C# is Case-Sensitive

C# is case-sensitive.

These are different identifiers:

name
Name
NAME

For example:

int age = 22;

Console.WriteLine(age);

is different from:

Console.WriteLine(Age);

if Age has not been declared.

📁 C# Source Files

C# source files normally use the:

.cs

extension.

Example:

Program.cs
Student.cs
Employee.cs
Calculator.cs

The filename does not generally have to match the class name.

🛠️ C# IDEs and Tools

An IDE (Integrated Development Environment) provides tools for writing, building, debugging and managing code.

Common options for C# development include:

Visual Studio
Visual Studio Code
JetBrains Rider

For beginners, Visual Studio Community is a popular choice for learning C# and .NET.

📚 What I Will Learn in This Repository

This repository will cover C# from Basic → Intermediate → Advanced.

The learning journey will include:

C# Introduction
      ↓
Basics
      ↓
Variables & Data Types
      ↓
Operators
      ↓
Conditions
      ↓
Loops
      ↓
Methods
      ↓
Arrays & Strings
      ↓
OOP
      ↓
Properties
      ↓
Structs & Enums
      ↓
Collections
      ↓
Exception Handling
      ↓
Generics
      ↓
Delegates
      ↓
Events
      ↓
Lambda Expressions
      ↓
LINQ
      ↓
File Handling
      ↓
Serialization
      ↓
Memory Management
      ↓
Async/Await
      ↓
Multithreading
      ↓
Pattern Matching
      ↓
Reflection
      ↓
Records
      ↓
Advanced C#
      ↓
Modern C# Features
🎯 My Learning Goal

The goal is to understand C# deeply rather than simply memorize syntax.

For every important topic, I will try to understand:

What is it?
Why is it used?
How does it work?
What is the syntax?
How do I use it?
Where is it used in real applications?
What are common mistakes?
What questions can be asked in interviews?
Can I solve problems using this concept?
📝 Learning Method

I will learn C# from tutorials and maintain my own notes here.

My learning process:

Learn
  ↓
Understand
  ↓
Write Notes
  ↓
Code
  ↓
Practice
  ↓
Make Mistakes
  ↓
Fix Mistakes
  ↓
Revise

Goal: Understand C#, don't just memorize C#.

👨‍💻 Author

Neeraj Lalwani

Learning C# from Basic to Advanced.
