# 17 Computer Science for JavaScript: Regex Tutorial

Developers write code, but they also *write about code*. Take a moment to search the web for tutorials about any of the subjects you’ve learned so far in this course. You’re likely to find thousands of tutorials written by developers of all skill levels, including junior developers&mdash;like yourself!

My assignment is to create a tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does. You'll use the template provided in the starter code to create your walkthrough.

## Summary

```
I will be breaking down how to match a search pattern of an email address using regex.
"/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/"
```

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components
```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

### Anchors

To match an email the anchors used are the following:
"^" is used to indicate the beginning position of the pattern.
"$" is used to indicate the end position of the pattern.


### Quantifiers

Quantifiers used are the following:
"{2,6}" the 2 indicates the minimum amount, and 6 being the maximum amount of characters.
"a-z" is used to match if there are any letters from a-z.
"0-9" is also used to match if there are any digits.
"_", ".", and "-" is also used to find if the email has any underscore, period, and dash.
"+" is used to connect the email name, followed by the domain name, then ends with the domain; ".com", ".org", ".info", etc.


### Grouping Constructs

```
"()" are used to group the patterns followed by a "+" to add more pattern.
The first grouping used is the ([a-z0-9_\.-]+)
```

### Bracket Expressions

```

```

### Character Classes

```

```

### The OR Operator

```

```

### Flags

```

```

### Character Escapes

```

```

## Author


---
Copyright © [2022] [Christian Empalmado]

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.