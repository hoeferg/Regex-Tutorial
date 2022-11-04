# Regular Expressions (regex)
 
A regular expression is a wonderful tool that a coder can use. This search parameter is similar to control f but with one major difference. Instead of searching for a set of characters, a regular expression is searching for a pattern in the code. This code could be a string of numbers, a set amount of characters, or many other variations. 

## Summary
 
The regular expression (which will be referred to as regex from now on), is meant to be used to help find a pattern within code. This will allow the coder to find the pattern that they need to make edits to. To assist in the understanding of regex, I will be referring to the following regex: ^[+-]?([1-9]\d$. In the following section this regex will be broken down to its components and each component will be explained.


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

Regex is made up of many different components. The components of a regex include single characters, wild cards, bracket expressions, control characters, escape character sets, anchors, and recursive expansion. All of these have an overall term of atoms. These atoms are what create each individual part of a regex. In the regex example ^[+-]?([1-9]\d$, every single individual part is an atom.

### Anchors

Anchors are the characters that signify the start or the end of the string. A carrot (^) anchor represents the start of a string. The character that follows the carrot will be the first part of the pattern that the code starts to look for. For instance, in the example ^[+-]?([1-9]\d$, the regex is started by a carrot so that the beginning of the search will start there.
 
The other anchor character is a dollar sign ($). The dollar sign is used at the end of a regex. This tells the program that this is the end of the search parameter that it is looking for. In ^[+-]?([1-9]\d$, it ends in a dollar sign to represent the end of the search parameter. 

### Quantifiers

### Grouping Constructs

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
