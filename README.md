# 17 Computer Science for JavaScript: Regex Tutorial

Developers write code, but they also *write about code*. Take a moment to search the web for tutorials about any of the subjects you’ve learned so far in this course. You’re likely to find thousands of tutorials written by developers of all skill levels, including junior developers&mdash;like yourself!

My assignment is to create a tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does. You'll use the template provided in the starter code to create your walkthrough.

## Summary

```
I will be breaking down the definitions on how to match a search pattern of an email address using regex.
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`
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

This is the regex pattern used to match an email address.
```
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
```

### Anchors

To match an email the anchors used are the following:

`^` is used to indicate the beginning position of the pattern. <br />
`$` is used to indicate the end position of the pattern.

### Quantifiers

Quantifiers used are the following: <br />

`{}` is used to show the amount of characters matching. <br />
`{2,6}` the 2 indicates the minimum amount, and the 6 being the maximum amount of characters. <br />
`a-z` is used to match if there are any letters from a-z. <br />
`0-9` is also used to match if there are any digits. <br />
`_`, `.`, and `-` is also used to find if the email has any underscore, period, and dash. <br />
`+` is used to connect the email name, followed by email server, then ends with the domain; `.com`, `.org`, `.info`, etc.

### Grouping Constructs

`()` are used to group the patterns followed by a `+` to add more pattern. <br />
The first grouping constructs used is the `([a-z0-9_\.-]+)` that indicates that the first part of the pattern will be the email name followed by `([\da-z\.-]+)` that indicates the email server then ends with `([a-z\.]{2,6})` which indicates the domain name.

### Bracket Expressions

Brackets are used to contain patterns as a set. <br />
`[]` is used in the first part of the email with `a-z`, `0-9`, `_`, `.`, `-`. It is necessary to validate the email name if it contains any letters, digits, underscore, period, or dash.

### Character Classes

Character Classes are the ones that appears in between square brackets. <br />
The brackets used in the expression is the one that validates the email name, email server, and domain. <br />
This example of Character Class `([a-z\.]{2,6})` validates the domain with a minimum of 2 up to a maximum of 6.

### The OR Operator

OR expression is not used in this tutorial since there is no use for that expression, since we look for any characters. <br />
OR operator is used with `|` symbol. If what we're matching is a specific domain name with `.com`, `.org`, and `.info` for example; we could write `.(com|org|info)`.

### Flags

There are no flags on the email address pattern since we do not need it. <br />
There are 6 flags we can use and these are the following: <br />

`g` This is a flag that looks for all matches. <br />
`m` This is a flag that enables multiline mode. <br />
`i` This is a flag that search case-insensitive. <br />
`s` This is a flag that allows a dot to match `/n` (newline) character. <br />
`u` This is a flag that enables correct processing of rare characters like `©`, `™`, or emojis. <br />
`y` This is a flag that searches the exact position in the text. <br />

 With these descriptions, now it makes all sense why flags are not used in the pattern.

### Character Escapes

`\` is used as a character escape. The backslash in a regular expression precedes a literal character. You also escape certain letters that represent common character classes, such as `\w` for one word character or `\s` for one space.

## Author

You can view all my work at Github with this link.
https://github.com/cmempalmado

---
Copyright © [2022] [Christian Empalmado]

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the `Software`), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED `AS IS`, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.