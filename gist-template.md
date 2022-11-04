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

Character classes are a regex component that allows the user to match only one character out of several characters. For instance you can type gr[ae]y. The computer will highlight both gray and grey. Character classes can also be applied to numbers. For instance, in ^[+-]?([1-9]\d$ [1-9] will highlight a single digit that is within that range. The biggest use of this feature is to help find words even if they are misspelled

### The OR Operator

The or operator allows the user to search for a list of terms as a whole and by individual characteristics. The or operator looks like (|). For example, this|that|them is an or code that means the computer will highlight the word this and that and them. The words do not need to be connected and each section will be looked for independently from each other. An example of the code is (1|2|3):(4|5|6). This will look for the string 123:456 and 1:6. In the example, ^[+-]?([1-9]\d$, will be rewritten to look like the following: ^ |[+-]| |?([1-9]\d| $. This will make the computer find those patterns separate from the other part of the regex.

### Flags

Flags are added at the end of regex to add additional features. There are a total of six flags. The three most common are g, i, and m. The g flag means that the program should run a global search to find all possible matches. The i flag means that case should be ignored in the search. The m flag means an input should be treated as multiple lines. Using the example code ^[+-]?([1-9]\d$, the user can add a g at the end and make the regex look like this: ^[+-]?([1-9]\d$ -g. This will search for the matching pattern globally.

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
