---
title: "Course Overview - Object-Oriented Programming in C++"
description: "Introduction to Object-Oriented Programming course covering encapsulation, inheritance, polymorphism, and abstract types"
course: "CS 165"
unit: "Unit 0"
chapter: "0-Course-Overview"
tags:
  - cpp
  - object-oriented-programming
  - course-overview
  - encapsulation
  - inheritance
  - polymorphism
source:
  type: "AI-Generated Draft"
  method: "Mistral OCR"
  original: "0-Course-Overview.pdf"
  generated: "2025-08-03 16:15:23"
  book:
    title: "CS165 Text"
    format: "Unknown Binding"
    asin: "B0DTVZSPM2"
  course_url: "https://content.byui.edu/file/eba8da04-5bfb-481c-aac6-d571199802f3/5/CS%20165%20Syllabus.html"
  institution: "Brigham Young University - Idaho"
author: "CS 165 Course Materials"
date: "2025-08-03"
---

# Table of Contents {.background}

| :---
| Course Overview |
| [Review](0-Review.ai.md) |
| [1.0 Design Documents](../Unit-1/Chapter-1.0/1.0-Using-Objects.ai.md) |
| [1.1 Defensive Programming](../Unit-1/Chapter-1.1/1.1-Defensive-Programming.ai.md) |
| [1.2 Exception Handling](../Unit-1/Chapter-1.2/1.2-Exception-Handling.ai.md) |
| [1.3 Structures](../Unit-1/Chapter-1.3/1.3-Structures.ai.md) |
| [1.4 Separate Compilation](../Unit-1/Chapter-1.4/1.4-Separate-Compilation.ai.md) |
| [1.5 Function: Advanced Topics](../Unit-1/Chapter-1.5/1.5-Function-Advanced-Topics.ai.md) |
| [2.0 Encapsulation Design](../Unit-2/Chapter-2.0/2.0-Encapsulation-Design.ai.md) |
| [2.1 Building a Class](../Unit-2/Chapter-2.1/2.1-Building-a-Class.ai.md) |
| [2.2 Class Syntax](../Unit-2/Chapter-2.2/2.2-Class-Syntax.ai.md) |
| [2.3 Accessors & Mutators](../Unit-2/Chapter-2.3/2.3-Accessors-&-Mutators.ai.md) |
| [2.4 Constructors & Destructors](../Unit-2/Chapter-2.4/2.4-Constructors-&-Destructors.ai.md) |
| [2.5 Static](../Unit-2/Chapter-2.5/2.5-Static.ai.md) |
| [2.6 Non-Member Operator Overloading](../Unit-2/Chapter-2.6/2.6-Non-Member-Operator-Overloading.ai.md) |
| [2.7 Friends](../Unit-2/Chapter-2.7/2.7-Friends.ai.md) |
| [2.8 Member Operator Overloading](../Unit-2/Chapter-2.8/2.8-Member-Operator-Overloading.ai.md) |
| [3.0 Class Relations](../Unit-3/Chapter-3.0/3.0-Class-Relations.ai.md) |
| [3.1 Building Polymorphism](../Unit-3/Chapter-3.1/3.1-Building-Polymorphism.ai.md) |
| [3.2 Inheritance](../Unit-3/Chapter-3.2/3.2-Inheritance.ai.md) |
| [3.3 Inheritance Qualifiers](../Unit-3/Chapter-3.3/3.3-Inheritance-Qualifiers.ai.md) |
| [3.4 Virtual Functions](../Unit-3/Chapter-3.4/3.4-Virtual-Functions.ai.md) |
| [3.5 Pure Virtual Functions](../Unit-3/Chapter-3.5/3.5-Pure-Virtual-Functions.ai.md) |
| [4.0 Type-Independent Design](../Unit-4/Chapter-4.0/4.0-Type-Independent-Design.ai.md) |
| [4.1 Void Pointers and Callbacks](../Unit-4/Chapter-4.1/4.1-Void-Pointers-and-Callbacks.ai.md) |
| [4.2 Function Templates](../Unit-4/Chapter-4.2/4.2-Function-Templates.ai.md) |
| [4.3 Class Templates](../Unit-4/Chapter-4.3/4.3-Class-Templates.ai.md) |
| [4.4 Linked Lists](../Unit-4/Chapter-4.4/4.4-Linked-List.ai.md) |
| [4.5 Iterators](../Unit-4/Chapter-4.5/4.5-Iterators.ai.md) |
| [4.6 Standard Template Library](../Unit-4/Chapter-4.6/4.6-Standard-Template-Library.ai.md) |
| [A. Elements of Style](../Appendix/Appendix-A-Elements-of-Style.ai.md) |
| [B. C++ Syntax Reference Guide](../Appendix/Appendix-B-C++-Reference-Guide.ai.md) |
| [C. Glossary](../Appendix/Appendix-C-Glossary.ai.md) |
| [D. Index](../Appendix/Appendix-D-Index.ai.md) |

