# Shrimp Regex

What is Regex?
- Regex is a series of pattern of character to validate user input with the provided parameters.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary. This can be added to code to define input validation for any required data that need to be inputted and checked that it meets the necessary parameters. This is mostly seen for password, username, email, and phone number entries. 

Code snippet: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/



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
* (period) - matches any single character except the newline character

* \w - matches any word character (alphanumeric character plus underscore)

* \W - matches any non-word character

* \d - matches any digit

* \D - matches any non-digit character
* \s - matches any whitespace character (space, tab, newline, and return)
* \S - matches any non-whitespace character
* \b - matches the empty string, but only at the start or end of a word
* \B - matches the empty string, but not at the start or end of a word
* \0 - matches the null character
* \n - matches a new line character
* \t - matches a tab character
* \v - matches a vertical tab character
* \f - matches a form feed character
* \r - matches a carriage return character
* \xhh - matches the character with the hexadecimal value hh
* \uhhhh - matches the character with the hexadecimal value hhhh
* \cX - matches the control character indicated by X

### Anchors
- The Anchors that can be the ^ that signifies the beginning of the string while the $ sign defines the ending of the string. For example lets say we wish to create the requirements for a password and we use the Regex ^([a-z0-9])$ it means we expect a it to have lowercase letters from a-z but also needs numbers. This expression ends with the dollar sign. 

### Quantifiers
- {} Quantifiers are in charge of defining the amount of characters needed in the expression with need the min required characters. For example [{5-9}] that means we should expect 5 character all teh wau to 9 needed for the expression to validate.

### OR Operator
- No 'OR' operator

### Character Classes
- The character class symbol '\d' is in charge of all single digit numbers in the expression. For example ([0-9]\) is in charge of matching all the digits inserted. This will not view 11 since it only does one digit numbers so it will match '1''1'. 

### Flags
- No 'Flags' in the expression

### Grouping and Capturing
- A straight forward definition of grouping the desired requirements for an input so that regex can match the provided data. This is inside parentheses that are mostly grouped for email names, domain name, and top-level domain.

* If we break up the expression on top we can break it into its three components the first ([a-z0-9_\.-]) which would be group #1. 
  - This expression is in charge of the name for the email. 

* The second group expression ([\da-z\.-]+).
  - This expression is in the domain name example being 'gmail' and can not have any numbers.

* The #3 group ([a-z\.]{2,6}).
  - This is requirement are for the top-level domain (.com/ .org)
### Bracket Expressions

- The bracket expression are used to match a single character of the inputted character possibilities. An example of this would be [a-z0-9_.-]. So this will match all the instances of a to z that are lowercase as well as any digit between 0 to 9 with an extra addition of underscore, period, and a hyphen.

### Greedy and Lazy Match
- The Greedy and Lazy match means to match as many possibilities of an instance so instead of the first instance it will continue to match. So as the name suggest it will match all the string. 

### Boundaries
- No Instance

### Back-references
- No instance

### Look-ahead and Look-behind
- No instance

## Author

A short section about the author with a link to the author's GitHub profile luisMtz-0 
- https://github.com/LuisMtz-0

