# Match an Email - Regex Tutorial

This is a regular expression used to validate email addresses.

## Summary

The regular expression /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/ is used to validate email addresses where the username can have lowercase letters, digits, underscore, dots, hyphens, the domain name can have digits, lower case letters, dots and hyphens and the length should be between 2and 6 characters.

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
/^ is the starting anchor that asserts the start of the string. The $/ is the end of the string anchor that asserts the end of the string.

### Quantifiers
The quantifier in this regex includes the + operator which means one or more 
of the characters preceding the quantifier is allowed in this context [a-z0-9_.-]+ one or more of the lower case letter, digit, underscore, dot and hyphen is allowed. The other quantifier is the {2,6} which indicates that the email address should contain 2 and 6 lowercase letters and dots.
### Grouping Constructs
Grouping constructs are used to capture and extract specific parts of the email address.
- Group 1: ([a-z0-9_\.-]+)
    This part captures the username part of the email address. 
- Group 2: ([\da-z\.-]+)
    This part captures the domain name part of the email address. 
- Group 3: ([a-z\.]{2,6})
    This part captures the top level part of the domain (TLD) part of the email address. It matches the lowercase letters and dots with a length between 2-3 characters

### Bracket Expressions
Bracket expressions are used to define a set of characters.
- [a-z0-9_\.-] The first part a-z matches the lowercase letter, 0-9 digits, _\.- underscores, dots and hyphens.
- [\da-z\.-] The character class matches lowercase letters, dots and hyphens.
- [a-z\.] this matches any lower case letters and  literal dot.

### Character Classes
\d matches any digits, it is a shorthand character class that represents a single digit. It is equivalent to the character range [0-9]

### Character Escapes
\. Here the `\` character Escapes the dot character, allowing it to match a literal dot.

## Author

Learn more about the author of this tutorial and find a link to their GitHub profile.
