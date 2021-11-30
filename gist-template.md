# REGEX TUTORIAL: How to Match HEX Values

<!-- Introductory paragraph (replace this with your text) -->
This tutorial is to provide an introduction to regular expressions and demonstrate how they function. A regular expression , also known as regex, is a sequence of characters that define a search pattern. They are used to find, match, or authorize valid input strings. For this tutorial, we will go over thye regular expression to match a HEX value. 

## Summary

The displayed regular expression below is used to match HEX values: 

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

<!-- Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary. -->

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

Anchors don't necessary match any regular expressions, but assert something about the string. Like a beginning and end of a string. Shown below is the anchors that are used: 

* `^` marks the beginning of the string
* `$` mariks the end of the string

Here is an example: 

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

As you can see, the string starts with `^` and ends with `$`.

### Quantifiers

Quantifiers surrounds the number of characters to match. Shown below is the charcters that will be  anaylze: 

Code Snipet:  ` /^#?([a-f0-9]{6} `

 * `+` the element may be repeated 1 or more times
 * `*` the element may be repeated 1 or more times, as well as 0 times
 * `?` the element is optional, match8ing 0 or 1 occurances 
 * ` {n} ` a single or a range of numbers 

` #? ` indicates that both HEX values are both matches. 


The `{n} ` quantifiers outlines that the HEX values are exactly ` {6} ` digits  or `{3}` digits long.


### Grouping Constructs

` ([a-f0-9]{6}|[a-f0-9]{3}) `

The regex outlines characters by using `( ) ` parentheses to group all of htem together.  As seen below, the multiple characters withing ` ( ) ` are a single unit. 

### Bracket Expressions

The brackets ` [ ] ` are used to define the pattern of character sets. 
 
 * The bracket expression ` [a-z ] ` pulls all the alphabet letters from a to z 
 * The bracket expression ` [0-9 ]` shows all whole numbers from 0-9

Code Snipet: ` [a-f0-9] `

For this HEX Value, it pulls all the alphabet letters from a to f and will display whole numberrs from 0 to 9.


### Character Classes

Character classes only match oen out of several characters defined in the character set. 

Code Snipet: ` a-f0-9 ` 

A hypen is used inside a character class to define the range of characters, as shown above. 


### OR Operator 

Code Snipet : ` [a-f0-9]{6}|[a-f0-9]{3}` 

The OR Operator ` | ` communicates to the regular expression to match the pattern either before or after. 

In this regular expression, the OR Operator shows that the matching pattern ` [a-f0-p] `  implies match with three character string containing lower case ` a-f ` with an integer ` 0-9 ` OR a string with 6 characters containing lowercase ` a-f ` between ` 0-9`. Therefore, a matching string has to have 3-6 characters with the specified pattern. Anything beyond 3-6 characters will not match. 

### Flags

### Character Escapes

## Author

My name is Miranda Zermeno. This tutorial was created for Full-Stack Web Developer Bootcamp program at Southern Methodist University.  I am an inspiring web developer, who wishes to expand their creativity and knowledge within web technologies. I selected HEX values, because it allowed me to learn more about color system that accuratley communicates to the computer to ensure consistency and accuracey in a electronic display. My GitHub page reflects the assignments/projects that I created thus far in the program: https://github.com/Zermeno94 . 
<!-- A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile) -->