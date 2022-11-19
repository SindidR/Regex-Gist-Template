# Matching an Email(Regex)

This is a overview of the Regex for "Matching an Email".
## Summary
The Regular Expression or Regex I am showcasing today is a search pattern for:
"Matching an Email":
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
## Table of Contents
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Boundaries](#boundaries)
## Regex Components
The Regular Expression showcased uses literal notation instead of using RegExp. You can see this by looking at the regex and seeing the forward slashes in the beggining and the end. If it were to use a Reg Exp constructor it would be in single quotation marks.
"Matching an Email":
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
### Anchors
The Anchors in this instance are ^ and $. The ^ anchor serves as a starting point and the $ anchor serves as a ending point with the string in between which in our case is ([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6}).
### Quantifiers
1st Quantifier: {2,6}
This quantifier sets the limit for the number of characters in the bracket expression in the group it is in. In our case our quantifier is {2,6} which means the bracket expression [a-z\.] can only have 2-6 characters. The reason why this quatifier is not affecting the rest of the regex is because it is grouped in with parenthesis as you can see here ([a-z\.]{2,6}). So in short the quantifier {2,6} puts a 2-6 character limit on [a-z\.].
### Character Classes
[\da-z\.-]
The character class used in this expression is \d which matches any single character that is a digit.
### Flags
Flags affect the search of the Regex which are i, g, m, s, u, y. The i flag is case-insensitive, g flag looks for all matches, m flag is multiline, s flag enables "dotall", u flag enables full unicode support, and y flag is "sticky" mode.
### Grouping and Capturing
The "Matching a Email" Regex is grouped in 3 sections. These sections are the strings in the parenthesis. In our case the sections are:
1st Group: ([a-z0-9_\.-]+)
2nd Group: ([\da-z\.-]+)
3rd Group: ([a-z\.]{2,6})
### Bracket Expressions
Bracket Expression match anything within a pair of brackets if we look at our regex we can see there are 3 Bracket Expressions which are:
1st Bracket Expression: [a-z0-9_\.-]
2nd Bracket Expression: [\da-z\.-]
3rd Bracket Expression: [a-z\.]
## Author
This Regex Tutorial on "Matching an Email" has been created by Sindid Reedh and can be reached on Github: https://github.com/SindidR.
