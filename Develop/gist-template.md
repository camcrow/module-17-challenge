# Challenge 17 Regex Tutorial

Regex, short for regular expression, is a powerful tool used for pattern matching and manipulating text strings. Regex is a sequence of characters which defines a search pattern. This allows you to match, find, and replace patterns that are in larger text. 

## Summary

The regex that will be followed in this tutorial is used for matching emails. This regex provides the ability to validate the structure of an email address.

The regex for this can be seen below.

Matching Email: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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
The anchors of the regex enforce that the string from beginning to end must match the specified pattern. In this case the anchors would be ^ and $. 
### Quantifiers
The quantifiers of the regex modify the behavior of the expressions and determine how many times they need to match. In this regex they ensure that certain parts of the email address have specific constraints regarding how many numbers they can contain. 
In this case [a-z0-9_\.-]+ means that the characters in the square brackets can appear one or more time consecutively. {2,6} means that the expression should match a minimum of 2 times and maximum of 6 times.
### OR Operator
While there is not an OR operator present in this example what it would be represented by is the | symbol. This operator is used to specify alternative matches fora particular pattern. This allows you to define multiple options which can then be picked. For example (yes|no) matches either yes or no. If the input string contains either of these then it would be considered a match.
### Character Classes
Character Classes allow you to define a set of characters and specify that any character from that set can be matched in the string. This allows you to match a range of characters without specifying each individual character.
In this case there are two defined characters which are: [a-z0-9_\.-] and [a-z\.] The former matches any lowercase letter (a-z), digit (0-9), underscore (_), period (.), or hyphen (-). The latter matches any lowercase letter (a-z) or period (.).
### Flags
Flags in regular expressions are optional parameters that modify the nehavior of pattern matching. They are typically added after the closing delimiter of the regex. This matching email regex however does not have any flags specified.
### Grouping and Capturing
There are three groups in this regex that are indicated by the use of parenthesis. These are: ([a-z0-9_\.-]+), ([\da-z\.-]+), and ([a-z\.]{2,6}). Groups are useful when you want to retrieve or manipulate specific parts of the pattern. In this case they are used to identify and extract the username, domain name, and the TLD of the email address.
### Bracket Expressions
Bracket expressions allow you to define a set of characters from which a single character can be matched at a particular position in the string. There are three bracket expressions in this regex which are: [a-z0-9_\.-], [\da-z\.-], and [a-z\.].
### Greedy and Lazy Match
There is no greedy or lazy match in the given expression. Greedy matching is the default behavior in regular expressions where the quantifiers will match as much as possible while still allowing the pattern to match. Lazy matching matches the least possible while still allowing the pattern to match.
### Boundaries
There are no boundaries in the given expression. Boundaries are used to match specific positions in the string. 
### Back-references
There are no back-references in the given expression. Back-references provide a way to refer back to previously captured content within the expression.
### Look-ahead and Look-behind
There is no look-ahead and look-behind in the given expression. These allow you to specify conditions for matching without including the matched content in the final
## Author

This tutorial was created by Cameron Croteau.

Here's where you can find him!
Github.com/camcrow

