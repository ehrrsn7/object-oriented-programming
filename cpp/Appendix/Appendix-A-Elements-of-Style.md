<style>
   /* VS-Code Markdown Preview-Specific Styles */
   pre:not(.hljs), pre.hljs code > div {
      padding: 4px 1em;
      margin: 0;
      border-radius: 3px;
      overflow: auto;
   /* Add a copy button to all code blocks */
   pre code {
      position: relative;
      display: block;
      padding-right: 3em;
   }
   .copy-btn {
      position: absolute;
      top: 8px;
      right: 8px;
      background: #0078d4;
      color: #fff;
      border: none;
      border-radius: 3px;
      padding: 2px 8px;
      font-size: 0.9em;
      cursor: pointer;
      opacity: 0.7;
      transition: opacity 0.2s;
      z-index: 10;
   }
   .copy-btn:hover {
      opacity: 1;

   :root {
      --scale-difference: 15%;
      zoom: 85%;
   }

   div::-webkit-scrollbar {
      display: none;
   }
</style>

<div id="Appendix-A-Elements-of-Style" style="
   display: block;
   flex-flow: column;
   justify-content: center;
   align-items: stretch;
   width: 100%;
   padding: 0;
   margin: 0;
   margin-left: -4em;
">

<div class="page" id="page-336" style="
   display: flex;
   flex-direction: column;
   font-size: calc(100% - var(--scale-difference));
   padding: 2em;
   margin: 0 auto;
   width: 8.5in;
   min-height: 11in;
   box-sizing: border-box;
   overflow-x: scroll;
   height: 11in;
   overflow-y: scroll;
   scrollbar-width: none;         /* Firefox */
   -ms-overflow-style: none;      /* IE/Edge  */
   page-break-after: always;
">

<div class="body" style="display: flex; flex-direction: column; flex-grow: 1">

<div id="topic-header" style="
   width: 100%;
   color: white;
   padding: 40px 0 0 0;
   background-color: rgb(0, 96, 232); /* Fallback */
   background-image: url('.etc/assets/topic-header.png')
">
<h1 style="width: 100%; text-align: right; padding-right: 1em;">

Appendix
$\quad$

</h1>
</div>

<div id="table-of-contents" style="
   display: flex;
   flex-direction: column;
   padding: 0;
   padding-left: 1in;
   padding-top: 1in;
   margin-left: -1in;
   margin-top: -1in;
   margin: 0 auto;
   width: 6in;
   max-width: calc(100% - 2in);
">
<a href="#page-337" alt="">
<div style="
   display: inline-flex;
   flex-direction: row;
   flex-wrap: nowrap;
   width: 100%;
   overflow-x: hidden;
">
   <span style="white-space: nowrap;">A. Elements of Style</span>
   <span style="
      flex-grow: 1;
      overflow: hidden;
      white-space: nowrap;
      text-align: right;
      font-family: monospace;
   ">
      ........................................................................
   </span>
   <span>337</span>
</div>
</a>
<a href="./Appendix-B-C++-Reference-Guide.md#page-342" alt="">
<div style="
   display: inline-flex;
   flex-direction: row;
   flex-wrap: nowrap;
   width: 100%;
   overflow-x: hidden;
">
   <span style="white-space: nowrap;">
      B. C++ Syntax Reference Guide  $\quad
   </span>
   <span style="
      flex-grow: 1;
      overflow: hidden;
      white-space: nowrap;
      text-align: right;
      font-family: monospace;
   ">
      ........................................................................
   </span>
   <span>342</span>
</div>
</a>
<a href="./Appendix-C-Glossary.md#page-346" alt="">
<div style="
   display: inline-flex;
   flex-direction: row;
   flex-wrap: nowrap;
   width: 100%;
   overflow-x: hidden;
">
   <span style="white-space: nowrap;">C. Glossary  $\quad</span>
   <span style="
      flex-grow: 1;
      overflow: hidden;
      white-space: nowrap;
      text-align: right;
      font-family: monospace;
   ">
      .............................................................................
   </span>
   <span>346</span>
</div>
</a>
<a href="./Appendix-D-Index.md#page-361" alt="">
<div style="
   display: inline-flex;
   flex-direction: row;
   flex-wrap: nowrap;
   width: 100%;
   overflow-x: hidden;
">
   <span style="white-space: nowrap;">D. Index  $\quad</span>
   <span style="
      flex-grow: 1;
      overflow: hidden;
      white-space: nowrap;
      text-align: right;
      font-family: monospace;
   ">
      ..............................................................................
   </span>
   <span>361</span>
</div>
</a>
</div> <!-- End Table of Contents -->

</div class="body">

<div class="footer" style="width: 100%; margin-top: auto; text-align: left;">
   <strong>Page 336</strong>
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   <!-- ! Typo -->
   4.6 Standard Template Library
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   Appendix
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   C++ Object Oriented Programming
</div>

</div> <!-- End of Page -->


<div class="page" id="page-337" style="
   display: flex;
   flex-direction: column;
   font-size: calc(100% - var(--scale-difference));
   padding: 2em;
   margin: 0 auto;
   width: 8.5in;
   min-height: 11in;
   box-sizing: border-box;
   overflow-x: scroll;
   height: 11in;
   overflow-y: scroll;
   scrollbar-width: none;         /* Firefox */
   -ms-overflow-style: none;      /* IE/Edge  */
   page-break-after: always;
">

<div class="body" style="display: flex; flex-direction: column; flex-grow: 1">

<div id="topic-header" style="
   width: 100%;
   color: white;
   padding: 40px 0 0 0;
   background-color: rgb(0, 96, 232); /* Fallback */
   background-image: url('.etc/assets/topic-header.png')
">
   <h1 style="width: 100%; text-align: right; padding-right: 1em;">
      Appendix
       $\quad
   </h1>
</div>

<h1 id="main">A. Elements of Style</h1>

While the ultimate test of a program is how well it performs for the user,
the value of the program is greatly limited if it is difficult to understand
or update. For this reason, it is very important for programmers to write
their code in the most clear and understandable way possible.
We call this “programming style.”

## Elements of Style

Perhaps the easiest way to explain coding style is this:
**give the bugs no place to hide**.
When our variable names are clearly and precisely named, we are leaving
little room for confusion or misinterpretation.
When things are always used the same way, then readers of the code have less
difficulty understanding what they mean.

There are four components to our style guidelines: variable and function
names, spacing, function and program headers, general comments,
and other standards.

## Variable and Function Names

The definitions of terms and acronyms of a software program typically consist
of variable declarations. While variables are declared in more than one
location, the format should be the same.
Using descriptive identifiers reduces or eliminates the need for explanatory
comments.
For example: `sum` tells us
we are adding something; `sumOfSquares` tells us specifically what we are
adding.
Use of descriptive identifiers also reduces the need for comments in the body
of the source code.
For example: `sum += x * x;` requires explanation.
On the other hand, `sumOfSquares += userInput * userInput;`
not only tells us where the item we are squaring came from,
but also that we are creating a sum of the squares of those items.
If identifiers are chosen carefully,
it is possible to write understandable code with very few, if any, comments.
The following are the University conventions for variable and function names:

| Identifier | Example         | Explanation                                                                                                                                                   |
| ---------- | --------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Variable   | `sumOfSquares`  | Variables are nouns so it follows that variable names should be nouns also. All the words are TitleCased except the first word. We call this style camelCase. |
| Function   | `displayDate()` | Functions are verbs so it follows that function names should also be verbs. Like variables, we camelCase funcitons.                                           |
| Constant   | `PI`            | Constants, include `#define`s are ALL_CAPS with underscore between the words.                                                                                 |
| Data types | `Date`          | Classes, enumeration types, type-defs, and structures are TitleCased with the first letter of each word capitalized. These are CS 165 constructs.             |

## Spacing

During the lexing process, the compiler removes all the spaces between keywords (such as `int`, `for`, or `if`) and operators (such as `+` or `>=`). To make the code human-readable, it is necessary to introduce spaces in a consistent way. The following are the University conventions for spaces:

</div class="body">

<div class="footer" style="width: 100%; margin-top: auto; text-align: right;">
   C++ Object Oriented Programming
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   Appendix
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   A. Elements of Style
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   <strong>Page 337</strong>
</div>

</div> <!-- End of Page -->

<div class="page" id="page-338" style="
   display: flex;
   flex-direction: column;
   font-size: calc(100% - var(--scale-difference));
   padding: 2em;
   margin: 0 auto;
   width: 8.5in;
   min-height: 11in;
   box-sizing: border-box;
   overflow-x: scroll;
   height: 11in;
   overflow-y: scroll;
   scrollbar-width: none;         /* Firefox */
   -ms-overflow-style: none;      /* IE/Edge  */
   page-break-after: always;
">

<div class="body" style="display: flex; flex-direction: column; flex-grow: 1; font-size: 90%;">

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

A function header appears immediately before every function. The purpose is to describe what the program does, any assumptions made about the input parameters, and describe the output. Ideally, a programmer should need no more information than is provided in the header before using a function. An example of a function header is the following:

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

A program header appears at the beginning of every file. This identifies what the program does, who wrote it, and a brief description of what it was written for. Our submission program reads this program header to determine how it is to be turned in. For this reason, it is important to start every program with the template provided at `/home/cs165/template.cpp`. The header for Assignment 1.0 is:

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

</div class="body">

<div class="footer" style="width: 100%; margin-top: auto; text-align: left;">
   <strong>Page 338</strong>
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   A. Elements of Style
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   Appendix
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   C++ Object Oriented Programming
</div>

</div> <!-- End of Page -->

<div class="page" id="page-339" style="
   display: flex;
   flex-direction: column;
   font-size: calc(100% - var(--scale-difference));
   padding: 2em;
   margin: 0 auto;
   width: 8.5in;
   min-height: 11in;
   box-sizing: border-box;
   overflow-x: scroll;
   height: 11in;
   overflow-y: scroll;
   scrollbar-width: none;         /* Firefox */
   -ms-overflow-style: none;      /* IE/Edge  */
   page-break-after: always;
">

<div class="body" style="display: flex; flex-direction: column; flex-grow: 1">

## General Comments

We put comments in our code for several reasons:

- To describe what the next few lines of code do
- To explain to the reader of the code why code was written a certain way
- To write a note to ourselves reminding us of things that still need to be done
- To make the code easier to read and understand

Since a comment can be easily read by a programmer and source code, in many cases, must be decoded, one purpose of comments is to clarify complicated code. Comments can be used to convey information to those who will maintain the code. For example, a comment might provide warning that a certain value cannot be changed without impacting other portions of the program. Comments can provide documentation of the logic used in a program. Above all else, comments should add _value_ to the code and should not simply restate what is obvious from the source code. The following are meaningless comments and add no value to the source code:

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

</div class="body">

<div style="width: 100%; margin-top: auto; text-align: right;">
   C++ Object Oriented Programming
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   Appendix
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   A. Elements of Style
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   <strong>Page 339</strong>
</div>

</div> <!-- End of Page -->

<div class="page" id="page-340" style="
   display: flex;
   flex-direction: column;
   font-size: calc(100% - var(--scale-difference));
   padding: 2em;
   margin: 0 auto;
   width: 8.5in;
   min-height: 11in;
   box-sizing: border-box;
   overflow-x: scroll;
   height: 11in;
   overflow-y: scroll;
   scrollbar-width: none;         /* Firefox */
   -ms-overflow-style: none;      /* IE/Edge  */
   page-break-after: always;
">

<div class="body" style="display: flex; flex-direction: column; flex-grow: 1">

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

</div class="body">

<div class="footer" style="width: 100%; margin-top: auto; text-align: left;">
   <strong>Page 340</strong>
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   Appendix
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   A. Elements of Style
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   C++ Object Oriented Programming
</div>

</div> <!-- End of Page -->

<div class="page" id="page-341" style="
   display: flex;
   flex-direction: column;
   font-size: calc(100% - var(--scale-difference));
   padding: 2em;
   margin: 0 auto;
   width: 8.5in;
   min-height: 11in;
   box-sizing: border-box;
   overflow-x: scroll;
   height: 11in;
   overflow-y: scroll;
   scrollbar-width: none;         /* Firefox */
   -ms-overflow-style: none;      /* IE/Edge  */
   page-break-after: always;
">

<div class="body" style="display: flex; flex-direction: column; flex-grow: 1; font-size: 80%;">

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

</div class="body">

<div style="width: 100%; margin-top: auto; text-align: right;">
   C++ Object Oriented Programming
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   Appendix
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   A. Elements of Style
    $\quad $\quad $\quad $\quad $\quad |  $\quad $\quad $\quad $\quad $\quad
   <strong>Page 341</strong>
</div>

</div> <!-- End of Page -->

</div> <!-- End of chapter -->

<!-- Add a copy button to all code blocks -->
<script>
document.addEventListener("DOMContentLoaded", function () {
   // Select all code blocks inside <pre> elements
   document.querySelectorAll("pre code").forEach(function (codeBlock) {
      // Avoid duplicate buttons
      if (codeBlock.parentElement.querySelector(".copy-btn")) return;

      // Create the button
      var button = document.createElement("button");
      .className += " copy-btn";= "copy-btn";
      button.type = "button";
      button.innerText = "Copy";

      // Position the button relative to the <pre>
      var pre = codeBlock.parentElement;
      pre.style.position = "relative";
      button.style.position = "absolute";
      button.style.top = "8px";
      button.style.right = "8px";

      // Copy code to clipboard on click
      button.addEventListener("click", function () {
         var text = codeBlock.innerText;
         navigator.clipboard.writeText(text).then(function () {
            button.innerText = "Copied!";
            setTimeout(function () {
               button.innerText = "Copy";
            }, 1200);
         });
      });

      pre.appendChild(button);
   });
});
</script>