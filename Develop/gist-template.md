# Title (replace with your title)

Introductory paragraph (replace this with your text)

## Summary

Below is a RegEx pattern example

/[A-Za-z0-9]{8,}/ would match any string that has a Capitalized A-Z, Lowercase A-Z, Numbers 0-9, and must be 8 or more characters long. This could be used to find or validate passwords with the specific set RegEx criteria.

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

Using the password example, we could add ^ and $ to the pattern as /^[A-Za-z0-9]{8,}$/ to indicate that the password string should be the entire string, with nothing before or after it.

### Quantifiers

Quantifiers identify various quantities of what the user is searching for. Ex- "*" placed after the keyword meaning "any" of what the user is searching for. The "+" sign after the keyword would mean the the pattern must appear at least once. A "?" sign after the keyword would indicate the pattern must appear 0- 1 times in the paragraoh. Any numbers wrapped in "{}" placed after te keyword would incicate how many times the user wants to recognize the pattern in the source string. 

An example would be the "{8,} suggesting that the password must be at least 8 characters long. /^[A-Za-z0-9]{8,}$/

### OR Operator

The OR Operator allows the user to user multiple search functionalities with the use of a "|" in between each keyword. This must be wrapped in a "()" to function. I.e - to search for "and", "or", "while" the user would type in "/(and|or|while)/".

### Character Classes

Character classes are a collection of related symbols usually wrapped in square brackets []. The common classes are letters, numbers, white spaces, etc. Regex has special syntax that assists in this such as "\w" for word letters, numbers, underscores & "\d" for numbers, & "\s" for inserting a white space in betwween keyword entries. 

Ex - /^\w{8,}$/ would be a shortened way of writing the exact same line of code on line 37 by utilizing Character Classes.

### Flags

Flags are almost like a filtering syastem the user can place before searching. This allows the user to narrow down their search based on which flag they've chosen. They're a letter added to the end of the pattern  

/pattern/i would indicate that to perform the match without considering capitalization. /test/i will match TEST, test, and TeSt, etc., but /test/ (without the i) would only match "test." 


### Grouping and Capturing

Grouping is a way of organizing your search based on sectioning off pieces in parenthesis in order to capture matches. 

Grouping "or" is when we use parentheses and the pipe (|) symbol to have options in the pattern. (Hi|Hello|Howdy|Yoyo) would match any of those words.

Grouping "capturing" is when use parentheses to recall some part of the matched pattern. /Hello (\w+)/ would match "Hello " followed by some text and "capture" the word that followed "Hello".

### Bracket Expressions

Brackets allow the user to narrow down their results by a specific range. Example - /ab/ would yield every "ab" in the document. /[ab]/ as a bracket expression would yield every "a" as well as every "b" in the document. 


### Greedy and Lazy Match

A greedy search attempts to find the largest possible match for a pattern. It is the default behavior.

A lazy search attempts to find the smallest possible match for a pattern. It is forced by adding a ? after the quantifier.

Example: .....

Greddy searches are made by default for the user to be able to capture everything within the pattern they're searching. By adding a "?" to the search, the user is using a "lazy match" that only displays the result of the first found pattern. 

### Boundaries

Boundaries allow the user to set a "\b" at the beginning or end of the pattern they're searching for. This will result in the user getting exactly the keyword they searched for with no additional letters attached. Example -"with" would result in with, withhold, wither, withdraw, etc. "\bwith\b" would result in only finding "with" and not other works such as "withhold", "wither", "withdraw".

### Back-references

Back references allows the user to recall previously typed pattern searches and recall them by their group number with a "\2" sign.   



### Look-ahead and Look-behind

The look ahead allows the user to sarch for a keyword pattern that is followed by another pattern. This will retrieve the first pattern the user is searching for without displaying the second pattern. Look behind functions the exact same way, except in reverse. 



## Author



<!-- GIVEN a regex tutorial

WHEN I open the tutorial
THEN I see a descriptive title and introductory paragraph explaining the purpose of the tutorial, a summary describing the regex featured in the tutorial, a table of contents linking to different sections that break down each component of the regex and explain what it does, and a section about the author with a link to the author’s GitHub profile


WHEN I click on the links in the table of contents
THEN I am taken to the corresponding sections of the tutorial


WHEN I read through each section of the tutorial
THEN I find a detailed explanation of what a specific component of the regex does


WHEN I reach the end of the tutorial
THEN I find a section about the author and a link to the author’s GitHub profile -->
