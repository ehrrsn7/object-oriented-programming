<div id="page-336" style="
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    min-height: 9in;
    padding: 0.5in 0;
    margin: 0;
    justify-content: flex-end;
">
<h1 style="width: 100%; text-align: right">Appendix</h1>

<div id="table-of-contents" style="margin-left: 2em">
<a href="#main" alt="">A. Elements of Style &nbsp;  <span style="monospace">...............................................................................................................................</span> 337</a><br>
<a href="./Appendix-B-C++-Reference-Guide.md#main" alt="">B. C++ Syntax Reference Guide &nbsp; <span style="monospace">.............................................................................................................</span> 342</a><br>
<a href="./Appendix-C-Glossary.md#main" alt="">C. Glossary &nbsp; <span style="monospace">.............................................................................................................................................</span> 346</a><br>
<a href="./Appendix-D-Index.md#main" alt="">D. Index &nbsp; <span style="monospace">...................................................................................................................................................</span> 361</a><br>
</div>

<div style="width: 100%; page-break-after: always; margin-top: auto; text-align: left;">
<strong>Page 336</strong>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<!-- ! Typo -->
4.6 Standard Template Library
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Appendix
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
C++ Object Oriented Programming
</div>

</div>

<div id="page-337" style="
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    min-height: 9in;
    padding: 0.5in 0;
    margin: 0;
    justify-content: start;
">

<h1 id="main">A. Elements of Style</h1>

While the ultimate test of a program is how well it performs for the user, the value of the program is greatly limited if it is difficult to understand or update. For this reason, it is very important for programmers to write their code in the most clear and understandable way possible. We call this “programming style.”

## Elements of Style

Perhaps the easiest way to explain coding style is this: **give the bugs no place to hide**. When our variable names are clearly and precisely named, we are leaving little room for confusion or misinterpretation. When things are always used the same way, then readers of the code have less difficulty understanding what they mean.

There are four components to our style guidelines: variable and function names, spacing, function and program headers, general comments, and other standards.

## Variable and Function Names

The definitions of terms and acronyms of a software program typically consist of variable declarations. While variables are declared in more than one location, the format should be the same. Using descriptive identifiers reduces or eliminates the need for explanatory comments. For example: `sum` tells us we are adding something; `sumOfSquares` tells us specifically what we are adding. Use of descriptive identifiers also reduces the need for comments in the body of the source code. For example: `sum += x * x;` requires explanation. On the other hand, `sumOfSquares += userInput * userInput;` not only tells us where the item we are squaring came from, but also that we are creating a sum of the squares of those items. If identifiers are chosen carefully, it is possible to write understandable code with very few, if any, comments. The following are the University conventions for variable and function names:

| Identifier | Example         | Explanation                                                                                                                                                   |
| ---------- | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Variable   | `sumOfSquares`  | Variables are nouns so it follows that variable names should be nouns also. All the words are TitleCased except the first word. We call this style camelCase. |
| Function   | `displayDate()` | Functions are verbs so it follows that function names should also be verbs. Like variables, we camelCase funcitons.                                           |
| Constant   | `PI`            | Constants, include `#define`s are ALL_CAPS with underscore between the words.                                                                                 |
| Data types | `Date`          | Classes, enumeration types, type-defs, and structures are TitleCased with the first letter of each word capitalized. These are CS 165 constructs.             |

## Spacing

During the lexing process, the compiler removes all the spaces between keywords (such as `int`, `for`, or `if`) and operators (such as `+` or `>=`). To make the code human-readable, it is necessary to introduce spaces in a consistent way. The following are the University conventions for spaces:

<div style="width: 100%; page-break-after: always; margin-top: auto; text-align: right;">
C++ Object Oriented Programming
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Appendix
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
A. Elements of Style
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<strong>Page 337</strong>
</div>
</div>

<div id="page-338" style="
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    min-height: 9in;
    padding: 0.5in 0;
    margin: 0;
    justify-content: start;
">

