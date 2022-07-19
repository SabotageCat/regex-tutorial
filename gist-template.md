# REGEX Tutorial
A Regular Expression or REGEX is a sequence a characters that defines a search pattern for text. REGEX are used to look for and match emails, urls, phone numbers, html tags, and many more ways. This allows web developers and others to filter and check for correct user input in forms and as well as defining limits and boundaries on text data.
## Summary
In this tutorial I will explain the following REGEX for an email. This REGEX matches emails.

REGEX for matching a URL
`/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

This REGEX is checking for:
- an email address with letters a-z and numbers 0-9
- an email with an @ symbol
- an email with a domain name ending with a period
- an email with a domain ending after the period that is 2-6 characters long

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
REGEX are written between two forward slashes `//` and contain components which define the search parameters. Components are customizable and allow you to create a REGEX for your needs!
### Anchors
There are two main anchors. The `^` anchor starts a regex literal and a `$` terminates it.
Our REGEX begins and ends as such `/^([a-z0-9_\.-]+)...` `...([a-z\.]{2,6})$/`
### Quantifiers
Quantifiers come in 3 main types. As proceeding to indicate zero or more `*`, one or more `+`, zero or one `?`, and specific or a range of multiples `{2} {2,} {2,5}`.
Our REGEX contains one after the first group `[a-z0-9_\.-]+`, and in the second group `[\da-z\.-]+` indicating here that there are one or more characters. As well as at the end `[a-z\.]{2,6}` to indicate 2 to 6 characters at the end of the email address.
### OR Operator
The OR operator comes as a `|` or  `[]`. An OR operator may be used as such `a|b`, `a[b]` to indicate either a or b.
### Character Classes
Character classes match a character from a set with a character set `[ABC]`, negated set `[^ABC]`, range `[A-Z]`, any `[\s\S]`, digit `\d`, and word `\w`.
Our REGEX contains 3 sets of character classes `[a-z0-9_\.-]` `[\da-z\.-]` `[a-z\.]` each searching for a specific string of letters, numbers and a period.
### Flags
Flags change how a regular expression (REGEX) is interpreted. A `g` flag is a global search. A `m` flag is a multiline search. A `i` flag is an ignore case that makes the REGEX case insensitive.
### Grouping and Capturing
Groups are placed between `()` and allow you to group sequences and use them together.
Our REGEX contains 3 groups `([a-z0-9_\.-]+)` `([\da-z\.-]+)` `([a-z\.]{2,6})`
### Bracket Expressions
Bracket Expressions are used in character classes to match a set.
Our REGEX contains 3 sets of character classes `[a-z0-9_\.-]` `[\da-z\.-]` `[a-z\.]` each searching for a specific string of letters, numbers and a period.
### Greedy and Lazy Match
Greedy expands the matches to as many as possible and its operators include `*`, `+`, `{}`
Lazy limits our matches and its operators include `?`.
Our REGEX has greedy operators after each bracket to include multiple characters, `[a-z0-9_\.-]+` `[\da-z\.-]+` `[a-z\.]{2,6}`
### Boundaries
Boundaries can exclude or include word boundaries for REGEX. Boundary operators are `\b` to indicate a word boundary, or `\B` to indicate a non-word boundary.
### Back-references
Back references match characters to a previous group in the REGEX. It is used with a forward slash and a number or such as `\1`, or name for that previous group with a foward slash and the letter k with the group name within less than and greater than signs, `\k<foo>`
### Look-ahead and Look-behind
Look ahead is used to match or fail a pattern using these operators `(?=)` `(?!)`. Look behind is used to match or fail patterns before the given components using operators `(?<=)` `(?<!)`
## Author

Hello! My Name is Robert David and i'm a web developer! Check out my github * [SabotageCat](<https://github.com/SabotageCat>)