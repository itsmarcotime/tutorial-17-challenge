# Matching Hex values using regular expressions!

This will be a turtorial on how to use regular expressions to find hex values

## Summary

this will be the regular expresion I will be evaluating:

/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)

## Regex Components

### Anchors 
There are two anchors used in the hex regular expression. The anchors used are "^" & "$". The "^" just represents the beginning of the regular expression. The "$" represents the end of the regular expression.

### Quantifiers
There are two quantifiers used in thi regular expresion. The two quantifiers are "?" ang "{x}". 

The "?" matches anything that precedes it. In our regular expression we have "#?" so this will match anything that starts with "#".

We also have a {x} quantifier. This will match to x amount of characters in the search. So in the case of our expression we have {6} & {3}. So our regular expresion will look for a sequence of 6 charatcers AND a sequence of 3 characters.

### OR Operator

In our expression /^#?([a-f0-9]{6}|[a-f0-9]{3})$/ you will see a "|" right after the {6} quantifier. The "|" is a OR operator that splits our expression into two peices "[a-f0-9]{6}" & "[a-f0-9]{3}". So the Or Operator will look for either a sequence of "[a-f0-9]{6}", or a sequence of "[a-f0-9]{3}".

### Character Classes

In our regular expresion we have a two classes but it is really just one class that is repeated twice. The two classes that are used in our expresion is just "[a-f0-9]" repeated twice. An investigation of this class will reveal that we are looking for characters between the ranges of "a" through "f" not including uppercase, and we are also looking for numbers between the ranges "0" through "9". 

## Author

This was created by Marco Mata. The profile of my github will be linked below.

github repo link:
https://github.com/itsmarcotime
