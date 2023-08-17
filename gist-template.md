# Regex Tutorial: Understanding and Usage of URL Pattern Matching

## Introduction
Welcome to this Regex Tutorial: Understanding and Usage of URL Pattern Matching.
In this tutorial, we'll take a close look at regular expressions (regex), learning how to craft and employ them effectively to match and analyze URLs. With the growing importance of web-based applications, understanding URL pattern matching is a fundamental skill for developers. By the end of this tutorial, you'll possess a solid foundation in URL regex patterns and the practicality of its usage in web development. 

## Summary

URL regex code that we will be analyzing today: 
`/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/`

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

The regex begins with `^` and ends with `$`, which are anchors. `^` declares the start of the string, while `$` declares the end. This makes sure that the URL matches from beginning to end.

### Quantifiers

Quantifiers such as `?`, `+`, and `*` are essential to regular expressions! While `?` introduces flexibility by making the preceding group optional, `+` enforces the presence of one or more instances, and `*` holds zero or more occurrences. This trio of quantifiers proves invaluable for accommodating variations in matching patterns, including the recognition of "http://" or "https://".

### OR Operator

 The `|` symbol functions as an OR operator. It allows the regex to match either the preceding or following expression. In this regex, it's used within the character class [a-z\.]{2,6} to match either lowercase letters or dots with a length between 2 and 6.

### Character Classes

The square brackets `[...]` create a character group. `[\da-z.-]` matches numbers `(\d)`, small letters `(a-z)`, periods `(.)`, and dashes `(-)`. It helps find characters in domain names and path sections.

### Flags

Flags like `i` (case-insensitive) or `g` (global) control how the regex is applied. In this specific URL regex, no flags are used.

### Grouping and Capturing

Parentheses `()` are used for grouping and capturing subexpressions. In this example, `(https?:\/\/)` captures `"http://"` or `"https://"` at the start of the URL, `([\da-z\.-]+)` captures the domain name characters, and `([\/\w \.-]*)*` captures optional path segments.

### Bracket Expressions

Within `[...]`, `[a-z\.]` matches any lowercase letter or dot. Its usage is to match the given characters within the domain name.

### Greedy and Lazy Match

Employing the `*` and `*?` quantifiers, we have two matching styles for this regex. The `*` is greedy in its matching style and grabs plenty of characters, while the `*?` is lazy and grabs as few as possible.

### Boundaries



### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
