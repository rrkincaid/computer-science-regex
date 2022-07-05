# Computer Science RegEx

## MOD 17 HW

Please see below for a brief description / tutorial that covers using RegEx, in particular: matching an email. To understand this syntax better, we will break it down into smaller parts below. Please use the table of contents to navigate through these different components.

## Summary

RegEx is a shorthand way of saying Regular Expression and can be used when writing code to quickly convey symbol or letter perameters within the code you are writing.

Rather than writing several lines of code, you can utilize RegEx to limit the type of characters that you will accept.

For this particular example, we will go over matching an email.

    Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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

    Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Anchors

The ^ will be used when starting a regex to identify the beginning of the string.

If this is used within brackets: [ ^ ] it means that rather than include, we exclude the contents.

The $ on the other hand, identifies the end of the string.

### Quantifiers

As the name suggests, these indicate number of characters or expressions to match

- one or more
- { 3 }
  3x
- {2,4}
  two to four times
- {3,}
  three + times
- - zero + times
- ?
  once or none

### OR Operator

### Character Classes

Distinguish different types of characters

-[ … ]

-[x-y]
indicates a range

- [^x]
  indicates that whatever value x is, will be excluded from the perameters

- [^x-y]
  indicates that the value cannot be within this range

### Flags

#### i, g, m, s, u, y

- i
  indicates case-sensitive
- g
  widens search to look for all matches (rather than just the 1st one)
- m
  multiline mode
- s
  allows a dot ( . ) to match newline character /n
- u
  enables correct processing of surrogate pairs
- y
  searches at the exact position in the text

### Grouping and Capturing

This is a way to treat multiple characters as a single unit.

### Bracket Expressions

Consists of one or more expression and is eithre a matching or non-matching list

### Greedy and Lazy Match

Greedy Match - longest possible string

Lazy Match - shortest possible string

### Boundaries

Boundaries work similar to anchors, but are defined by use of a backslash and letter

### Back-references

RegEx command that refers to a previous part of the matched regex (specified by using a backslash and single digit: /1 )

### Look-ahead and Look-behind

Look-ahead:
Allows you to define patters that only match when they're followed or not followed by another pattern.

Look-behind:
Tells regex engine to temporarily step backwards in the string, to check if hte text inside can be matched there.

## Author

Rachel Kincaid

Rachel is a Colorado native who is currently enrolled in the DU Coding Bootcamp, honing her skills as a web developer. Link to repository below:

    Github: https://github.com/rrkincaid/computer-science-regex

## Misc

    Please note that certain anchors and boundaries, etc will differ depending on the language. This particular tutorial is intended for use in JS. Please go to the following site if reference for Python or Ruby, etc are desired: https://www.rexegg.com/
