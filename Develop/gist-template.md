# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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

Anchors are considered placeholders where text begins or ends. They are used as "^" in the beginning of a word or "$" at the end of a word. 

### Quantifiers

Quantifiers identify various quantities of what the user is searching for. Ex- "*" placed after the keyword meaning "any" of what the user is searching for. The "+" sign after the keyword would mean the the pattern must appear at least once. A "?" sign after the keyword would indicate the pattern must appear 0- 1 times in the paragraoh. Any numbers wrapped in "{}" placed after te keyword would incicate how many times the user wants to recognize the pattern in the source string.

### OR Operator

The OR Operator allows the user to user multiple search functionalities with the use of a "|" in between each keyword. This must be wrapped in a "()" to function. I.e - to search for "and", "or", "while" the user would type in "/(and|or|while)/".

### Character Classes

Character classes are a collection of related symbols usually wrapped in square brackets []. The common classes are letters, numbers, white spaces, etc. Regex has special syntax that assists in this such as "\w" for word letters, numbers, underscores & "\d" for numbers, & "\s" for inserting a white space in betwween keyword entries. 

### Flags

Flags are almost like a filtering syastem the user can place before searching. This allows the user to narrow down their search based on which flag they've chosen. 

### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)

<!-- GIVEN a regex tutorial

WHEN I open the tutorial
THEN I see a descriptive title and introductory paragraph explaining the purpose of the tutorial, a summary describing the regex featured in the tutorial, a table of contents linking to different sections that break down each component of the regex and explain what it does, and a section about the author with a link to the author’s GitHub profile


WHEN I click on the links in the table of contents
THEN I am taken to the corresponding sections of the tutorial


WHEN I read through each section of the tutorial
THEN I find a detailed explanation of what a specific component of the regex does


WHEN I reach the end of the tutorial
THEN I find a section about the author and a link to the author’s GitHub profile -->
