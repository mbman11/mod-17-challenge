# Regex Expression Tutorial

This is a simple walkthrough detailing different components within a regular expression.


## Table of Contents

- [Regex Expression Tutorial](#regex-expression-tutorial)
  - [Table of Contents](#table-of-contents)
  - [Summary](#summary)
    - [Regex Components](#regex-components)
    - [Anchors](#anchors)
    - [Quantifiers](#quantifiers)
    - [OR Operator](#or-operator)
    - [Character Classes](#character-classes)
    - [Flags](#flags)
    - [Grouping and Capturing](#grouping-and-capturing)
    - [Bracket Expressions](#bracket-expressions)
    - [Greedy and Lazy Match](#greedy-and-lazy-match)
    - [Boundaries](#boundaries)
    - [Back-references](#back-references)
    - [Look-ahead and Look-behind](#look-ahead-and-look-behind)
  - [Author](#author)



## Summary

Below  is the regex expression I will be referencing in this tutorial.
 
 `/^<([a-z]+)([^<]+)*(?:>(.*)<\/\1>|\s+\/>)$/`




### Regex Components
There are many regex components in this regex such as: anchors, groups and capturing, OR operator, Quantifiers, character classes, back references, white space quantifier, escape sequences

### Anchors
^ signifies the start of a line.
$ signifies the end of a line.

### Quantifiers
the `+` sign means "one or more". So the `[a-z]+` means one or more lowercase letters from letters a to z. A quantifier in a regular expression specifies how many characters or group of characters should be matched.

### OR Operator
The `|` in this expression is an OR operator. The regex engine will try to match the pattern on the left side of the |, and if that doesn't work it will try to match the pattern on the right side.

### Character Classes
Character classes are used to match one character with a set of characters. In this regex expression `[a-z]` is a character class. it matches any lowercase letter from a to z.

### Flags
This regex does not have any flags in it. A flag specifies things like case sensitivity, ignore whitespace and more. 

### Grouping and Capturing
`([a-z]+)` is a capturing group. It matches one or more lowercase letters a to z inside the brackets < >. Parenthesis are used for grouping.

### Bracket Expressions
there are two bracket expressions in this regex. `[a-z]+` is an example of one bracket expression that matches one or more lowercase letters a to z.

### Greedy and Lazy Match
the `.*` within the regex is an example of a greedy match. It will match zero or more of any characters and does as many as possible while still allowing the pattern to match. A lazy match will do the opposite and match the least amount of characters needed to allow the pattern to match.

### Boundaries
boundaries specify a position where a match must occur. Boundaries within this expression are `^` and `$`. They signify the start and end of the string, and the pattern within these boundaries must match throughout the whole string. This is an implicit boundary rather than an explicit boundary.

### Back-references
The back reference `\1` is used to refer back to the first capturing group `([a-z]+)`. So whatever was matched by the first capturing group has to match again later in the pattern. This back reference makes sure that the closing tag `<\/\1>` matches the same tag as the opening tag.

### Look-ahead and Look-behind
There are no look behind and look ahead being used in this expression. Look behind and look ahead specifies conditions that need to be met after and/or before a match has been made.

## Author
Max Behrmann

GitHub profile link: https://github.com/mbman11


I am in a coding boot camp trying to learn as much as I can to become a web developer. I also have a background in UX/UI. I enjoy coding and am trying to really learn the fundamentals! Thanks for reading!

