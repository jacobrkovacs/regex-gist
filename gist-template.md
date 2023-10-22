# Matching a Hex Value

A gist that explains a regex

## Summary

This gist will go in detail on the components of a regex that can be used to match a hex value. The following regex expression will be explained in this gist: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`<br>
This regex is looking for a string that starts with # and is followed by either a mix of 6 characters that are either letters from a-f or numbers from 0-9 OR it's looking for the same thing but with only 3 characters following the #.

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
- To start, all regex need to be wrapped in `/` because every regex is considered a literal
### Anchors
- The two anchors in this regex are `^` and `$`
- The `^` shows that the string will start with the character(s) following the anchor. In our instance, that character would be the `#`
- the `$` indicates a string that ends with the characters that precede it
### Quantifiers
- The two quantifiers in this regex are `?` and `{6}/{3}`
- The `?` puts a hard limit on the string repeating itself. In this case, the string can only repeat zero or one time
- The `{6}/{3}` dictates how many characters need to be in the string. In this case, the string would need to be either 6 or 3 characters long
### Grouping Constructs
- The way to make groups or subexpressions is to use `()`. These parentheses are used to separate different parts of the expression. In this case, the regex we are using is separating `#` from the other characters in the string. 
### Bracket Expressions
- Anything inside the `[]` indicates a range of characters that can be used in the string. In this case, the string can only include any letter from lowercase a-f and any number from 0-9
### Character Classes
- Our regex does not use any character classes, but they are used for defining a set of characters that can be used in the string
### The OR Operator
- The OR operator is indicated by `|`. In this case, or regex looks for either `[a-f0-9]{6}` or `[a-f0-9]{3}`
### Flags
- Our regex doesn't use any flags, but what flags do are they add functionality or limits to the regex.
### Character Escapes
- Just like in other aspects of JavaScript, the `\` character indicates an escape character. Put it before a character that you don't want to be interpreted literally.
## Author
Jacob Kovacs is a fullstack bootcamp student trying to break in to the world of web development. https://github.com/jacobrkovacs
