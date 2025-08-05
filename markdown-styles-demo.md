---
title: "Bootstrap-Enhanced Markdown Styles Demo"
description: "A comprehensive demonstration of all available Bootstrap-inspired Markdown styles for educational content"
course: "CS 165"
unit: "Demo"
chapter: "Styles-Demo"
tags:
  - markdown
  - bootstrap
  - styles
  - demo
  - educational-content
source:
  type: "Manual Creation"
  method: "Style Demonstration"
  original: "N/A"
  generated: "2025-08-04 16:30:00"
author: "Style Demo"
date: "2025-08-04"
---

# Bootstrap-Enhanced Markdown Styles Demo

This document demonstrates all the available Bootstrap-inspired styles for educational content. Use this as a reference when creating your course materials.

## Table of Contents

| Content Section | Page |
|:---|:---|
| Educational Blocks | 1 |
| Typography & Headings | 2 |
| Tables & Lists | 3 |
| Code & Math | 4 |
| Interactive Elements | 5 |

---

## Educational Content Blocks

### Warning Blocks

> [WARNING]
> ⚠️ **Warning:** \
> *This is a warning block using the standard format. It will be styled with Bootstrap danger colors (red theme).*

### Tip Blocks

> [TIP]
> 💡 **Tip:** \
> *This is a tip block that provides helpful advice. It uses Bootstrap info colors (cyan theme).*

### Info Blocks

> [INFO]
> ℹ️ **Info:** \
> *This is an informational block for additional context. It uses Bootstrap primary colors (blue theme).*

### Danger Blocks

> [DANGER]
> 🚨 **Danger:** \
> *This is a danger block for critical warnings. It uses a stronger red theme than warnings.*

### Success Blocks

> [SUCCESS]
> ✅ **Success:** \
> *This is a success block for positive reinforcement. It uses Bootstrap success colors (green theme).*

---

## Typography Demonstrations

# Heading 1 (2.5rem)
## Heading 2 (2rem)  
### Heading 3 (1.75rem)
#### Heading 4 (1.5rem)
##### Heading 5 (1.25rem)
###### Heading 6 (1rem)

### Text Formatting

This is **bold text** and this is *italic text*. You can also use ==highlighted text== for emphasis.

### Inline Code Styling

Here are examples of styled inline code:

- `code.warning`{.warning} - Warning-styled code
- `code.tip`{.tip} - Tip-styled code  
- `code.info`{.info} - Info-styled code
- `code.danger`{.danger} - Danger-styled code
- `code.success`{.success} - Success-styled code

```cpp {.warning}
hello
```

```cpp {.warning}
#include <iostream>
#include <string>

class Student {
private:
    std::string name;
    int id;

public:
    // Constructor
    Student(const std::string& studentName, int studentId) 
        : name(studentName), id(studentId) {}
    
    // Accessor methods
    std::string getName() const { return name; }
    int getId() const { return id; }
    
    // Display method
    void display() const {
        std::cout << "Student: " << name << " (ID: " << id << ")" << std::endl;
    }
};

int main() {
    Student student("John Doe", 12345);
    student.display();
    return 0;
}
```

### Enhanced Blockquotes

> This is a standard blockquote that has been enhanced with Bootstrap styling.
> It includes better padding, margins, and a subtle background color.

---

## Tables with Bootstrap Styling

| Feature | Description | Status |
|:--------|:------------|:-------|
| Warning Blocks | Red-themed alerts | ✅ Active |
| Tip Blocks | Cyan-themed helpful hints | ✅ Active |
| Info Blocks | Blue-themed information | ✅ Active |
| Success Blocks | Green-themed confirmations | ✅ Active |
| Enhanced Tables | Bootstrap-styled tables | ✅ Active |

### Complex Table Example

| Unit | Chapter | Topic | Difficulty | Estimated Time |
|:-----|:--------|:------|:-----------|:---------------|
| 1 | 1.0 | Using Objects | Beginner | 2 hours |
| 1 | 1.1 | Defensive Programming | Intermediate | 3 hours |
| 2 | 2.0 | Encapsulation Design | Intermediate | 4 hours |
| 2 | 2.1 | Building a Class | Advanced | 5 hours |

---

## Code Examples

### C++ Code Block with Syntax Highlighting

```cpp
#include <iostream>
#include <string>

class Student {
private:
    std::string name;
    int id;

public:
    // Constructor
    Student(const std::string& studentName, int studentId) 
        : name(studentName), id(studentId) {}
    
    // Accessor methods
    std::string getName() const { return name; }
    int getId() const { return id; }
    
    // Display method
    void display() const {
        std::cout << "Student: " << name << " (ID: " << id << ")" << std::endl;
    }
};

int main() {
    Student student("John Doe", 12345);
    student.display();
    return 0;
}
```

