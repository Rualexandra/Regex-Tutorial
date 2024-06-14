# Email Regex Tutorial

Regular expressions (regex) are powerful tools for matching patterns in text. This tutorial will break down a specific regex pattern used to validate email addresses.

## Summary
The regex pattern we'll be analyzing is used to verify that user input is a valid email address:/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/
This pattern ensures that the email starts with a series of characters, followed by the @ symbol, a domain name, and a valid top-level domain.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Boundaries](#boundaries)


## Regex Components

### Anchors
Anchors are used to specify the position within a string where a match must occur.
#### In our regex: ^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$
- ^ asserts the position at the start of the string.
- $ asserts the position at the end of the string.


### Quantifiers
Quantifiers define how many instances of a character, group, or character class must be present in the input for a match to be found.
#### [a-z0-9_\.-]+
-  Where + specifies that the preceding element (any lowercase letter, digit, underscore, dot, or hyphen) must appear one or more times.

### Character Classes
Character classes allow you to match any one of several characters.
#### [a-z0-9_\.-]
- [a-z] matches any lowercase letter.
- [0-9] matches any digit.
- _ matches an underscore.
- \. matches a dot.
- The - matches a hyphen.


### Grouping and Capturing
Grouping and capturing are used to group multiple tokens together and to capture parts of the match for later use.
#### ([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})
- ([a-z0-9_\.-]+) captures the username part of the email.
- ([\da-z\.-]+) captures the domain name part.
- ([a-z\.]{2,6}) captures the top-level domain part.

### Bracket Expressions
Bracket expressions match any one of the enclosed characters.
#### [a-z0-9_\.-]
- This bracket expression matches any single character that is a lowercase letter, digit, underscore, dot, or hyphen.

### Boundaries
Boundaries ensure that the pattern matches a complete email address from start to finish.
- ^ at the start of the pattern.
- $ at the end of the pattern.


## Author

Alexandra Ruiz is a web development student who enjoys learning about new technologies and sharing knowledge with others. You can find more about Alexandra on her GitHub profile. 

- GitHub: https://github.com/Rualexandra
-Gist: https://gist.github.com/b84a22c00749206a9cc328d99ca0d9a9.git

