# Regex Tutorial for Matching an Email

For this tutorial, I will explain how to match an email using regex.

## Summary

In this tutorial I will describe the regex for matching an email, /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. 
I will explain how each character works in mathching the URL. 

## Table of Contents

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

## Regex Components

### Anchors
Anchors are characters that cause a match to succeed or fail depending on the position of the characters in the string, the anchors
used in the email expression are, ```^``` and ```$```. The ```^``` is always used at the beginning of the expression, and ```$```
signifies the end of the expression. 

### Quantifiers
A quantifier specifies how many instances of the previous element must be present in the string for a match to occur. The
quantifiers used in this expression are ```{}``` and ```+```. The ```{}``` will match between x and y consecutive occurrences, 
inclusive, of the preceding character or expression. The ```+``` matches one-or-more of the preceding character or expression. 
So it would combine the email name, email service and the .com. 

### OR Operator
There are no OR Operators in this expression. 

### Character Classes
A character class matches any one of the group of characters. The character class used here would be ```\d```, this class would match 
any digit between 0 and 9. For example, it could match '3' or '7' but if there was to be more than one digit it wouldn't match 
anything for that reason. 

### Flags
There are no Flags in this expression.

### Grouping and Capturing
Grouping constructs describe the subexpressions of a regular expression and capture the substrings of an input string. The grouping 
constructs used here are, ```([a-z0-9_\.-]+)```, ```([\da-z\.-]+)```, and ```([a-z\.]{2,6})```. You can usually identify the group by 
the parenthesis used. The first group is capturing the email name, the second group is capturing the email service, and the third 
group is capturing the .com in the email address.   

### Bracket Expressions
Brackets indicate a set of characters to match. Any individual character between the brackets will match, and you can also use a 
hyphen to define a set. The brackets used in this expression start and terminate bracket expressions.

### Greedy and Lazy Match
Greedy means your expression will match as large a group as possible, lazy means it will match the smallest group possible. 
The greedy match used in this expression are ```+``` and ```{}```, and they expand the match as far as they can through the provided 
text. 

### Boundaries
There are no Boundaries used in this expression. 

### Back-references
There are no Back-references used in this expression. 

### Look-ahead and Look-behind
There are no Look-ahead and Look-behind contents in this expression. 

## Author
My name is Angel Escobar and I am aspiring to become a Full-Stack Web Developer and you can find my projects at, 
https://github.com/angelgiovanna. 