<table>
<thead>
<tr>
<th>Rule</th>
<th>Example</th>
<th>Explanation</th>
</tr>
</thead>
<tbody>
<tr>
<td>Operators</td>
<td><code>tempC = 5.0 / 9.5 (tempF – 32.0)</code></td>
<td>There needs to be one space between all operators, including arithmetic (<code>+</code> and <code>%</code>), assignment (<code>=</code> and <code>+=</code>) and comparison (<code>&gt;=</code> and <code>!=</code>).</td>
</tr>
<tr>
<td>Indention</td>
<td style="min-width: 320px">

```cpp
{
    int answer = 42;
    if (answer > 100)
        cout << "Wrong answer!";
}
```

</td>
<td>With every level of indention, add three white spaces. Do not use the tab character to indent.</td>
</tr>
<tr>
<td>Functions</td>
<td></td>
<td>Put one blank line between functions. More than one results in unnecessary scrolling, less feels cramped</td>
</tr>
<tr>
<td>Related code</td>
<td>

```cpp
// get the data
float income;
cout << "Enter income: ";
cin  >> income;
```

</td>
<td>Much like an essay is sub-divided into paragraphs, a function can be sub-divided into related statements.  Each statement should have a blank line separating them.</td>
</tr>
</tbody>
</table>

## Function and Program Headers

It takes quite a bit of work to figure out what a program or function is trying to do when all the reader has is the source code. We can simplify this process immensely by providing brief summaries. The two most common places to do this are in function and program headers.

A function header appears immediately before every function. The purpose is to describe what the program does, any assumptions  made  about the  input parameters, and describe  the output.  Ideally, a programmer should need no more information than is provided in the header before using a function.  An example of a function header is the following:

```cpp
/******************************************************
 * GET YEAR
 * Prompt the user for the current year. Error checking
 * will be performed to ensure the year is valid
 *    INPUT:  None (provided by the user)
 *    OUTPUT: year
 ******************************************************/
```

### Program Header Example

A program header appears at the beginning of every file. This identifies what the program does, who wrote it, and a brief description of what it was written for. Our submission program reads this program header to determine how it is to be turned in.  For this reason, it is important to start every program with the template provided at `/home/cs165/template.cpp`.  The header for Assignment 1.0 is:

```cpp
/***********************************************************************
 * Program:
 *    Assignment 10, Hello World
 *    Brother Helfrich, CS165
 * Author:
 *    Sam Student
 * Summary:
 *    Display the text “Hello world” on the screen.
 *    Estimated:  0.7 hrs
 *    Actual:     0.5 hrs
 *      I had a hard time using emacs.
 ************************************************************************/
```

<div style="width: 100%; page-break-after: always; margin-top: auto; text-align: left;">
<strong>Page 338</strong>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
A. Elements of Style
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Appendix
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
C++ Object Oriented Programming
</div>
</div>

<div id="page-339" style="
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    min-height: 9in;
    padding: 0.5in 0;
    margin: 0;
    justify-content: start;
">

## General Comments

We put comments in our code for several reasons:
- To describe what the next few lines of code do
- To explain to the reader of the code why code was written a certain way
- To write a note to ourselves reminding us of things that still need to be done
- To make the code easier to read and understand

Since a comment can be easily read by a programmer and source code, in many cases, must be decoded, one purpose of comments is to clarify complicated code. Comments can be used to convey information to those who will maintain the code. For example, a comment might provide warning that a certain value cannot be changed without impacting other portions of the program. Comments can provide documentation of the logic used in a program. Above all else, comments should add *value* to the code and should not simply restate what is obvious from the source code. The following are meaningless comments and add no value to the source code:

```cpp
int i; // declare i to be an integer
i = 2; // set i to 2
```

On the other hand, the following comments add value:

```cpp
int i; // indexing variable for loops
i = 2; // skip cases 0 and 1 in the loop since they were processed earlier
```

With few exceptions, we use line comments (`//`) rather than block comments (`/* ... */`) inside functions. Please add just enough comments to make your code more readable, but not so many that it is overly verbose. There is no hard-and-fast rule here.

“Commenting out” portions of the source code can be an effective debugging technique. However, these sections can be confusing to those who read the source code. The final version of the program should not contain segments of code that have been commented out.

## Other Standards

Because of the way printers and video displays handle text, readability is improved by keeping each line of code less than 80 characters long.