> **In this Chapter:**
> [[toc]]

# Course Overview {.background}

Procedural programming, the subject of CS 124 preceding this class, is a style of programming where the focus is on the function. This includes how to subdivide a program into functions (in a process called modularization) and what goes on inside functions. Virtually any programming project can be completed with procedural programming tools.
Object-Oriented programming, on the other hand, is a style of programming where the focus is on the class. A class is a construct containing a collection of functions as well as the data associated with them. Topics such as encapsulation (how to create well-designed classes), inheritance (the relationship between classes), and polymorphism (working with many versions of related classes) form the backbone of Object-Oriented programming.
This class will teach Object-Oriented programming in C++ as well as software development methodologies that enable programmers to work with large projects and many individuals.

## Goals

By the end of this semester, you will be able to:

- Generate a design document describing an approach to solve a given program definition
- Predict the output of Object-Oriented C++ code
- Identify syntax errors
- Identify code matching a given output example
- Identify code matching a given output description
- Identify the best design for a given problem
- Write Object-Oriented C++ code conforming to a problem definition
- List and define the terms and concepts of Object-Oriented design

These goals will be explored in the context of `C++` using the Linux operating system.

## Course layout

This course will be broken into four units:

1. **Using Classes**. This is a preparatory unit, ensuring we have the programming skills to learn ObjectOriented programming and to lay the foundation for the topics to come.
2. **Encapsulation**. Our first undertaking into the world of Object-Oriented programming, the encapsulation unit introduces us to classes. Here we will learn how to design a program with classes and create our first class.
3. **Inheritance & Polymorphism**. With knowledge of how to create and use classes, the next unit is concerned with leveraging the relationships between similar classes to minimize code duplication and to provide a new perspective on class design.
4. **Abstract Types**. After spending virtually the entire semester concerning ourselves with designing and creating new data types, the final unit is about defining functions and classes that operate independent of the data type passed to them.

# How to use this textbook 

This textbook is closely aligned with CS 165. All the topics, problems, and technology used in CS 165 are described in detail with these pages.

## Sam and Sue

You may notice two characters present in various sections of this text. They embody two common archetypes representative of people you will probably encounter in industry.

> [!Danger] Sue's Tips
> ![Sue](../../.vscode/assets/sue.png){.sue}
> Sue is a pragmatist. She cares only about getting the job done at a high quality level and with the minimum amount of effort. In other words, she cares little for the art of programming, focusing instead on the engineering of the craft.
> Sue's Tips tend to focus on the following topics:
> 
> - Pitfalls: How to avoid common programming pitfalls that cause bugs
> - Effort: How to do the same work with less time and effort
> - Robustness: How to make code more resistant to bugs
> - Efficiency: How to make code execute with fewer resources


> [!tldr] Sam's Corner
> ![Sam](../../.vscode/assets/sam.png){.sam}
> Sam is a technology nerd. He likes solving hard problems for their own sake, not necessarily because they even need to be solved. Sam enjoys getting to the heart of a problem and finding the most elegant solution. It is easy for Sam to get hung up on a problem for hours even though he found a working solution long ago.
> The following topics are commonly discussed in Sam's Corner:
> 
> - Details: The details of how various operations work, even though this knowledge is not necessary to get the job done
> - Tidbits: Interesting tidbits explaining why things are the way they are

Neither Sue's Tips nor Sam's Corner are required knowledge for this course. However, you may discover your inner Sam or Sue and find yourself reading one of their columns.

## Needing Help

Occasionally, each of us reaches a roadblock or feels like help is needed. This textbook offers two ways to bail yourself out of trouble.

If you find you are not able to understand the problems we do in class, work through them at home before class. This will give you time for reflection and help ask better questions in class.

If you find the programming problems to be too hard, take the time to type out all the examples by hand. Once you finish them, work through the challenge associated with each example. There is something about typing code by hand that helps it seep into our brains. I hope this helps.