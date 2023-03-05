# wk17-regex


A regular expression, also known as regex, is a sequence of characters that forms a search pattern used to match and manipulate text. It is a powerful tool used in computer science, programming, and text processing to find and extract information from text by defining a specific pattern or set of rules which intern allows to check if a string contains a certain character or phrase.

## Summary

Hex values (Hexadecimals) are used throughout color coding where they are used to represent color in RGB format (red, green and blue). An example of this is a hexadecimal #2c333e which would have to match the criteria from this regex expression /^#?([a-f0-9]{6}|[a-f0-9]{3})$/. Hex values contain numbers and letters, numbers ranging from 0-9, letter from A-F or a-f A representing 10 and ascending through to F which is 15 with the numbering system that’s base is 16. This criterion must strictly meet the regular expression outlined each time to be a hexadecimal code.

## Table of Contents

Anchors

Quantifiers

Grouping Constructs

Bracket Expressions

Character Classes

The OR Operator

Regex Components

Anchors

Anchor

^ - is a character which states the beginning of the regex and which character it must start with. It must match the exact character so the “#” symbol must be at the start of the string.

E.G. “the” matches the string “the chair” this anchor tag is also case sensitive

Quantifiers

{} - Using quantifiers limits the amount the string that the regular expression matches. This includes the minimum or maximum number of characters that the regex looks for. In this example, we set a limit of 6 or 3 characters or using a or operator. So, a string can only be 3 or 6 characters long.

E.G. “{3-6}” indicates a string must range between 3 to 6 characters long

? - Indicates that a character can be used zero or once

In our hex example, we can see a "?" used which means the character # would have to be used either zero or once after looking for the Amont of occurrences required. So, it is optional to use a "#" symbol.

E.G. “#?” indicates that a “#” symbol can be used zero or once

Grouping Constructs

() - grouping constructs break up sections of a string to determine if they meet the requirements set out within the regex checking multiple parts of a string to check they match and meet the requirements needed. In our example, we see the quantifiers 6 and 3 placed after the bracket expressions between the operators which indicates that the unit within the brackets would have to set the number of characters between 6 or 3 while meeting the conditions within the brackets. Our grouping constructor wraps the expression with the "$" anchor that ends it and "#?" which starts it.

E.G. “(Hello){3}” indicates that anything inside the bracket must be repeated three times as stated by the quantifier.

Bracket Expressions

[] - Anything within a bracket expression must match a specific pattern of characters outlined within them. To outline a range a "–" is used for example any number between 0 to 9. In our example, the condition follows that there must be lower-case characters between a-f and/or a number between 0-9.

E.G. “[0-9a-f]” the string must contain at least one character ranging between 0-9 or a-f

Character Classes

0-9 – these must match one of the characters outlined within the range provided this could be numerical or alphabetic. In our example this is a 0-9 or a-f meaning any number between 0 and 9 and any lower-case letter between a – f .

E.G. 1-10 meaning number ranging from 1 to 10

The OR Operator

| - an OR Operator is a Boolean that matches expressions that come before or after it. In our example ([a-f0-9]{6}|[a-f0-9]{3}) this indicates before the operator which contains a quantifier of 6 and after which contains a quantifier of three are both valid on the condition the pattern contains either 6 or 3 characters.

E.G. x|y meaning either x or y can be used

## Author
  Thank you for reading my breakdown of a regex function validating the Hex value with all the regex functions relevant to the hex value given.
  
  I am currently a student at UOB completing a full stack development bootcamp with future plans to enter the world of tech as a software engineer. 