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

Quantifiers are used to limit the amount of characters you want to search for. An example of a quantifier is ({ 4, 17 }). This means that the search for the pattern will have to include a minimum of four characters and a maxim of seventeen. When quantifiers are used, they want to find as many examples of the pattern as possible. This can generate a large amount of results. A way to fix this is to have it end in a question mark (?). A question mark makes the program search for as few matches as possible. In the example code, if we add ({ 4, 17 }) to ^[+-]?([1-9]\d({4,17}); the ({ 4, 17 }) is a quantifier.

### Grouping Constructs

Grouping constructs is when you separate parts of the regex into sections so that each part can be tested. You separate each section in the code using parentheses (). For example our code ^[+-]?([1-9]\d$ can be broken into (^[+-]?) ([1-9]\d$). With these two sections, the user can ensure that the regex is searching for the right parameters.

### Bracket Expressions

Bracket expressions look like a bracket ([]) in regex. These represent the range of characters we want to search for. If we had the example [and] the regex will search for anything that has any single character in that list. For instance apple and neat would be highlighted. 
 
Brackets can be used with a dash as well. These represent a range in the search parameters. A bracket can also include anchors and other regex components. In our example ^[+-]?([1-9]\d$, [1-9] is a bracket expression. In this bracket expression we are searching for a number between one and nine. 

### Character Classes

### The OR Operator

### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
