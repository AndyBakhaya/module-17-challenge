# Regular Expression- Matching Hex Values

This file is intended to explain a basis of Regular Expressions and how to use them to Match a Hex Value

## Summary

The following String is the Regex used to Match Hex Values

(  /^#?([a-f0-9]{6}|[a-f0-9]{3})$/  )

Refer to the TOC for each component

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

### Anchors

Anchors define either the beginning or the end of a string.
Most common examples being "/^" for the begining and "$/" for the ending

"/^#"
This is the begining anchor, the # means it's a HEX decimal rather than a normal decimal. 

### Quantifiers

Quantifiers are used to specify how many times the previous character is matched.

"/^#?" 
The ? is the quantifier in the String. It's stating that the # is optional at the begining of the string.

"{}"
The {} defines how many times the character is matched.
In our case {6} defines that there are 6 instances of the string containing letters a-f and numbers 0-9 "([a-f0-9])"

### Grouping Constructs

"([a-f0-9]{6}|[a-f0-9]{3})"

### Bracket Expressions

The Bracket Expression tells you what is being matched through a pattern of (alphabetic, numeric, special characters, etc..) defined in the brackets

"[a-f0-9]"
This pattern tells us that there are alphabetic characters from "a-f" and numberic characters from "0-9"

### Character Classes

The Character Classes are the paramaters inside the Bracket Expression that are being matched

"[a-f]" is one character class
"[0-9]" is another character class

### The OR Operator

"|"

"[a-f0-9]{6}|[a-f0-9]{3}"

### Flags

Flags change the way the regex searches.

i- ignore casing: case insensitive
g- global: searches all matches
s- dot all: "." matches a newline character
m- multiline: matches the start and end of the string and line
y- sticky: exact position
u- unicode: enables unicode support

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
Hi my name is Andy Bakhaya. I want to further expand my knowledge of computer science through school and browsing the internet.
My Github has projects I've worked on: https://github.com/AndyBakhaya
