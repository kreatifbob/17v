# REGEX MATCHING AN EMAIL

## Summary

A tutorial which explains the email matching regex for:

/^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)

- [Character Classes](#character-classes)
- [Bracket Expressions](#bracket-expressions)
- [Grouping and Capturing](#grouping-and-capturing)

- [Greedy](#greedy match)
- [Quantifiers](#quantifiers)

- [Other Regex Components]
- [OR Operator](#or-operator)
- [Lazy](#lazy match)
- [Flags](#flags)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Components

- [Anchors](#anchors)
  ^ asserts position at start of the string
  $ asserts position at the end of the string, or before the line terminator right at the end of the string (if any)

- [Character Classes](#character-classes)
- [Bracket Expressions](#bracket-expressions)
- [Grouping and Capturing](#grouping-and-capturing)
  1st Capturing Group and/or Character Class is
  ([a-z0-9_\.-]+)
  Matches a single character present from emails [a-z0-9_\.-]

2nd Capturing Group and/or Character Class is ([\da-z\.-]+)
Matches a single character present from emails [\da-z\.-]

3rd Capturing Group and/or Character Class is ([a-z\.]{2,6})
Matches a single character present from emails [a-z\.]

- [Greedy](#greedy match)
  From 1st Capturing Group

* matches the previous token between one and unlimited times, as many times as possible, giving back as needed (greedy)
  From 3rd Capturing Group
  {2,6} matches the previous token between 2 and 6 times, as many times as possible, giving back as needed (greedy)

- [Quantifiers](#quantifiers)

The "+" symbol is used at the end of 2nd capturing group as Quantifier

a-z matches a single character in the range between a and z (case sensitive)
0-9 matches a single character in the range between 0 and 9 (case sensitive)
\d matches a digit (equivalent to [0-9])
a-z matches a single character in the range between a and z case sensitive)

- [Other Regex Components]
- [OR Operator](#or-operator)
  Not used
- [Lazy](#lazy match)
  Not used
- [Flags](#flags)
  Not used

- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

Can be used but does not apply

## Gist Profile & Author

Gist Revisions can be fpund here
https://gist.github.com/kreatifbob/9c4d3fb3ad9e42c132e70a19ed72b116
Tanel Colak https://github.com/kreatifbob/Regex