### Python Code Example

```python
class Calculator:
    def __init__(self):
        self.result = 0
    
    def add(self, value):
        self.result += value
        return self
    
    def multiply(self, value):
        self.result *= value
        return self
    
    def get_result(self):
        return self.result

# Usage example
calc = Calculator()
result = calc.add(5).multiply(3).get_result()
print(f"Result: {result}")  # Output: Result: 15
```

### JSON Configuration Example

```json
{
  "markdown.styles": [
    "./.vscode/markdown-styles.css",
  ],
  "markdown.preview.breaks": true,
  "markdown.preview.linkify": true,
  "markdown.preview.typographer": true
}
```

---

## Mathematical Expressions

### Inline Math
The quadratic formula is $x = \frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$.

### Block Math Equations

$$
\begin{align}
f(x) &= ax^2 + bx + c \\
f'(x) &= 2ax + b \\
\int f(x)\,dx &= \frac{ax^3}{3} + \frac{bx^2}{2} + cx + C
\end{align}
$$

### Algorithm Complexity

$$
\begin{cases}
O(1) & \text{constant time} \\
O(\log n) & \text{logarithmic time} \\
O(n) & \text{linear time} \\
O(n \log n) & \text{linearithmic time} \\
O(n^2) & \text{quadratic time}
\end{cases}
$$

---

## Interactive Elements

### Collapsible Sections

<details>
<summary>Click to expand: Advanced C++ Topics</summary>

#### Template Metaprogramming

Template metaprogramming is a metaprogramming technique in which templates are used by a compiler to generate temporary source code.

```cpp
template<int N>
struct Factorial {
    static const int value = N * Factorial<N-1>::value;
};

template<>
struct Factorial<0> {
    static const int value = 1;
};
```

</details>

<details>
<summary>Click to expand: Design Patterns</summary>

#### Singleton Pattern

```cpp
class Singleton {
private:
    static Singleton* instance;
    Singleton() {}

public:
    static Singleton* getInstance() {
        if (instance == nullptr) {
            instance = new Singleton();
        }
        return instance;
    }
};
```

</details>

---

## Educational Character Sections

### Sue's Tips

> [TIP]
> ![Sue](.vscode/assets/sue.png){width=50 align=right} 💡 **Sue's Tip:** \
> *Always use meaningful variable names and consistent formatting. Your future self (and your teammates) will thank you. Focus on writing code that works first, then optimize for readability.*

### Sam's Corner

> [INFO]
> ![Sam](.vscode/assets/sam.png){width=50 align=right} 🤓 **Sam's Corner:** \
> *Did you know that C++ templates are Turing complete? This means you can theoretically compute any computable function at compile time using only template metaprogramming techniques.*

---

## Lists and Organization

### Ordered Lists

1. **First Principle**: Encapsulation
   - Hide implementation details
   - Provide clean interfaces
   - Protect data integrity

2. **Second Principle**: Inheritance
   - Code reusability
   - Hierarchical relationships
   - Polymorphic behavior

3. **Third Principle**: Polymorphism
   - Runtime type binding
   - Interface consistency
   - Flexible design patterns

### Unordered Lists

- ✅ **Completed Topics**
  - Basic syntax and semantics
  - Control structures and functions
  - Arrays and pointers

- 🔄 **In Progress**
  - Object-oriented design
  - Template programming
  - STL containers

- 📋 **Upcoming**
  - Advanced templates
  - Design patterns
  - Performance optimization

### Task Lists

- [x] Set up development environment
- [x] Learn basic C++ syntax
- [ ] Master class design
- [ ] Implement inheritance hierarchies
- [ ] Practice template programming
- [ ] Complete final project

---

## Conclusion

This demo showcases all available Bootstrap-enhanced Markdown styles. The styles provide:

> [SUCCESS]
> ✅ **Benefits:** \
> *Professional appearance, consistent formatting, improved readability, and enhanced educational content presentation.*

### Quick Reference

| Style Type | Syntax | Use Case |
|:-----------|:-------|:---------|
| Warning | `> [WARNING]` | Important alerts |
| Tip | `> [TIP]` | Helpful advice |
| Info | `> [INFO]` | Additional context |
| Danger | `> [DANGER]` | Critical warnings |
| Success | `> [SUCCESS]` | Positive feedback |
| Highlight | `==text==` | Emphasis |
| Math | `$equation$` or `$$block$$` | Mathematical expressions |

---

*Happy writing with your enhanced Markdown styles! 🎉*

```cpp {.hello}
void helloWorld() {
    return;
}
```

> [WARNING]
> ⚠️ **Warning:** \
> *Your warning message here*
>