Subroutines and classes should be ordered in a program such that they are easy to locate by the reader of the source code. For larger programs, an alphabetical arrangement works well. For shorter programs, following the order in which the subroutines are invoked or objects are instantiated is useful.

Each curly brace should be on its own line; this makes them easier to match up.

Just as one would expect correct spelling in a technical paper, one should also find correct spelling within a program

<div style="width: 100%; page-break-after: always; margin-top: auto; text-align: right;">
C++ Object Oriented Programming
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Appendix
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
A. Elements of Style
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<strong>Page 339</strong>
</div>

</div>

<div id="page-340" style="
    display: flex;
    flex-direction: column;
    align-items: flex-start;
    min-height: 9in;
    padding: 0.5in 0;
    margin: 0;
    justify-content: start;
">
<h2 style="margin-top: 0;">Style Checklist</h2>

<table>
<tbody>
<tr>
<td><br>

**Comments**
- program introductory comment block
- identify program
- identify instructor and class
- identify author
- brief explanation of the program
- brief explanation of each class
- brief explanation of each subroutine

**Variable declarations**
- declared on separate lines
- comments (if necessary)

**Identifiers**
- descriptive
- correct use of case
- correct use of underscores

</td>
<td>

**White space**
- white space around operators
- white space between subroutines
- white space after key words
- each curly brace on its own line

**Indentation**
- statements consistently indented
- block of code within another block of code further indented

**General**
- code appropriately commented
- each line less than 80 characters long
- correct spelling
- no unused (e.g. commented out) code

</td>
</tr>
</tbody>
</table>

## Example 1: Method

The following is an example of a class method with excellent style.

```cpp
/**********************************************************************
 * Extraction    cin >> x;
 * RETURN:    istream by reference  (so we can say (cin >> x) >> y;)
 * PARAMETER: istream by reference  (we do not want a copy of cin)
 *            by reference          (no copies but we do want to change this)
 *********************************************************************/
istream & operator >> (istream & in, Card & card)
{
   // input comes in the form of a string
   string input;
   in >> input;

   // do the actual work
   card.parse(input);
   assert(card.validate());

   // return the input stream
   return in;
}
```

<div style="width: 100%; page-break-after: always; margin-top: auto; text-align: left;">
<strong>Page 340</strong>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Appendix
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
A. Elements of Style
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
C++ Object Oriented Programming
</div>

</div>

## Example 2: Header

The following example is a header file with excellent style.

```cpp
/***********************************************************************
 * This file describes the WRITE interface, a class
 *      designed to write data to a file
 ************************************************************************/
#ifndef WRITE_H
#define WRITE_H

#include <fstream>        // necessary for the ofstream object
#include <string>         // necessary for the string parameters

/******************************************************
 * WRITE
 * This class will write text to a file without having
 * the client have to worry about opening or closing it
 ******************************************************/
class Write
{
   public:
      Write() : isOpen(false)      {       }
      Write(const std::string & fileName);
     ~Write();

      void writeToFile(const std::string & text);

   private:
      bool          isOpen;           // did we successfully open the file?
      std::ofstream fout;             // the file stream object
};
#endif // WRITE_H
```

## Example 3: Makefile

The following example is a makefile with excellent style.

```makefile
##############################################################
# Program:
#     Example 1.5, Complex Numbers demo
#     Brother Helfrich, CS165
# Author:
#     Br. Helfrich
# Summary:
#     This program will demonstrate how to break a large program into several files
##############################################################

##############################################################
# The main rule
##############################################################
a.out: complexTest.o complex.o
        g++ -o a.out complexTest.o complex.o
        tar -cf example14.tar *.h *.cpp makefile

##############################################################
# The individual components
#      complex.o      : Compile only if complex.cpp or complex.h changed
#      complexTest.o  : Compile only if complextTest.cpp or complex.h changed
##############################################################
complexTest.o: complexTest.cpp complex.h
        g++ -c complexTest.cpp

complex.o: complex.cpp complex.h
        g++ -c complex.cpp
```

<div style="width: 100%; page-break-after: always; margin-top: auto; text-align: right;">
C++ Object Oriented Programming
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
Appendix
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
A. Elements of Style
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; | &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;
<strong>Page 341</strong>
</div>
